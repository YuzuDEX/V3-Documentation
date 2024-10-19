
<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common"></a>

# Module `0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::common`



-  [Constants](#@Constants_0)
-  [Function `amount_out`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_amount_out)
-  [Function `amount_in`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_amount_in)
-  [Function `quote`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_quote)
-  [Function `calculate_amount`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_calculate_amount)
-  [Function `transfer_in`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_transfer_in)
-  [Function `transfer_out`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_transfer_out)
-  [Function `smaller_enum`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_smaller_enum)
-  [Function `greater_enum`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_greater_enum)
-  [Function `equal_enum`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_equal_enum)
-  [Function `sort_token`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_sort_token)


<pre><code><b>use</b> <a href="">0x1::comparator</a>;
<b>use</b> <a href="">0x1::dispatchable_fungible_asset</a>;
<b>use</b> <a href="">0x1::fungible_asset</a>;
<b>use</b> <a href="">0x1::object</a>;
<b>use</b> <a href="">0x1::primary_fungible_store</a>;
<b>use</b> <a href="">0x1::signer</a>;
<b>use</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::errors</a>;
</code></pre>



<a id="@Constants_0"></a>

## Constants


<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_EQUAL"></a>



<pre><code><b>const</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_EQUAL">EQUAL</a>: u8 = 0;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_GREATER"></a>



<pre><code><b>const</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_GREATER">GREATER</a>: u8 = 2;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_SMALLER"></a>



<pre><code><b>const</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_SMALLER">SMALLER</a>: u8 = 1;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_amount_out"></a>

## Function `amount_out`



<pre><code><b>public</b> <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_amount_out">amount_out</a>(amount_in: u64, reserve_in: u64, reserve_out: u64, total_fees: u128): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_amount_in"></a>

## Function `amount_in`



<pre><code><b>public</b> <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_amount_in">amount_in</a>(amount_out: u64, reserve_in: u64, reserve_out: u64, total_fees: u128): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_quote"></a>

## Function `quote`



<pre><code><b>public</b> <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_quote">quote</a>(amount_x: u64, reserve_x: u64, reserve_y: u64): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_calculate_amount"></a>

## Function `calculate_amount`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_calculate_amount">calculate_amount</a>(numerator: u128, amount_in: u64): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_transfer_in"></a>

## Function `transfer_in`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_transfer_in">transfer_in</a>&lt;CoinType: key&gt;(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;CoinType&gt;, store: <a href="_Object">object::Object</a>&lt;<a href="_FungibleStore">fungible_asset::FungibleStore</a>&gt;, amount: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_transfer_out"></a>

## Function `transfer_out`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_transfer_out">transfer_out</a>&lt;CoinType: key&gt;(sender: &<a href="">signer</a>, metadata: <a href="_Object">object::Object</a>&lt;CoinType&gt;, recipient_store: <a href="_Object">object::Object</a>&lt;<a href="_FungibleStore">fungible_asset::FungibleStore</a>&gt;, amount: u64)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_smaller_enum"></a>

## Function `smaller_enum`



<pre><code><b>public</b> <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_smaller_enum">smaller_enum</a>(): u8
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_greater_enum"></a>

## Function `greater_enum`



<pre><code><b>public</b> <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_greater_enum">greater_enum</a>(): u8
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_equal_enum"></a>

## Function `equal_enum`



<pre><code><b>public</b> <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_equal_enum">equal_enum</a>(): u8
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_sort_token"></a>

## Function `sort_token`



<pre><code><b>public</b> <b>fun</b> <a href="common.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_common_sort_token">sort_token</a>(left: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;, right: <a href="_Object">object::Object</a>&lt;<a href="_Metadata">fungible_asset::Metadata</a>&gt;): bool
</code></pre>
