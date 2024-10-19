
<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake"></a>

# Module `0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::stake`



-  [Resource `TokenPairRewardsPool`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_TokenPairRewardsPool)
-  [Resource `UserInfoRegistry`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_UserInfoRegistry)
-  [Resource `RewardsPoolUserInfo`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_RewardsPoolUserInfo)
-  [Function `create_pool`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_create_pool)
-  [Function `deposit`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_deposit)
-  [Function `withdraw`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_withdraw)
-  [Function `add_rewards`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_add_rewards)
-  [Function `claim_rewards`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_claim_rewards)
-  [Function `is_pool_created`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_is_pool_created)
-  [Function `token_rewards_pool_info`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_token_rewards_pool_info)
-  [Function `rewards_fees_accumulated`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_rewards_fees_accumulated)
-  [Function `distribute_rewards`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_distribute_rewards)


<pre><code><b>use</b> <a href="">0x1::dispatchable_fungible_asset</a>;
<b>use</b> <a href="">0x1::fungible_asset</a>;
<b>use</b> <a href="">0x1::object</a>;
<b>use</b> <a href="">0x1::option</a>;
<b>use</b> <a href="">0x1::primary_fungible_store</a>;
<b>use</b> <a href="">0x1::signer</a>;
<b>use</b> <a href="">0x1::smart_table</a>;
<b>use</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::admin</a>;
<b>use</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::common</a>;
<b>use</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::constants</a>;
<b>use</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::errors</a>;
<b>use</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::fee_on_transfer</a>;
<b>use</b> <a href="math.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_math">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::math</a>;
<b>use</b> <a href="u256.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_u256">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::u256</a>;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_TokenPairRewardsPool"></a>

## Resource `TokenPairRewardsPool`



<pre><code><b>struct</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_TokenPairRewardsPool">TokenPairRewardsPool</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_UserInfoRegistry"></a>

## Resource `UserInfoRegistry`

Global storage for user info in a rewards pool <pool_addr, info_addr>


<pre><code><b>struct</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_UserInfoRegistry">UserInfoRegistry</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_RewardsPoolUserInfo"></a>

## Resource `RewardsPoolUserInfo`



<pre><code><b>struct</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_RewardsPoolUserInfo">RewardsPoolUserInfo</a> <b>has</b> store, key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_create_pool"></a>

## Function `create_pool`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_create_pool">create_pool</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_deposit"></a>

## Function `deposit`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_deposit">deposit</a>(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_withdraw"></a>

## Function `withdraw`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_withdraw">withdraw</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_add_rewards"></a>

## Function `add_rewards`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_add_rewards">add_rewards</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_claim_rewards"></a>

## Function `claim_rewards`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_claim_rewards">claim_rewards</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_is_pool_created"></a>

## Function `is_pool_created`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_is_pool_created">is_pool_created</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): bool
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_token_rewards_pool_info"></a>

## Function `token_rewards_pool_info`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_token_rewards_pool_info">token_rewards_pool_info</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): (u64, u64, u64, u128, u128, u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_rewards_fees_accumulated"></a>

## Function `rewards_fees_accumulated`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_rewards_fees_accumulated">rewards_fees_accumulated</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): (u64, u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_distribute_rewards"></a>

## Function `distribute_rewards`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake_distribute_rewards">distribute_rewards</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, rewards_x: <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>, rewards_y: <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>)
</code></pre>
