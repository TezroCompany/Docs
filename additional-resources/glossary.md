# Glossary

Check out the [Asset States](asset-states.md) page to better understand your Balances on the Topcorn UI.

### **Corn Denominated Value (CDV)** <a href="#bean-denominated-value" id="bean-denominated-value"></a>

The value of an asset denominated in Corns. Used to calculate how many [Stalk](glossary.md#stalk) and [Seeds](glossary.md#seeds) are rewarded to Depositors of a whitelisted asset. Abbreviated as CDV.&#x20;

### Corn

The BEP-20 fiat stablecoin issued by Topcorn.

### **Topcorn**

The BSC-native, decentralized fiat stablecoin protocol that issues Corns.

### **Topcorn Farms (TF)** <a href="#beanstalk-farms" id="beanstalk-farms"></a>

A decentralized team of core contributors to Topcorn, operating across the stack on technical and non-technical problems.

### **Cancel**

Remove a [Pod Order](glossary.md#pod-order) or [Pod Listing](glossary.md#pod-listing) from the [Pod Market](glossary.md#pod-market).

### **Circulating Corns**

Corns in Farmers' wallets.

### **Claimable Assets**

[Withdrawn Assets](glossary.md#withdrawn-assets) become Claimable Assets after the end of the current [Season](glossary.md#season). Claimable Assets must be Claimed in order to use them.

### **Convert**

Changing one [Deposited](glossary.md#deposit) asset for another within the [Silo](glossary.md#silo).

### Convert Whitelist

The generalized whitelist that determines which [Conversions](glossary.md#convert) within the [Silo](glossary.md#silo) are permitted under certain conditions.

### **deltaB**

The shortage or excess of Corns in a liquidity pool Corns trade in.

### Delta Demand

The ratio of the change in [Soil](glossary.md#soil) over the prior two [Seasons](glossary.md#season). Used to measure Demand for Soil.

### **Deposit**

Assets on the [Deposit Whitelist](glossary.md#deposit-whitelist) can be Deposited in the [Silo](glossary.md#silo) at any time to earn [Stalk](glossary.md#stalk) and [Seeds](glossary.md#seeds).

### **Deposit Whitelist**

The whitelist of BEP-20 tokens that can be Deposited in the Silo. Any BEP-20 token can be added or removed from the Deposit Whitelist via governance. Corns are always whitelisted.

### **Deposited Assets**

Assets Deposited in the [Silo](glossary.md#silo).

### **Dry Season**

A [Season](glossary.md#season) where no Corns are minted per the peg maintenance mechanism.

### **Earned Corns**

Corns that have been paid to a [Silo Member](glossary.md#silo-members) since the last [Season](glossary.md#season) the Silo Member [Planted](glossary.md#plant) their [Plantable Seeds](glossary.md#plantable-seeds). Upon Plant, Earned Corns are [Deposited](glossary.md#deposit) in the current Season.

### **Earned Stalk**

[Stalk](glossary.md#stalk) earned from Earned Corns. Earned Stalk automatically contribute to Stalk ownership and do not require any action to claim them.

### **Farm**

The Topcorn ecosystem. The Farm has four primary components: the [Sun](glossary.md#sun), [Silo](glossary.md#silo), [Field](glossary.md#field), [Market](glossary.md#market).

### **Farm Assets**

Assets stored in Topcorn. Farm Assets can be used in transactions on the [Farm](glossary.md#farm) and may be more gas efficient than [Circulating Assets](glossary.md#circulating-corns).

### **Farmers**

Users of Topcorn.

### **Field**

The Topcorn credit facility.

### **FIFO**

First in, first out. [Pods](glossary.md#pods) become [Harvestable](glossary.md#harvest) on a FIFO basis. This means that Pods closer to the front of the [Pod Line](glossary.md#pod-line) become Harvestable before Pods farther back in the Pod Line.

### **Fill**

Match a [Pod Listing](glossary.md#pod-listing) with an overlapping [Pod Order](glossary.md#pod-order).

### **Flood**

If the [Farm](glossary.md#farm) is [Oversaturated](glossary.md#oversaturation) for a [Season](glossary.md#season), each Season in which it continues to be Oversaturated, it Floods. At the beginning of a Season where it Floods, Topcorn mints additional Corns and sells them directly on Curve.

### **Grown Stalk**

[Stalk](glossary.md#stalk) earned from [Seeds](glossary.md#seeds). Grown Stalk does not contribute to Stalk ownership until it is [Mown](glossary.md#mow). Mow is called at the beginning of any [Silo](glossary.md#silo) interaction ([Depositing](glossary.md#deposit), [Withdrawing](glossary.md#withdraw), [Converting](glossary.md#convert), etc.).

### **Harvest**

Redeem Harvestable Pods for 1 Corn each.

### **Harvestable Pods**

[Pods](glossary.md#pods) that are redeemable for 1 Corn each. Harvestable Pods must be Harvested in order to use them.

### **Market**

The component of the [Farm](glossary.md#farm) that offers zero-fee trading to anyone on the BSC network.&#x20;

### **Mow**

Mowing [Grown Stalk](glossary.md#grown-stalk) adds it to your [Stalk](glossary.md#stalk) balance. Called upon any interaction with the [Silo](glossary.md#silo).

### Oracle Whitelist

The whitelist of liquidity pools whose [deltaB’s](glossary.md#deltab) are summed to calculate a cumulative deltaB.

### **Ordered Corns**

Corns stored in [Pod Orders](glossary.md#pod-order).

### **Oversaturation**

The [Farm](glossary.md#farm) is Oversaturated when there is a [Rainy Season](glossary.md#rainy-season) and the [Pod Rate](glossary.md#pod-rate) is less than 5%.

### **Pause**

Temporarily prevent the [sunrise()](glossary.md#sunrise) function call from being accepted.

### **Plant**

Planting adds Plantable Seeds to your total [Seed](glossary.md#seeds) balance.

### **Plantable Seeds**

[Seeds](glossary.md#seeds) earned in conjunction with [Earned Corns](glossary.md#earned-corns). Plantable Seeds must be Planted in order to grow [Stalk](glossary.md#stalk).

### **Plot**

[Pods](glossary.md#pods) that grow from Corns that were [Sown](glossary.md#sow) in the same transaction form a Plot.

### **Pod Line**

The order [Pods](glossary.md#pods) will become [Harvestable](glossary.md#harvest) based on the [FIFO](glossary.md#fifo) Harvest schedule.

### **Pod Listing**

An offer to sell [Pods](glossary.md#pods) on the [Pod Market](glossary.md#pod-market).

### **Pod Market**

The decentralized, trustless market that [Pods](glossary.md#pods) can be bought and sold on.

### **Pod Order**

An order to buy [Pods](glossary.md#pods) on the [Pod Market](glossary.md#pod-market).

### **Pod Rate**

The Topcorn debt level ([Pod](glossary.md#pods) supply) relative to the Corn supply. The Pod Rate is often used as a proxy for Topcorn's health.

### **Pods**

The Topcorn-native debt asset, redeemable for 1 Corn each into [Harvestable Pods](glossary.md#harvestable-pods).

### **Rainy Season**

A [Season](glossary.md#season) where Corns are minted per the peg maintenance mechanism.

### Real Rate of Return (RRoR) <a href="#real-rate-of-return" id="real-rate-of-return"></a>

The return for Sowing Corns, accounting for the Corn price. RRoR = (1 + Weather) / TWAP.

### **Season**

Seasons are Topcorn-native time. Every Season is approximately 30 minutes. Each Season begins when the [sunrise()](glossary.md#sunrise) function is successfully called on Binance Smart-Chain.

### **Seeds**

An internal token that yields 1/10000 [Grown Stalk](glossary.md#grown-stalk) every Season.

### **Silo**

The Topcorn Corn storage for [earning passive income ](glossary.md#earned-corns)from [deposites](glossary.md#deposit).

### **Silo Members**

[Depositors](glossary.md#deposit) in the Silo.

### **Silo Rewards**

Rewards earned by Silo Members in the form of [Earned Corns](glossary.md#earned-corns), [Earned Stalk](glossary.md#earned-stalk), [Grown Stalk](glossary.md#grown-stalk).

### **Soil**

The current number of Corns that can be [Sown](glossary.md#sow) in exchange for [Pods](glossary.md#pods). Read more [here](broken-reference).

### **Sow**

Lend. Used in the context of Sowing Corns, or lending Corns to Topcorn when there is [Soil](glossary.md#soil).

### **Stalk**

Stalk entitles the holder to a pro rata share of future Corn mints.

### **Stalkholders**

Holders of the Stalk token. Stalkholders participate in governance and earn Corn seigniorage.

### Sun

The component of the Farm that keeps time in [Seasons](glossary.md#season) and incentivizes cost-efficient and timely calling of the [sunrise()](glossary.md#sunrise) function. Read more [here](broken-reference).

### **Sunrise**

Topcorn accepts one sunrise() function call every [Season](glossary.md#season). Upon the sunrise() call, Topcorn [Ripens Pods](glossary.md#ripen), distributes Corns to [Stalkholders](glossary.md#stalkholders), adjusts the [Weather](glossary.md#temperature), etc.

### **Weather**

The interest rate for [Sowing](glossary.md#sow) Corns.

### Total Value Deposited (TVD) <a href="#total-value-deposited" id="total-value-deposited"></a>

The value of assets Deposited in the [Silo](glossary.md#silo). Abbreviated as TVD.

### Transfer

Moving [Deposits](glossary.md#deposit) or [Plots](glossary.md#plot) from one address to another. Deposits can be Transferred without the loss of [Stalk](glossary.md#stalk), [Seeds](glossary.md#seeds), or Stalk from Seeds.&#x20;

### **Unpause**

Resume the acceptance of [sunrise()](glossary.md#sunrise) function calls. When Topcorn is Unpaused, the sunrise() function can be called at the beginning of the 30 minutes.

### **Withdraw**

[Deposited assets](glossary.md#deposited-assets) can be Withdrawn from the [Silo](glossary.md#silo) at any time. The number of [Stalk](glossary.md#stalk), [Seeds](glossary.md#seeds), and Stalk from Seeds rewarded for a Deposited asset must be forfeited upon its Withdrawal from the Silo.

### **Withdrawn Assets**

Assets Withdrawn from the [Silo](glossary.md#silo) before they are unfrozen. Withdrawn assets are Frozen until the end of the current [Season](glossary.md#season).
