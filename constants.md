
<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants"></a>

# Module `0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::constants`



-  [Constants](#@Constants_0)
-  [Function `seed`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_seed)
-  [Function `code_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_code_address)
-  [Function `dev_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_dev_address)
-  [Function `fee_threshold_numerator`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_fee_threshold_numerator)
-  [Function `minimum_liquidity`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_minimum_liquidity)
-  [Function `max_coin_name_length`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_max_coin_name_length)
-  [Function `precision`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_precision)
-  [Function `max_u128`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_max_u128)
-  [Function `fee_on_transfer_threshold_numerator`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_fee_on_transfer_threshold_numerator)


<pre><code></code></pre>



<a id="@Constants_0"></a>

## Constants


<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_MAX_U128"></a>

Max u128: 2^128 - 1


<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_MAX_U128">MAX_U128</a>: u128 = 340282366920938463463374607431768211455;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_MAX_COIN_NAME_LENGTH"></a>

Max coin name length: 32


<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_MAX_COIN_NAME_LENGTH">MAX_COIN_NAME_LENGTH</a>: u64 = 32;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_DEV"></a>



<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_DEV">DEV</a>: <b>address</b> = 0x46e7aa46f70e2e38642bf0c7c21da06f165001252bd85fabdc070b0c0a3c3597;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_DEX_FEE_THRESHOLD_NUMERATOR"></a>

Max DEX fee: 0.9%; (90 / (100*100))


<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_DEX_FEE_THRESHOLD_NUMERATOR">DEX_FEE_THRESHOLD_NUMERATOR</a>: u128 = 90;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_FEE_ON_TRANSFER_THRESHOLD_NUMERATOR"></a>

Max individual token fee: 15%; (1500 / (100*100))


<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_FEE_ON_TRANSFER_THRESHOLD_NUMERATOR">FEE_ON_TRANSFER_THRESHOLD_NUMERATOR</a>: u128 = 1500;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_MINIMUM_LIQUIDITY"></a>

Minimum liquidity: 1000


<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_MINIMUM_LIQUIDITY">MINIMUM_LIQUIDITY</a>: u128 = 1000;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_PRECISION"></a>

Precision: 10000


<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_PRECISION">PRECISION</a>: u64 = 10000;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_RESOURCE_ACCOUNT"></a>



<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_RESOURCE_ACCOUNT">RESOURCE_ACCOUNT</a>: <b>address</b> = 0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_SEED"></a>

Seed; used to name lp tokens


<pre><code><b>const</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_SEED">SEED</a>: u64 = 0;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_seed"></a>

## Function `seed`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_seed">seed</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_code_address"></a>

## Function `code_address`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_code_address">code_address</a>(): <b>address</b>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_dev_address"></a>

## Function `dev_address`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_dev_address">dev_address</a>(): <b>address</b>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_fee_threshold_numerator"></a>

## Function `fee_threshold_numerator`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_fee_threshold_numerator">fee_threshold_numerator</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_minimum_liquidity"></a>

## Function `minimum_liquidity`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_minimum_liquidity">minimum_liquidity</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_max_coin_name_length"></a>

## Function `max_coin_name_length`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_max_coin_name_length">max_coin_name_length</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_precision"></a>

## Function `precision`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_precision">precision</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_max_u128"></a>

## Function `max_u128`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_max_u128">max_u128</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_fee_on_transfer_threshold_numerator"></a>

## Function `fee_on_transfer_threshold_numerator`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants_fee_on_transfer_threshold_numerator">fee_on_transfer_threshold_numerator</a>(): u128
</code></pre>
