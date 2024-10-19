
<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin"></a>

# Module `0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::admin`



-  [Resource `LPRegistry`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_LPRegistry)
-  [Resource `Pair`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pair)
-  [Resource `FeeOnTransferRegistry`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_FeeOnTransferRegistry)
-  [Resource `RewardsPoolRegistry`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_RewardsPoolRegistry)
-  [Resource `AdminInfo`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_AdminInfo)
-  [Resource `Universal`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Universal)
-  [Resource `PopularTraded`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_PopularTraded)
-  [Resource `Stable`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Stable)
-  [Resource `VeryStable`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_VeryStable)
-  [Resource `Pending`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pending)
-  [Struct `Admin`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Admin)
-  [Struct `Treasury`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Treasury)
-  [Struct `OwnershipTransferRequestEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferRequestEvent)
-  [Struct `OwnershipTransferCanceledEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferCanceledEvent)
-  [Struct `TreasuryAddressUpdatedEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_TreasuryAddressUpdatedEvent)
-  [Struct `AdminUpdatedEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_AdminUpdatedEvent)
-  [Struct `DexLiquidityFeeUpdatedEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_DexLiquidityFeeUpdatedEvent)
-  [Struct `DexTreasuryFeeUpdatedEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_DexTreasuryFeeUpdatedEvent)
-  [Struct `OwnershipTransferRejectedEvent`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferRejectedEvent)
-  [Function `offer_admin_previliges`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_offer_admin_previliges)
-  [Function `offer_treasury_previliges`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_offer_treasury_previliges)
-  [Function `cancel_admin_previliges_offer`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_cancel_admin_previliges_offer)
-  [Function `cancel_treasury_previliges_offer`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_cancel_treasury_previliges_offer)
-  [Function `claim_admin_previliges`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_claim_admin_previliges)
-  [Function `claim_treasury_previliges`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_claim_treasury_previliges)
-  [Function `reject_admin_previliges`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_reject_admin_previliges)
-  [Function `reject_treasury_previliges`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_reject_treasury_previliges)
-  [Function `register_lp`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_lp)
-  [Function `register_fee_on_transfer`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_fee_on_transfer)
-  [Function `register_rewards_pool`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_rewards_pool)
-  [Function `set_dex_liquidity_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_set_dex_liquidity_fee)
-  [Function `set_dex_treasury_fee`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_set_dex_treasury_fee)
-  [Function `resource_signer`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_resource_signer)
-  [Function `treasury_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_treasury_address)
-  [Function `admin_address`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_admin_address)
-  [Function `liquidity_fee_modifier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_liquidity_fee_modifier)
-  [Function `treasury_fee_modifier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_treasury_fee_modifier)
-  [Function `dex_fees`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_dex_fees)
-  [Function `universal_liquidity_fee_modifier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_universal_liquidity_fee_modifier)
-  [Function `popular_traded_liquidity_fee_modifier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_popular_traded_liquidity_fee_modifier)
-  [Function `stable_liquidity_fee_modifier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_stable_liquidity_fee_modifier)
-  [Function `very_stable_liquidity_fee_modifier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_very_stable_liquidity_fee_modifier)
-  [Function `universal_tier_fees`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_universal_tier_fees)
-  [Function `popular_traded_tier_fees`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_popular_traded_tier_fees)
-  [Function `stable_tier_fees`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_stable_tier_fees)
-  [Function `very_stable_tier_fees`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_very_stable_tier_fees)
-  [Function `is_valid_tier`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_valid_tier)
-  [Function `is_pair_created`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_pair_created)
-  [Function `is_rewards_pool_created`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_rewards_pool_created)
-  [Function `fee_on_transfer_exists`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_exists)
-  [Function `fee_on_transfer_obj_addr`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_obj_addr)
-  [Function `fee_on_transfer_registry`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_registry)
-  [Function `rewards_pool_registry`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_rewards_pool_registry)
-  [Function `lp_registry`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_lp_registry)
-  [Function `pair_list`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_pair_list)
-  [Function `rewards_pool_pair_list`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_rewards_pool_pair_list)
-  [Function `lp_list`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_lp_list)
-  [Function `does_not_exceed_dex_fee_threshold`](#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_does_not_exceed_dex_fee_threshold)


<pre><code><b>use</b> <a href="">0x1::account</a>;
<b>use</b> <a href="">0x1::event</a>;
<b>use</b> <a href="">0x1::option</a>;
<b>use</b> <a href="">0x1::resource_account</a>;
<b>use</b> <a href="">0x1::signer</a>;
<b>use</b> <a href="">0x1::simple_map</a>;
<b>use</b> <a href="">0x1::smart_table</a>;
<b>use</b> <a href="">0x1::type_info</a>;
<b>use</b> <a href="constants.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_constants">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::constants</a>;
<b>use</b> <a href="errors.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_errors">0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0::errors</a>;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_LPRegistry"></a>

## Resource `LPRegistry`

Global storage for LP registry


<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_LPRegistry">LPRegistry</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pair"></a>

## Resource `Pair`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pair">Pair</a> <b>has</b> <b>copy</b>, drop, store, key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_FeeOnTransferRegistry"></a>

## Resource `FeeOnTransferRegistry`

Global storage for the tokens that have fee on transfer


<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_FeeOnTransferRegistry">FeeOnTransferRegistry</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_RewardsPoolRegistry"></a>

## Resource `RewardsPoolRegistry`

Global storage for Rewards pool


<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_RewardsPoolRegistry">RewardsPoolRegistry</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_AdminInfo"></a>

## Resource `AdminInfo`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_AdminInfo">AdminInfo</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Universal"></a>

## Resource `Universal`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Universal">Universal</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_PopularTraded"></a>

## Resource `PopularTraded`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_PopularTraded">PopularTraded</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Stable"></a>

## Resource `Stable`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Stable">Stable</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_VeryStable"></a>

## Resource `VeryStable`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_VeryStable">VeryStable</a> <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pending"></a>

## Resource `Pending`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pending">Pending</a>&lt;T&gt; <b>has</b> key
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Admin"></a>

## Struct `Admin`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Admin">Admin</a> <b>has</b> <b>copy</b>, drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Treasury"></a>

## Struct `Treasury`



<pre><code><b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Treasury">Treasury</a> <b>has</b> <b>copy</b>, drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferRequestEvent"></a>

## Struct `OwnershipTransferRequestEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferRequestEvent">OwnershipTransferRequestEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferCanceledEvent"></a>

## Struct `OwnershipTransferCanceledEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferCanceledEvent">OwnershipTransferCanceledEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_TreasuryAddressUpdatedEvent"></a>

## Struct `TreasuryAddressUpdatedEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_TreasuryAddressUpdatedEvent">TreasuryAddressUpdatedEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_AdminUpdatedEvent"></a>

## Struct `AdminUpdatedEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_AdminUpdatedEvent">AdminUpdatedEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_DexLiquidityFeeUpdatedEvent"></a>

## Struct `DexLiquidityFeeUpdatedEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_DexLiquidityFeeUpdatedEvent">DexLiquidityFeeUpdatedEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_DexTreasuryFeeUpdatedEvent"></a>

## Struct `DexTreasuryFeeUpdatedEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_DexTreasuryFeeUpdatedEvent">DexTreasuryFeeUpdatedEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferRejectedEvent"></a>

## Struct `OwnershipTransferRejectedEvent`



<pre><code>#[<a href="">event</a>]
<b>struct</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_OwnershipTransferRejectedEvent">OwnershipTransferRejectedEvent</a> <b>has</b> drop, store
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_offer_admin_previliges"></a>

## Function `offer_admin_previliges`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_offer_admin_previliges">offer_admin_previliges</a>(signer_ref: &<a href="">signer</a>, receiver_addr: <b>address</b>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_offer_treasury_previliges"></a>

## Function `offer_treasury_previliges`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_offer_treasury_previliges">offer_treasury_previliges</a>(signer_ref: &<a href="">signer</a>, receiver_addr: <b>address</b>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_cancel_admin_previliges_offer"></a>

## Function `cancel_admin_previliges_offer`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_cancel_admin_previliges_offer">cancel_admin_previliges_offer</a>(signer_ref: &<a href="">signer</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_cancel_treasury_previliges_offer"></a>

## Function `cancel_treasury_previliges_offer`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_cancel_treasury_previliges_offer">cancel_treasury_previliges_offer</a>(signer_ref: &<a href="">signer</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_claim_admin_previliges"></a>

## Function `claim_admin_previliges`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_claim_admin_previliges">claim_admin_previliges</a>(signer_ref: &<a href="">signer</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_claim_treasury_previliges"></a>

## Function `claim_treasury_previliges`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_claim_treasury_previliges">claim_treasury_previliges</a>(signer_ref: &<a href="">signer</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_reject_admin_previliges"></a>

## Function `reject_admin_previliges`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_reject_admin_previliges">reject_admin_previliges</a>(signer_ref: &<a href="">signer</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_reject_treasury_previliges"></a>

## Function `reject_treasury_previliges`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_reject_treasury_previliges">reject_treasury_previliges</a>(signer_ref: &<a href="">signer</a>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_lp"></a>

## Function `register_lp`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_lp">register_lp</a>(lp_addr: <b>address</b>, x: <b>address</b>, y: <b>address</b>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_fee_on_transfer"></a>

## Function `register_fee_on_transfer`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_fee_on_transfer">register_fee_on_transfer</a>(token_addr: <b>address</b>, fee_on_transfer_obj_addr: <b>address</b>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_rewards_pool"></a>

## Function `register_rewards_pool`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_register_rewards_pool">register_rewards_pool</a>(pool: <b>address</b>, x: <b>address</b>, y: <b>address</b>)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_set_dex_liquidity_fee"></a>

## Function `set_dex_liquidity_fee`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_set_dex_liquidity_fee">set_dex_liquidity_fee</a>(sender: &<a href="">signer</a>, new_fee: u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_set_dex_treasury_fee"></a>

## Function `set_dex_treasury_fee`



<pre><code><b>public</b> entry <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_set_dex_treasury_fee">set_dex_treasury_fee</a>(sender: &<a href="">signer</a>, new_fee: u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_resource_signer"></a>

## Function `resource_signer`



<pre><code><b>public</b>(<b>friend</b>) <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_resource_signer">resource_signer</a>(): <a href="">signer</a>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_treasury_address"></a>

## Function `treasury_address`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_treasury_address">treasury_address</a>(): <b>address</b>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_admin_address"></a>

## Function `admin_address`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_admin_address">admin_address</a>(): <b>address</b>
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_liquidity_fee_modifier"></a>

## Function `liquidity_fee_modifier`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_liquidity_fee_modifier">liquidity_fee_modifier</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_treasury_fee_modifier"></a>

## Function `treasury_fee_modifier`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_treasury_fee_modifier">treasury_fee_modifier</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_dex_fees"></a>

## Function `dex_fees`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_dex_fees">dex_fees</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_universal_liquidity_fee_modifier"></a>

## Function `universal_liquidity_fee_modifier`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_universal_liquidity_fee_modifier">universal_liquidity_fee_modifier</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_popular_traded_liquidity_fee_modifier"></a>

## Function `popular_traded_liquidity_fee_modifier`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_popular_traded_liquidity_fee_modifier">popular_traded_liquidity_fee_modifier</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_stable_liquidity_fee_modifier"></a>

## Function `stable_liquidity_fee_modifier`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_stable_liquidity_fee_modifier">stable_liquidity_fee_modifier</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_very_stable_liquidity_fee_modifier"></a>

## Function `very_stable_liquidity_fee_modifier`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_very_stable_liquidity_fee_modifier">very_stable_liquidity_fee_modifier</a>(): u128
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_universal_tier_fees"></a>

## Function `universal_tier_fees`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_universal_tier_fees">universal_tier_fees</a>(): (u128, u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_popular_traded_tier_fees"></a>

## Function `popular_traded_tier_fees`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_popular_traded_tier_fees">popular_traded_tier_fees</a>(): (u128, u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_stable_tier_fees"></a>

## Function `stable_tier_fees`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_stable_tier_fees">stable_tier_fees</a>(): (u128, u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_very_stable_tier_fees"></a>

## Function `very_stable_tier_fees`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_very_stable_tier_fees">very_stable_tier_fees</a>(): (u128, u128)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_valid_tier"></a>

## Function `is_valid_tier`



<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_valid_tier">is_valid_tier</a>&lt;Tier&gt;(): bool
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_pair_created"></a>

## Function `is_pair_created`

Checks if a given address is an LP address


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_pair_created">is_pair_created</a>(x: <b>address</b>, y: <b>address</b>): (bool, <a href="_Option">option::Option</a>&lt;<b>address</b>&gt;)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_rewards_pool_created"></a>

## Function `is_rewards_pool_created`

Is rewards pool created


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_is_rewards_pool_created">is_rewards_pool_created</a>(x: <b>address</b>, y: <b>address</b>): (bool, <a href="_Option">option::Option</a>&lt;<b>address</b>&gt;)
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_exists"></a>

## Function `fee_on_transfer_exists`

Returns if fee on transfer exists for a given token address


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_exists">fee_on_transfer_exists</a>(metadata: <b>address</b>): bool
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_obj_addr"></a>

## Function `fee_on_transfer_obj_addr`

Returns the fee on transfer object address for a given token address


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_obj_addr">fee_on_transfer_obj_addr</a>(metadata: <b>address</b>): <a href="_Option">option::Option</a>&lt;<b>address</b>&gt;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_registry"></a>

## Function `fee_on_transfer_registry`

Returns all the tokens registered with fee on transfer


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_fee_on_transfer_registry">fee_on_transfer_registry</a>(): <a href="_SimpleMap">simple_map::SimpleMap</a>&lt;<b>address</b>, <b>address</b>&gt;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_rewards_pool_registry"></a>

## Function `rewards_pool_registry`

Returns the rewards pool registry


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_rewards_pool_registry">rewards_pool_registry</a>(): <a href="_SimpleMap">simple_map::SimpleMap</a>&lt;<a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pair">admin::Pair</a>, <b>address</b>&gt;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_lp_registry"></a>

## Function `lp_registry`

Returns the LP registry


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_lp_registry">lp_registry</a>(): <a href="_SimpleMap">simple_map::SimpleMap</a>&lt;<a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pair">admin::Pair</a>, <b>address</b>&gt;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_pair_list"></a>

## Function `pair_list`

Returns a list of pair addresses


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_pair_list">pair_list</a>(): <a href="">vector</a>&lt;<a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_Pair">admin::Pair</a>&gt;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_rewards_pool_pair_list"></a>

## Function `rewards_pool_pair_list`

Returns a list of rewards pool addresses


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_rewards_pool_pair_list">rewards_pool_pair_list</a>(): <a href="">vector</a>&lt;<b>address</b>&gt;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_lp_list"></a>

## Function `lp_list`

Returns a list of LP addresses


<pre><code>#[view]
<b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_lp_list">lp_list</a>(): <a href="">vector</a>&lt;<b>address</b>&gt;
</code></pre>



<a id="0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_does_not_exceed_dex_fee_threshold"></a>

## Function `does_not_exceed_dex_fee_threshold`

returns true if given rate is less than dex fee threshold


<pre><code><b>public</b> <b>fun</b> <a href="admin.md#0x2c1ef73c34fbe77663773bd450e0fe910a67492779957ced9cfad955b7d229e0_admin_does_not_exceed_dex_fee_threshold">does_not_exceed_dex_fee_threshold</a>(total_fees_numerator: u128): bool
</code></pre>
