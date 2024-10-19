
<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors"></a>

# Module `0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::errors`



-  [Constants](#@Constants_0)
-  [Function `only_admin_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_only_admin_address)
-  [Function `already_initialized`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_already_initialized)
-  [Function `not_creator`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_creator)
-  [Function `insufficient_liquidity_minted`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity_minted)
-  [Function `insufficient_amount`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_amount)
-  [Function `insufficient_liquidity`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity)
-  [Function `invalid_amount`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_invalid_amount)
-  [Function `tokens_not_sorted`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_tokens_not_sorted)
-  [Function `insufficient_liquidity_burned`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity_burned)
-  [Function `insufficient_output_amount`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_output_amount)
-  [Function `insufficient_input_amount`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_input_amount)
-  [Function `k`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_k)
-  [Function `x_not_registered`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_x_not_registered)
-  [Function `y_not_registered`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_y_not_registered)
-  [Function `not_admin`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_admin)
-  [Function `not_treasury_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_treasury_address)
-  [Function `not_equal_exact_amount`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_equal_exact_amount)
-  [Function `not_resource_account`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_resource_account)
-  [Function `no_fee_withdraw`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_fee_withdraw)
-  [Function `excessive_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_excessive_fee)
-  [Function `pair_not_created`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pair_not_created)
-  [Function `must_be_inferior_to_twenty`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_must_be_inferior_to_twenty)
-  [Function `pool_not_created`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pool_not_created)
-  [Function `no_stake`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_stake)
-  [Function `insufficient_balance`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_balance)
-  [Function `no_rewards`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_rewards)
-  [Function `not_owner`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_owner)
-  [Function `fee_on_transfer_not_initialized`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_fee_on_transfer_not_initialized)
-  [Function `output_less_than_min`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_output_less_than_min)
-  [Function `input_more_than_max`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_input_more_than_max)
-  [Function `insufficient_x_amount`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_x_amount)
-  [Function `insufficient_y_amount`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_y_amount)
-  [Function `pair_created`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pair_created)
-  [Function `pool_exists`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pool_exists)
-  [Function `max_coin_name_length`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_max_coin_name_length)
-  [Function `coin_type_does_not_match_x_or_y`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_coin_type_does_not_match_x_or_y)
-  [Function `same_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_same_address)
-  [Function `not_liquidity_provider`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_liquidity_provider)
-  [Function `same_token`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_same_token)
-  [Function `internal`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_internal)
-  [Function `pending_request`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pending_request)
-  [Function `invalid_tier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_invalid_tier)
-  [Function `fee_on_transfer_not_registered`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_fee_on_transfer_not_registered)
-  [Function `max_coin_symbol_length`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_max_coin_symbol_length)
-  [Function `icon_uri_needed`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_icon_uri_needed)
-  [Function `project_uri_needed`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_project_uri_needed)
-  [Function `coin_type_resource_does_not_exist`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_coin_type_resource_does_not_exist)
-  [Function `blacklisted`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_blacklisted)
-  [Function `balance_threshold_exceeded`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_balance_threshold_exceeded)
-  [Function `transaction_threshold_exceeded`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_transaction_threshold_exceeded)


<pre><code></code></pre>



<a id="@Constants_0"></a>

## Constants


<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_BALANCE"></a>

Insufficient balance


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_BALANCE">EINSUFFICIENT_BALANCE</a>: u64 = 27;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_MAX_COIN_NAME_LENGTH"></a>

Max coin name length


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_MAX_COIN_NAME_LENGTH">MAX_COIN_NAME_LENGTH</a>: u64 = 32;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_ADMIN"></a>

Not admin


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_ADMIN">ENOT_ADMIN</a>: u64 = 17;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_OWNER"></a>

Not owner


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_OWNER">ENOT_OWNER</a>: u64 = 29;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_COINTYPE_DOES_NOT_MATCH_X_OR_Y"></a>

Coin type does not match X or Y


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_COINTYPE_DOES_NOT_MATCH_X_OR_Y">COINTYPE_DOES_NOT_MATCH_X_OR_Y</a>: u64 = 38;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EALREADY_INITIALIZED"></a>

Already initialized


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EALREADY_INITIALIZED">EALREADY_INITIALIZED</a>: u64 = 1;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EBLACKLISTED_ADDRESS"></a>

The address is blacklisted


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EBLACKLISTED_ADDRESS">EBLACKLISTED_ADDRESS</a>: u64 = 48;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ECOIN_TYPE_RESOURCE_DOES_NOT_EXIST"></a>

Coin type resource does not exist the inputted metadata


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ECOIN_TYPE_RESOURCE_DOES_NOT_EXIST">ECOIN_TYPE_RESOURCE_DOES_NOT_EXIST</a>: u64 = 47;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EEXCESSIVE_BALANCE"></a>

The balance exceeds the balance threshold


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EEXCESSIVE_BALANCE">EEXCESSIVE_BALANCE</a>: u64 = 49;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EEXCESSIVE_FEE"></a>

Excessive fee


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EEXCESSIVE_FEE">EEXCESSIVE_FEE</a>: u64 = 22;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EEXCESSIVE_TRANSACTION"></a>

The transaction exceeds the transaction threshold


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EEXCESSIVE_TRANSACTION">EEXCESSIVE_TRANSACTION</a>: u64 = 50;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EFEE_ON_TRANSFER_NOT_INITIALIZED"></a>

Fee on transfer not initialized


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EFEE_ON_TRANSFER_NOT_INITIALIZED">EFEE_ON_TRANSFER_NOT_INITIALIZED</a>: u64 = 30;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EFEE_ON_TRANSFER_NOT_REGISTERED"></a>

Fee on transfer not registered


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EFEE_ON_TRANSFER_NOT_REGISTERED">EFEE_ON_TRANSFER_NOT_REGISTERED</a>: u64 = 301;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EICON_URI_NOT_INPUTTED"></a>

Icon URI not inputted


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EICON_URI_NOT_INPUTTED">EICON_URI_NOT_INPUTTED</a>: u64 = 45;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINPUT_MORE_THAN_MAX"></a>

Require Input amount is more than max limit


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINPUT_MORE_THAN_MAX">EINPUT_MORE_THAN_MAX</a>: u64 = 44;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_AMOUNT"></a>

Insufficient amount


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_AMOUNT">EINSUFFICIENT_AMOUNT</a>: u64 = 6;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_INPUT_AMOUNT"></a>

Insufficient input amount


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_INPUT_AMOUNT">EINSUFFICIENT_INPUT_AMOUNT</a>: u64 = 14;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_LIQUIDITY"></a>

Insufficient liquidity


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_LIQUIDITY">EINSUFFICIENT_LIQUIDITY</a>: u64 = 7;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_LIQUIDITY_BURNED"></a>

Insufficient liquidity burned


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_LIQUIDITY_BURNED">EINSUFFICIENT_LIQUIDITY_BURNED</a>: u64 = 10;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_LIQUIDITY_MINTED"></a>

Insufficient liquidity minted


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_LIQUIDITY_MINTED">EINSUFFICIENT_LIQUIDITY_MINTED</a>: u64 = 4;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_OUTPUT_AMOUNT"></a>

Insufficient output amount


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_OUTPUT_AMOUNT">EINSUFFICIENT_OUTPUT_AMOUNT</a>: u64 = 13;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_X_AMOUNT"></a>

Insufficient X


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_X_AMOUNT">EINSUFFICIENT_X_AMOUNT</a>: u64 = 33;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_Y_AMOUNT"></a>

Insufficient Y


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINSUFFICIENT_Y_AMOUNT">EINSUFFICIENT_Y_AMOUNT</a>: u64 = 34;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINTERNAL"></a>

Internal error


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINTERNAL">EINTERNAL</a>: u64 = 1000;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINVALID_AMOUNT"></a>

Invalid amount


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINVALID_AMOUNT">EINVALID_AMOUNT</a>: u64 = 8;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINVALID_TIER"></a>

Invalid tier


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EINVALID_TIER">EINVALID_TIER</a>: u64 = 43;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EK"></a>

K constant error


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EK">EK</a>: u64 = 15;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EMAX_COIN_SYMBOL_LENGTH"></a>

Max coin symbol length


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EMAX_COIN_SYMBOL_LENGTH">EMAX_COIN_SYMBOL_LENGTH</a>: u64 = 10;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EMUST_BE_INFERIOR_TO_TWENTY"></a>

Must be inferior to twenty


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EMUST_BE_INFERIOR_TO_TWENTY">EMUST_BE_INFERIOR_TO_TWENTY</a>: u64 = 24;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_CREATOR"></a>

Not creator


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_CREATOR">ENOT_CREATOR</a>: u64 = 2;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_EQUAL_EXACT_AMOUNT"></a>

Not equal exact amount


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_EQUAL_EXACT_AMOUNT">ENOT_EQUAL_EXACT_AMOUNT</a>: u64 = 19;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_RESOURCE_ACCOUNT"></a>

Not resource account


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_RESOURCE_ACCOUNT">ENOT_RESOURCE_ACCOUNT</a>: u64 = 20;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_TREASURY_ADDRESS"></a>

Not treasury address


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENOT_TREASURY_ADDRESS">ENOT_TREASURY_ADDRESS</a>: u64 = 18;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENO_FEE_WITHDRAW"></a>

No fee withdraw


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENO_FEE_WITHDRAW">ENO_FEE_WITHDRAW</a>: u64 = 21;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENO_REWARDS"></a>

No rewards


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENO_REWARDS">ENO_REWARDS</a>: u64 = 28;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENO_STAKE"></a>

No stake


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ENO_STAKE">ENO_STAKE</a>: u64 = 26;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EONLY_ADMIN"></a>

Only admin can call this function


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EONLY_ADMIN">EONLY_ADMIN</a>: u64 = 0;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EOUTPUT_LESS_THAN_MIN"></a>

Output amount is less than required


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EOUTPUT_LESS_THAN_MIN">EOUTPUT_LESS_THAN_MIN</a>: u64 = 31;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPAIR_CREATED"></a>

Pair is created


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPAIR_CREATED">EPAIR_CREATED</a>: u64 = 35;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPAIR_NOT_CREATED"></a>

Pair not created


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPAIR_NOT_CREATED">EPAIR_NOT_CREATED</a>: u64 = 23;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPENDING_REQUEST"></a>

Pending request


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPENDING_REQUEST">EPENDING_REQUEST</a>: u64 = 42;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPOOL_EXISTS"></a>

Pool already created


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPOOL_EXISTS">EPOOL_EXISTS</a>: u64 = 36;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPOOL_NOT_CREATED"></a>

Pool not created


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPOOL_NOT_CREATED">EPOOL_NOT_CREATED</a>: u64 = 25;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPROJECT_URI_NOT_INPUTTED"></a>

Project URI not inputted


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EPROJECT_URI_NOT_INPUTTED">EPROJECT_URI_NOT_INPUTTED</a>: u64 = 46;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ESAME_ADDRESS"></a>

Same address


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ESAME_ADDRESS">ESAME_ADDRESS</a>: u64 = 39;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ESAME_TOKEN"></a>

Same token


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ESAME_TOKEN">ESAME_TOKEN</a>: u64 = 41;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ETOKENS_NOT_SORTED"></a>

Tokens not sorted


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_ETOKENS_NOT_SORTED">ETOKENS_NOT_SORTED</a>: u64 = 9;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EX_NOT_REGISTERED"></a>

X not registered


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EX_NOT_REGISTERED">EX_NOT_REGISTERED</a>: u64 = 16;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EY_NOT_REGISTERED"></a>

Y not registered


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_EY_NOT_REGISTERED">EY_NOT_REGISTERED</a>: u64 = 16;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_NOT_LIQUIDITY_PROVIDER"></a>

Not liquidity provider


<pre><code><b>const</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_NOT_LIQUIDITY_PROVIDER">NOT_LIQUIDITY_PROVIDER</a>: u64 = 40;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_only_admin_address"></a>

## Function `only_admin_address`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_only_admin_address">only_admin_address</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_already_initialized"></a>

## Function `already_initialized`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_already_initialized">already_initialized</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_creator"></a>

## Function `not_creator`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_creator">not_creator</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity_minted"></a>

## Function `insufficient_liquidity_minted`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity_minted">insufficient_liquidity_minted</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_amount"></a>

## Function `insufficient_amount`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_amount">insufficient_amount</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity"></a>

## Function `insufficient_liquidity`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity">insufficient_liquidity</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_invalid_amount"></a>

## Function `invalid_amount`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_invalid_amount">invalid_amount</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_tokens_not_sorted"></a>

## Function `tokens_not_sorted`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_tokens_not_sorted">tokens_not_sorted</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity_burned"></a>

## Function `insufficient_liquidity_burned`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_liquidity_burned">insufficient_liquidity_burned</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_output_amount"></a>

## Function `insufficient_output_amount`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_output_amount">insufficient_output_amount</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_input_amount"></a>

## Function `insufficient_input_amount`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_input_amount">insufficient_input_amount</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_k"></a>

## Function `k`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_k">k</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_x_not_registered"></a>

## Function `x_not_registered`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_x_not_registered">x_not_registered</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_y_not_registered"></a>

## Function `y_not_registered`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_y_not_registered">y_not_registered</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_admin"></a>

## Function `not_admin`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_admin">not_admin</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_treasury_address"></a>

## Function `not_treasury_address`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_treasury_address">not_treasury_address</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_equal_exact_amount"></a>

## Function `not_equal_exact_amount`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_equal_exact_amount">not_equal_exact_amount</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_resource_account"></a>

## Function `not_resource_account`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_resource_account">not_resource_account</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_fee_withdraw"></a>

## Function `no_fee_withdraw`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_fee_withdraw">no_fee_withdraw</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_excessive_fee"></a>

## Function `excessive_fee`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_excessive_fee">excessive_fee</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pair_not_created"></a>

## Function `pair_not_created`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pair_not_created">pair_not_created</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_must_be_inferior_to_twenty"></a>

## Function `must_be_inferior_to_twenty`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_must_be_inferior_to_twenty">must_be_inferior_to_twenty</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pool_not_created"></a>

## Function `pool_not_created`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pool_not_created">pool_not_created</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_stake"></a>

## Function `no_stake`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_stake">no_stake</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_balance"></a>

## Function `insufficient_balance`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_balance">insufficient_balance</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_rewards"></a>

## Function `no_rewards`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_no_rewards">no_rewards</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_owner"></a>

## Function `not_owner`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_owner">not_owner</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_fee_on_transfer_not_initialized"></a>

## Function `fee_on_transfer_not_initialized`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_fee_on_transfer_not_initialized">fee_on_transfer_not_initialized</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_output_less_than_min"></a>

## Function `output_less_than_min`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_output_less_than_min">output_less_than_min</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_input_more_than_max"></a>

## Function `input_more_than_max`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_input_more_than_max">input_more_than_max</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_x_amount"></a>

## Function `insufficient_x_amount`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_x_amount">insufficient_x_amount</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_y_amount"></a>

## Function `insufficient_y_amount`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_insufficient_y_amount">insufficient_y_amount</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pair_created"></a>

## Function `pair_created`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pair_created">pair_created</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pool_exists"></a>

## Function `pool_exists`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pool_exists">pool_exists</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_max_coin_name_length"></a>

## Function `max_coin_name_length`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_max_coin_name_length">max_coin_name_length</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_coin_type_does_not_match_x_or_y"></a>

## Function `coin_type_does_not_match_x_or_y`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_coin_type_does_not_match_x_or_y">coin_type_does_not_match_x_or_y</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_same_address"></a>

## Function `same_address`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_same_address">same_address</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_liquidity_provider"></a>

## Function `not_liquidity_provider`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_not_liquidity_provider">not_liquidity_provider</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_same_token"></a>

## Function `same_token`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_same_token">same_token</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_internal"></a>

## Function `internal`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <b>internal</b>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pending_request"></a>

## Function `pending_request`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_pending_request">pending_request</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_invalid_tier"></a>

## Function `invalid_tier`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_invalid_tier">invalid_tier</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_fee_on_transfer_not_registered"></a>

## Function `fee_on_transfer_not_registered`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_fee_on_transfer_not_registered">fee_on_transfer_not_registered</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_max_coin_symbol_length"></a>

## Function `max_coin_symbol_length`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_max_coin_symbol_length">max_coin_symbol_length</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_icon_uri_needed"></a>

## Function `icon_uri_needed`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_icon_uri_needed">icon_uri_needed</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_project_uri_needed"></a>

## Function `project_uri_needed`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_project_uri_needed">project_uri_needed</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_coin_type_resource_does_not_exist"></a>

## Function `coin_type_resource_does_not_exist`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_coin_type_resource_does_not_exist">coin_type_resource_does_not_exist</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_blacklisted"></a>

## Function `blacklisted`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_blacklisted">blacklisted</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_balance_threshold_exceeded"></a>

## Function `balance_threshold_exceeded`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_balance_threshold_exceeded">balance_threshold_exceeded</a>(): u64
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_transaction_threshold_exceeded"></a>

## Function `transaction_threshold_exceeded`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors_transaction_threshold_exceeded">transaction_threshold_exceeded</a>(): u64
</code></pre>
