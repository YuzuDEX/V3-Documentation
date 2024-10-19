
<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap"></a>

# Module `0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::swap`



-  [Resource `TokenPairMetadata`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_TokenPairMetadata)
-  [Resource `TokenPairReserve`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_TokenPairReserve)
-  [Struct `PairCreatedEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_PairCreatedEvent)
-  [Struct `LiquidityAdded`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_LiquidityAdded)
-  [Struct `LiquidityRemoved`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_LiquidityRemoved)
-  [Struct `SwapEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_SwapEvent)
-  [Struct `FeeOnTransferRegistered`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_FeeOnTransferRegistered)
-  [Function `add_swap_event_with_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_swap_event_with_address)
-  [Function `assert_owner`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_assert_owner)
-  [Function `toggle_all_fees`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_all_fees)
-  [Function `toggle_liquidity_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_liquidity_fee)
-  [Function `toggle_team_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_team_fee)
-  [Function `toggle_rewards_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_rewards_fee)
-  [Function `add_liquidity`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_liquidity)
-  [Function `remove_liquidity`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_remove_liquidity)
-  [Function `create_pair`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_create_pair)
-  [Function `add_fee_on_transfer_in_pair`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_fee_on_transfer_in_pair)
-  [Function `swap_exact_x_to_y_direct`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_x_to_y_direct)
-  [Function `swap_exact_x_to_y`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_x_to_y)
-  [Function `swap_x_to_exact_y`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_x_to_exact_y)
-  [Function `swap_x_to_exact_y_direct`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_x_to_exact_y_direct)
-  [Function `swap_exact_y_to_x_direct`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_y_to_x_direct)
-  [Function `swap_exact_y_to_x`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_y_to_x)
-  [Function `swap_y_to_exact_x`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_y_to_exact_x)
-  [Function `total_lp_supply`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_total_lp_supply)
-  [Function `liquidity_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_liquidity_fee)
-  [Function `token_fees`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_fees)
-  [Function `token_reserves`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_reserves)
-  [Function `token_balances`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_balances)
-  [Function `lp_balance`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_lp_balance)
-  [Function `reserve`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_reserve)
-  [Function `is_fee_on_transfer_registered`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_is_fee_on_transfer_registered)
-  [Function `dex_fees_in_a_pair`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_dex_fees_in_a_pair)
-  [Function `is_pair_created`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_is_pair_created)
-  [Function `pair_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_pair_address)
-  [Function `update_fee_tier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_update_fee_tier)


<pre><code><b>use</b> <a href="">0x1::dispatchable_fungible_asset</a>;
<b>use</b> <a href="">0x1::event</a>;
<b>use</b> <a href="">0x1::fungible_asset</a>;
<b>use</b> <a href="">0x1::object</a>;
<b>use</b> <a href="">0x1::option</a>;
<b>use</b> <a href="">0x1::primary_fungible_store</a>;
<b>use</b> <a href="">0x1::signer</a>;
<b>use</b> <a href="">0x1::string</a>;
<b>use</b> <a href="">0x1::timestamp</a>;
<b>use</b> <a href="">0x1::type_info</a>;
<b>use</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::admin</a>;
<b>use</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::common</a>;
<b>use</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::constants</a>;
<b>use</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::errors</a>;
<b>use</b> <a href="fee_on_transfer.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_fee_on_transfer">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::fee_on_transfer</a>;
<b>use</b> <a href="math.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_math">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::math</a>;
<b>use</b> <a href="stake.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_stake">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::stake</a>;
<b>use</b> <a href="u256.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_u256">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::u256</a>;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_TokenPairMetadata"></a>

## Resource `TokenPairMetadata`

Stores the metadata required for the token pairs


<pre><code><b>struct</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_TokenPairMetadata">TokenPairMetadata</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_TokenPairReserve"></a>

## Resource `TokenPairReserve`

Stores the reservation info required for the token pairs


<pre><code><b>struct</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_TokenPairReserve">TokenPairReserve</a> <b>has</b> <b>copy</b>, store, key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_PairCreatedEvent"></a>

## Struct `PairCreatedEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_PairCreatedEvent">PairCreatedEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_LiquidityAdded"></a>

## Struct `LiquidityAdded`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_LiquidityAdded">LiquidityAdded</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_LiquidityRemoved"></a>

## Struct `LiquidityRemoved`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_LiquidityRemoved">LiquidityRemoved</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_SwapEvent"></a>

## Struct `SwapEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_SwapEvent">SwapEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_FeeOnTransferRegistered"></a>

## Struct `FeeOnTransferRegistered`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_FeeOnTransferRegistered">FeeOnTransferRegistered</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_swap_event_with_address"></a>

## Function `add_swap_event_with_address`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_swap_event_with_address">add_swap_event_with_address</a>(sender_addr: <b>address</b>, amount_x_in: u64, amount_y_in: u64, amount_x_out: u64, amount_y_out: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_assert_owner"></a>

## Function `assert_owner`

Assert the address is the owner of the token


<pre><code><b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_assert_owner">assert_owner</a>(metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, addr: <b>address</b>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_all_fees"></a>

## Function `toggle_all_fees`

toggle all individual token fees in a token pair; given CoinType, and a Token Pair


<pre><code><b>public</b> entry <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_all_fees">toggle_all_fees</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, activate: bool)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_liquidity_fee"></a>

## Function `toggle_liquidity_fee`

Toggle liquidity fee


<pre><code><b>public</b> entry <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_liquidity_fee">toggle_liquidity_fee</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, activate: bool)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_team_fee"></a>

## Function `toggle_team_fee`

Toggle team fee


<pre><code><b>public</b> entry <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_team_fee">toggle_team_fee</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, activate: bool)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_rewards_fee"></a>

## Function `toggle_rewards_fee`

Toggle rewards fee for a token in a token pair


<pre><code><b>public</b> entry <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_toggle_rewards_fee">toggle_rewards_fee</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, activate: bool)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_liquidity"></a>

## Function `add_liquidity`

Add more liquidity to token types. This method explicitly assumes the
min of both tokens are 0.


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_liquidity">add_liquidity</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount_x: u64, amount_y: u64): (u64, u64, u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_remove_liquidity"></a>

## Function `remove_liquidity`

Remove liquidity to token types.


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_remove_liquidity">remove_liquidity</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, liquidity: u64): (u64, u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_create_pair"></a>

## Function `create_pair`

Create the specified coin pair; all fees are toggled off
Returns the address for the LP token metadata


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_create_pair">create_pair</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, icon_uri: <a href="_String">string::String</a>, project_uri: <a href="_String">string::String</a>): <b>address</b>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_fee_on_transfer_in_pair"></a>

## Function `add_fee_on_transfer_in_pair`

Register a pair; callable only by token owners; a one time operation in a pair


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_add_fee_on_transfer_in_pair">add_fee_on_transfer_in_pair</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_x_to_y_direct"></a>

## Function `swap_exact_x_to_y_direct`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_x_to_y_direct">swap_exact_x_to_y_direct</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, coins: <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>): <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_x_to_y"></a>

## Function `swap_exact_x_to_y`

Swap X to Y, X is in and Y is out. This method assumes amount_out_min is 0


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_x_to_y">swap_exact_x_to_y</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount_in: u64, <b>to</b>: <b>address</b>): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_x_to_exact_y"></a>

## Function `swap_x_to_exact_y`

Swap Y to X, Y is in and X is out.


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_x_to_exact_y">swap_x_to_exact_y</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount_in: u64, amount_out: u64, <b>to</b>: <b>address</b>): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_x_to_exact_y_direct"></a>

## Function `swap_x_to_exact_y_direct`

Swap X to Y, X is in and Y is out.


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_x_to_exact_y_direct">swap_x_to_exact_y_direct</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, coins_in: <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>, amount_out: u64): (<a href="_FungibleAsset">fungible_asset::FungibleAsset</a>, <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_y_to_x_direct"></a>

## Function `swap_exact_y_to_x_direct`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_y_to_x_direct">swap_exact_y_to_x_direct</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, coins: <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>): <a href="_FungibleAsset">fungible_asset::FungibleAsset</a>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_y_to_x"></a>

## Function `swap_exact_y_to_x`

Swap Y to X, Y is in and X is out. This method assumes amount_out_min is 0


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_exact_y_to_x">swap_exact_y_to_x</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount_in: u64, <b>to</b>: <b>address</b>): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_y_to_exact_x"></a>

## Function `swap_y_to_exact_x`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_swap_y_to_exact_x">swap_y_to_exact_x</a>(sender: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, amount_in: u64, amount_out: u64, <b>to</b>: <b>address</b>): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_total_lp_supply"></a>

## Function `total_lp_supply`

Get the total supply of LP Tokens


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_total_lp_supply">total_lp_supply</a>(lp_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_liquidity_fee"></a>

## Function `liquidity_fee`

Get the current liquidity fee for a token pair


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_liquidity_fee">liquidity_fee</a>(lp_addr: <b>address</b>): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_fees"></a>

## Function `token_fees`

Get the current fees for a token pair


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_fees">token_fees</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_reserves"></a>

## Function `token_reserves`

Get the current reserves of T0 and T1 with the latest updated timestamp


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_reserves">token_reserves</a>(x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): (u64, u64, u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_balances"></a>

## Function `token_balances`

The amount of balance currently in pools of the liquidity pair


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_token_balances">token_balances</a>(lp_addr: <b>address</b>): (u64, u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_lp_balance"></a>

## Function `lp_balance`

Obtain the LP token balance of <code>addr</code>.
This method can only be used to check other users' balance.


<pre><code><b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_lp_balance">lp_balance</a>(lp_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, addr: <b>address</b>): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_reserve"></a>

## Function `reserve`

return pair reserve if it's created


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_reserve">reserve</a>(lp_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_TokenPairReserve">swap::TokenPairReserve</a>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_is_fee_on_transfer_registered"></a>

## Function `is_fee_on_transfer_registered`

return true if fee_on_transfer is registered in a pair


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_is_fee_on_transfer_registered">is_fee_on_transfer_registered</a>(lp_addr: <b>address</b>, metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): bool
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_dex_fees_in_a_pair"></a>

## Function `dex_fees_in_a_pair`

returns dex fees in a given pair; this is useful when pairs have different tiers


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_dex_fees_in_a_pair">dex_fees_in_a_pair</a>(x: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): (u128, u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_is_pair_created"></a>

## Function `is_pair_created`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_is_pair_created">is_pair_created</a>(x: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): bool
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_pair_address"></a>

## Function `pair_address`



<pre><code><b>public</b> <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_pair_address">pair_address</a>(x: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): <b>address</b>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_update_fee_tier"></a>

## Function `update_fee_tier`

Update fee tier in a pair


<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="swap.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_swap_update_fee_tier">update_fee_tier</a>&lt;Tier&gt;(signer_ref: &<a href="">signer</a>, x_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, y_metadata: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;)
</code></pre>
