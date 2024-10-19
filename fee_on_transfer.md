
<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer"></a>

# Module `0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::fee_on_transfer`



-  [Resource `FeeOnTransferInfo`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_FeeOnTransferInfo)
-  [Struct `FeeOnTransferInfoInitialized`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_FeeOnTransferInfoInitialized)
-  [Struct `LiquidityUpdated`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_LiquidityUpdated)
-  [Struct `RewardsUpdated`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_RewardsUpdated)
-  [Struct `TeamUpdated`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_TeamUpdated)
-  [Function `assert_owner`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_assert_owner)
-  [Function `initialize_fee_on_transfer`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_initialize_fee_on_transfer)
-  [Function `set_liquidity_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_liquidity_fee)
-  [Function `set_rewards_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_rewards_fee)
-  [Function `set_team_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_team_fee)
-  [Function `set_all_fees`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_all_fees)
-  [Function `does_not_exceed_fee_on_transfer_threshold`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_does_not_exceed_fee_on_transfer_threshold)
-  [Function `fee_on_transfer_parameters`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_fee_on_transfer_parameters)
-  [Function `owner`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_owner)
-  [Function `liquidity_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_liquidity_fee)
-  [Function `team_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_team_fee)
-  [Function `rewards_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_rewards_fee)
-  [Function `all_fee_on_transfer`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_all_fee_on_transfer)
-  [Function `is_created`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_is_created)


<pre><code><b>use</b> <a href="">0x1::event</a>;
<b>use</b> <a href="">0x1::fungible_asset</a>;
<b>use</b> <a href="">0x1::object</a>;
<b>use</b> <a href="">0x1::option</a>;
<b>use</b> <a href="">0x1::signer</a>;
<b>use</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::admin</a>;
<b>use</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::constants</a>;
<b>use</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::errors</a>;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_FeeOnTransferInfo"></a>

## Resource `FeeOnTransferInfo`

used to store the token owner and the token fee; needed for Individual token fees


<pre><code><b>struct</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_FeeOnTransferInfo">FeeOnTransferInfo</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_FeeOnTransferInfoInitialized"></a>

## Struct `FeeOnTransferInfoInitialized`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_FeeOnTransferInfoInitialized">FeeOnTransferInfoInitialized</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_LiquidityUpdated"></a>

## Struct `LiquidityUpdated`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_LiquidityUpdated">LiquidityUpdated</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_RewardsUpdated"></a>

## Struct `RewardsUpdated`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_RewardsUpdated">RewardsUpdated</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_TeamUpdated"></a>

## Struct `TeamUpdated`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_TeamUpdated">TeamUpdated</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_assert_owner"></a>

## Function `assert_owner`

Assert the address is the owner of the token


<pre><code><b>public</b> <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_assert_owner">assert_owner</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, addr: <b>address</b>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_initialize_fee_on_transfer"></a>

## Function `initialize_fee_on_transfer`

token owners will to specify the cointype and input the fees.


<pre><code><b>public</b> entry <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_initialize_fee_on_transfer">initialize_fee_on_transfer</a>(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, liquidity_fee: u128, rewards_fee: u128, team_fee: u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_liquidity_fee"></a>

## Function `set_liquidity_fee`

update fee_on_transfer liquidity fee


<pre><code><b>public</b> entry <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_liquidity_fee">set_liquidity_fee</a>(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, new_fee: u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_rewards_fee"></a>

## Function `set_rewards_fee`

update fee_on_transfer rewards fee


<pre><code><b>public</b> entry <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_rewards_fee">set_rewards_fee</a>(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, new_fee: u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_team_fee"></a>

## Function `set_team_fee`

update fee_on_transfer team fee


<pre><code><b>public</b> entry <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_team_fee">set_team_fee</a>(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, new_fee: u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_all_fees"></a>

## Function `set_all_fees`

update fee_on_transfer all fees


<pre><code><b>public</b> entry <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_set_all_fees">set_all_fees</a>(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, new_liquidity_fee: u128, new_rewards_fee: u128, new_team_fee: u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_does_not_exceed_fee_on_transfer_threshold"></a>

## Function `does_not_exceed_fee_on_transfer_threshold`

returns true if given rate is less than the individual token threshold


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_does_not_exceed_fee_on_transfer_threshold">does_not_exceed_fee_on_transfer_threshold</a>(total_fees_numerator: u128): bool
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_fee_on_transfer_parameters"></a>

## Function `fee_on_transfer_parameters`

Returns the token fee on transfer parameters


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_fee_on_transfer_parameters">fee_on_transfer_parameters</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): (u128, u128, u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_owner"></a>

## Function `owner`

Returns the owner of the fa


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_owner">owner</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): <b>address</b>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_liquidity_fee"></a>

## Function `liquidity_fee`

Returns the liquidity fee


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_liquidity_fee">liquidity_fee</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_team_fee"></a>

## Function `team_fee`

Returns the rewards fee


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_team_fee">team_fee</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_rewards_fee"></a>

## Function `rewards_fee`

Returns the team fee


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_rewards_fee">rewards_fee</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_all_fee_on_transfer"></a>

## Function `all_fee_on_transfer`

Returns the total fee on transfer fees for a given token


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_all_fee_on_transfer">all_fee_on_transfer</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_is_created"></a>

## Function `is_created`

Checks if the fee on transfer is created


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer_is_created">is_created</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): bool
</code></pre>
