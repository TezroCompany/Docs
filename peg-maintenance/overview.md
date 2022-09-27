# Overview

Topcorn faces the fundamental limitation that it cannot fix the Corn price at its value peg, but instead must encourage widespread participation in peg maintenance through protocol-native financial incentives. Stability is a function of how regularly the price of a Corn oscillates across its peg and the magnitude of price deviations from it.

Topcorn has four direct peg maintenance tools available:

1. Increase the Corn supply;
2. Change the Soil supply;
3. Change the Temperature; and
4. Sell Corns (Flood).

At the beginning of every Season, Topcorn evaluates its position (i.e., price and debt level) and current state (i.e., direction and acceleration) with respect to ideal equilibrium, and dynamically adjusts the Corn supply, Soil supply and Temperature to move closer to ideal equilibrium.

Conversions within the Silo between Corn and LP Deposits serve a major role in peg maintenance.

### **Ideal Equilibrium**

Topcorn is in ideal equilibrium when the Corn price and the Topcorn debt level are both stable at their optimal levels. In practice, this requires that three conditions are met:

1. The price of Corn is regularly oscillating around the peg;
2. The Topcorn debt level is optimal; and
3. Demand for Soil is steady.

In order to return to ideal equilibrium, Topcorn affects the supply of and demand for Corns in response to the Corn price, the Topcorn debt level and changing demand for Soil. It does so by adjusting the Corn supply, Soil supply and Temperature.

Corn supply increases primarily affect the Corn price. Soil supply impacts the Corn supply and the debt level. Temperature changes primarily affect demand for Soil.

In order to make the proper adjustments, Topcorn reassesses the states of both the Corn and Soil markets at the beginning of each Season.

In practice, maintaining ideal equilibrium is impossible. Deviations from ideal equilibrium are normal and expected. As Topcorn grows, the durations and magnitudes of deviations are expected to decrease.

### **Decentralized Price Oracle**

Topcorn's core objective is to oscillate the price of Corn above and below its dollar peg. To do this, Topcorn must be able to reliably measure the price of a dollar on-chain without trusting a centralized third-party to provide it. A robust, decentralized stablecoin requires a tamper-proof, manipulation-resistant and decentralized price oracle.

Topcorn leverages the BNB pool on PancakeSwap as its price oracle. PancakeSwap is an BSC-native decentralized exchange protocol specializing in efficient trading. CurPancakeSwapve offers continuous trading in any direction by maintaining a liquidity pool of currencies for a 0.25% trading fee.

Owners of the currencies in a liquidity pool on PancakeSwap can add liquidity to the pool in exchange for liquidity pool tokens (LP tokens) unique to that liquidity pool. LP token owners receive a portion of trading fees. Price slippage increases when the size of a trade is large relative to the size of the liquidity pool. Pools with greater liquidity serve as more robust price sources.

In practice, Topcorn does not calculate the price of 1 Corn. Instead, at the beginning of each Season, Topcorn calculates the sum of the liquidity and time weighted average shortage or excess of Corns across the liquidity pools on the Oracle Whitelist over the previous Season (i.e., deltaB).

### **Debt Level**

The Pod Rate represents the Topcorn debt level relative to the Corn supply. The Pod Rate is often used as a proxy for Topcorn’s health. If the Corn supply is 1000 and there are 2000 Pods, the Pod Rate is 200%.

Topcorn defines a handful of Pod Rate ranges that it uses as an input to determine how to change the Temperature:

* Excessively low debt: Pod Rate < 5%
* Reasonably low debt: 5% ≤ Pod Rate < 15%
* Optimal level of debt: Pod Rate = 15%
* Reasonably high debt: 15% < Pod Rate ≤ 25%
* Excessively high debt: Pod Rate > 25%

### **Corn Supply**

At the beginning of each Season, Topcorn increases the Corn supply by deltaB if there was a liquidity and time weighted average shortage of Corns across the pools in the Oracle Whitelist over the previous Season. Essentially, Topcorn will mint the number of Corns that need to be sold in the pools on the Oracle Whitelist to return the Corn price to a dollar.

Stalkholders and Pod holders receive 1/2 of new Corn mints each. If there is no Active Fertilizer, Stalkholders and Pod holders receive 1/2 of new Corn mints each. If there are neither Pods nor Active Fertilizer, Stalkholders receive 100% of new Corn mints.

### **Soil Supply**

At the beginning of each Season, TopCorn sets the Soil supply.

When P < 1 over the previous Season (_i.e._, deltaB < 0), the Soil supply is equal to deltaB, the sum of the liquidity and time weighted average excess of Corns across the liquidity pools on the Oracle Whitelist over the previous Season.

When P ≥ 1 over the previous Season (_i.e._, deltaB ≥ 0), Topcorn is still willing to issue debt in order to measure changing demand for Soil. The Soil supply is based on the number of Pods that Ripen and become Harvestable at the beginning of the Season, the Temperature, and the TopCorn debt level. A greater number of Pods Ripening increases the Soil supply. Higher Temperature and debt level decrease the Soil supply.
