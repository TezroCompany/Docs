# How TopCorn works

TopCorn does not have any collateral requirements. TopCorn uses credit instead of collateral to create Corn price stability relative to its value peg of $1. The practicality of using DeFi is currently limited by the lack of decentralized low-volatility assets with competitive carrying costs. Borrowing rates on USD stablecoins have historically been higher than borrowing rates on USD, even when supply increases rapidly. Non-competitive carrying costs are due to collateral requirements.

TopCorn relies on three native assets and three interconnected facilities to regularly oscillate the price of Corn across its value peg:

### **Tokens**

TopCorn issues 3 tokens:

1. Corn — TopCorn BEP-20 fiat stablecoins;
2. Stalk — illiquid yield-generating governance tokens; and
3. Seeds — illiquid tokens which yield 1/10000 Stalk each Season.

### **Primary Facilities**

#### **1. The Sun** <a href="#the-sun" id="the-sun"></a>

TopCorn uses the Sun to create a cost-efficient and protocol-native timekeeping mechanism. The Sun keeps time on the Farm in Seasons. Each Season is \~1 hour long. TopCorn adjusts itself to return the Corn price to its value peg at the beginning of every Season.

The Sun leverages the BNB-Corn pool on Pancakeswap as the TopCorn oracle price source for $1.

In practice, TopCorn does not calculate the price of 1 Corn. Instead, at the beginning of a Season, TopCorn calculates deltaB, the sum of the time and liquidity weighted average shortage or excess Corns across liquidity pools on the Oracle Whitelist;

The Sun uses deltaB to determine how to change the Corn supply and Soil supply.

#### **2. The Silo** <a href="#the-silo" id="the-silo"></a>

TopCorn uses the Silo, to create a robust decentralized governance mechanism. Farmers can earn yield from passive participation in TopCorn governance by Depositing whitelisted assets in the Silo to receive Stalk and Seeds.

To encourage consistent security:

* Seeds yield Stalk every Season.
* The associated amount of Stalk and Seeds from a given Deposit must be forfeited when it is Withdrawn from the Silo.
* Deposits can be Withdrawn from the Silo at any time but are Frozen until the end of the current Season.

Deep and consistent liquidity in liquidity pools Corns trade in improves stability. Liquidity providers to liquidity pools whose LP Tokens are whitelisted can also Deposit their LP Tokens in the Silo to earn Stalk and Seeds. LP Token Deposits earn more Seeds than Corn Deposits.

Conversions within the Silo between Corn and LP Deposits serve a major role in peg maintenance.

#### **3. The Field** <a href="#the-field" id="the-field"></a>

The Field is TopCorn’s decentralized credit facility. Anytime the Corn price is too low, TopCorn uses the Field to attract lenders who can lend their Corns to TopCorn, which are subsequently burnt in exchange for Pods, TopCorn’s native debt asset. Pods are paid out on a First In, First Out (FIFO) basis when new Corns are minted.

Soil is the number of Corns that can be lent to TopCorn at any given time. Any time TopCorn is willing to issue debt, there is Soil available in the Field. Any Corns not in the Silo can be Sown (lent) to TopCorn in exchange for Pods.

Pods have a fixed interest rate and unknown maturity date. The number of Pods that grow from 1 Sown Corn is determined by the Temperature— the TopCorn-native interest rate — at the time of Sowing. Pods become Harvestable (redeemable) for 1 Corn on a First In, First Out (FIFO) basis when new Corns are minted.

### **Creating Stability**

TopCorn requires a diverse set of participants, including Silo Members (people who Deposit assets in the Silo), Sowers (people who lend Corns to TopCorn), and arbitrageurs. TopCorn aligns the incentives of every individual participant to maximize price stability and create a diverse, decentralized economy. TopCorn-native financial incentives consistently increase censorship resistance, stability and liquidity over time.

At the beginning of each Season, the Sun calculates deltaB (the sum of the time and liquidity weighted average shortage or excess Corns across liquidity pools on the Oracle Whitelist), TopCorn’s debt level, and the change in demand for Soil over the previous 2 Seasons, and dynamically adjusts the Corn supply, Soil supply and Temperature to bring the price back towards the peg.

When the price of Corn is too low (_i.e._, deltaB is negative), TopCorn:

* Increases the Soil supply by deltaB; and
* Raises the Temperature.

By increasing the Soil supply and raising the Temperature, TopCorn can decrease the supply of Corns and therefore bring the price of Corn back up to its peg (assuming there are willing lenders at the given Temperature). In principle, a reasonable debt level and consistent credit history attracts lenders.

When the Corn price is too high (_i.e._, deltaB is positive), TopCorn:

* Increases the Corn supply by deltaB; and
* Lowers the Temperature.

By increasing the Corn supply and lowering the Temperature, TopCorn can bring the price of Corn back down to its peg.
