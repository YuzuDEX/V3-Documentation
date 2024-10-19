
<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router"></a>

# Module `0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::router`



-  [Function `create_pair`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_create_pair)
-  [Function `register_fee_on_transfer_in_a_pair`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_register_fee_on_transfer_in_a_pair)
-  [Function `stake`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_stake)
-  [Function `unstake`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_unstake)
-  [Function `claim_rewards`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_claim_rewards)
-  [Function `add_liquidity`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_add_liquidity)
-  [Function `remove_liquidity`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_remove_liquidity)
-  [Function `add_rewards_to_pool`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_add_rewards_to_pool)
-  [Function `swap_exact_input`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_input)
-  [Function `multi_hop_exact_input`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_multi_hop_exact_input)
-  [Function `swap_exact_output`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_output)
-  [Function `update_fee_tier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_update_fee_tier)
-  [Function `amount_in`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_amount_in)
-  [Function `amount_out`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_amount_out)
-  [Function `swap_exact_x_to_y_direct_external`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_x_to_y_direct_external)


<pre><code><b>use</b> <a href="">0x1::fungible_asset</a>;
<b>use</b> <a href="">0x1::object</a>;
<b>use</b> <a href="">0x1::signer</a>;
<b>use</b> <a href="">0x1::string</a>;
<b>use</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::common</a>;
<b>use</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::errors</a>;
<b>use</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::stake</a>;
<b>use</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::swap</a>;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_create_pair"></a>

## Function `create_pair`

Create a pair of X and Y tokens
Should revert if the pair is already created


<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_create_pair">create_pair</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, icon_uri: <a href="_String">string::String</a>, project_uri: <a href="_String">string::String</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_register_fee_on_transfer_in_a_pair"></a>

## Function `register_fee_on_transfer_in_a_pair`

Add fee on transfer to a pair; callable only by owners of X or Y


<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_register_fee_on_transfer_in_a_pair">register_fee_on_transfer_in_a_pair</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_stake"></a>

## Function `stake`



<pre><code><b>public</b> entry <b>fun</b> <a href="">stake</a>(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_unstake"></a>

## Function `unstake`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_unstake">unstake</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_claim_rewards"></a>

## Function `claim_rewards`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_claim_rewards">claim_rewards</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_add_liquidity"></a>

## Function `add_liquidity`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_add_liquidity">add_liquidity</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount_x_desired: u64, amount_y_desired: u64, amount_x_min: u64, amount_y_min: u64, icon_uri: <a href="_String">string::String</a>, project_uri: <a href="_String">string::String</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_remove_liquidity"></a>

## Function `remove_liquidity`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_remove_liquidity">remove_liquidity</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, liquidity: u64, amount_x_min: u64, amount_y_min: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_add_rewards_to_pool"></a>

## Function `add_rewards_to_pool`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_add_rewards_to_pool">add_rewards_to_pool</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_input"></a>

## Function `swap_exact_input`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_input">swap_exact_input</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, x_in: u64, y_min_out: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_multi_hop_exact_input"></a>

## Function `multi_hop_exact_input`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_multi_hop_exact_input">multi_hop_exact_input</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, z_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, x_in: u64, y_min_out: u64, z_min_out: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_output"></a>

## Function `swap_exact_output`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_output">swap_exact_output</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_out: u64, x_max_in: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_update_fee_tier"></a>

## Function `update_fee_tier`



<pre><code><b>public</b> entry <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_update_fee_tier">update_fee_tier</a>&lt;Tier&gt;(signer_ref: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_amount_in"></a>

## Function `amount_in`



<pre><code><b>public</b> <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_amount_in">amount_in</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_out_amount: u64): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_amount_out"></a>

## Function `amount_out`



<pre><code><b>public</b> <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_amount_out">amount_out</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, x_in_amount: u64): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_x_to_y_direct_external"></a>

## Function `swap_exact_x_to_y_direct_external`



<pre><code><b>public</b> <b>fun</b> <a href="router.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_router_swap_exact_x_to_y_direct_external">swap_exact_x_to_y_direct_external</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, x_in: <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>): <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>
</code></pre>
