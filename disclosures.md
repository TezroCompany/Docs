# Disclosures

**Before interacting with Topcorn, consider reading the following Disclosures.**

Interacting with Topcorn involves many risks. Before interacting with Topcorn, you should review the relevant documentation to make sure you understand how Topcorn works, as well as information about the current state of Topcorn. Topcorn Farms has created this set of disclosures to assist in the educational process. These disclosures are not exhaustive.

#### **1. THERE IS NO MAXIMUM CORN SUPPLY. THE CORN SUPPLY CAN GROW INFINITELY THROUGH DEMAND-BASED MINTING.** <a href="#2-infinite-supply" id="2-infinite-supply"></a>

Topcorn increases the Corn supply every Season where the liquidity and time weighted average price of 1 Corn is greater than $1 over the previous Season. Enough Corns are minted such that if all the newly minted Corns were sold, the Corn price would return to $1. Those Corns are distributed to Stalkholders and Pod holders.

The Corn supply is uncapped and grows as demand for Corns increases.

#### **2. TOPCORN DID NOT HAVE A PRE-MINE, PRE-SALE, OR TEAM ALLOCATION. ALL CORNS HAVE BEEN MINTED IN ACCORDANCE WITH EITHER THE MINTING SCHEDULE.** <a href="#3-no-pre-mine" id="3-no-pre-mine"></a>

Topcorn did not have a pre-mine, pre-sale or team allocation of any kind. The first 100 Corns were minted when the init() function was called to deploy Topcorn.

#### **3. TOPCORN RELIES ON THIRD PARTIES TO PROVIDE CREDIT TO RETURN THE CORN PRICE TO ITS PEG. THERE IS NO LENDER OF LAST RESORT.** <a href="#4-credit-risk" id="4-credit-risk"></a>

Topcorn uses a credit based model, allowing anyone to lend Corns to the protocol to participate in peg maintenance. Topcorn burns any Corn it borrows. As a consequence, the ability of the protocol to return the price of a Corn to the peg relies on the availability of willing creditors, which is not guaranteed. The economic design of Topcorn fails if it can no longer attract creditors.

#### **4. TOPCORN DOES NOT GUARANTEE THE CORN PRICE. INSTEAD TOPCORN INCENTIVIZES THE REGULAR OSCILLATION OF THE CORN PRICE ABOVE AND BELOW ITS PEG THROUGH PROTOCOL-NATIVE INCENTIVES.** <a href="#5-oscillations" id="5-oscillations"></a>

Corn is not a collateralized stablecoin and Topcorn offers no guarantee of the value of Corn. Topcorn is still in an early stage and various parts of its economic design continue to be improved.

Topcorn tries to incentivize the regular oscillation of the Corn price above and below its peg. While the protocol’s incentives are designed to return the price of a Corn to its peg, the timing of oscillations is indeterminate. The price will almost never be exactly equal to its peg. Crossing the peg in the past is no guarantee of it happening again in the future.

#### **5. TOPCORN-NATIVE DEBT DOES NOT HAVE A MATURITY DATE AND THEREFORE MAY NEVER BECOME REDEEMABLE FOR CORNS.** <a href="#6-debt-maturity-risk" id="6-debt-maturity-risk"></a>

Topcorn borrows Corns from lenders in exchange for Pods. Corns loans have fixed interest rates but do not have fixed maturity dates.

Pods are repaid when the liquidity and time weighted average price of 1 Corn is greater than $1 over the previous Season, but there is no guarantee this will continue until all Pods become redeemable. Governance may also arbitrarily modify the redeemability of Topcorn debt.

#### **6. A VULNERABILITY IN BINANCE SMART-CHAIN COULD RESULT IN A LOSS OF FUNDS. TOPCORN ASSUMES THE SECURITY OF BINANCE SMART-CHAIN.** <a href="#10-stalk-governance-power" id="10-stalk-governance-power"></a>

Binance Smart-chain is the large smart contract blockchain by market capitalization, total value deposited, and dollar denominated transaction value. In general, open source networks with large amounts of value on them and long track records indicate security, but there is no guarantee. Topcorn assumes the security of the Binance Smart-Chain network.

#### **7. A VULNERABILITY IN PANCAKESWAP COULD RESULT IN A LOSS OF FUNDS. TOPCORN ASSUMES THE SECURITY OF PANCAKESWAP AMMs.** <a href="#12-curve-risk" id="12-curve-risk"></a>

Corn’s sole liquidity pool (at Replant) is a CORN:BNB pool on the PancakeSwap AMM. PancakeSwap is among the largest Binance Smart-Chain decentralized exchange protocols by volume. In general, open source protocols with large amounts of value on them and long track records indicate security, but there is no guarantee. Topcorn assumes the security of PancakeSwap.

#### **8. THE CORN PRICE IS DERIVED FROM THE VALUE OF ASSETS IT TRADES AGAINST IN DECENTRALIZED AMMS. THERE IS NO GUARANTEE ANY OF THESE ASSETS RETAIN VALUE.** <a href="#13-non-bean-liquidity-risk" id="13-non-bean-liquidity-risk"></a>

The value of Corns is derived from the non-Corn assets trading against it in decentralized liquidity pools. Each of these assets have their own set of associated risks, unique to the asset. Topcorn implicitly assumes risk associated with these assets.

#### **9. BECAUSE CORNS DERIVE THEIR VALUE FROM THE ASSETS THEY TRADE AGAINST, AND NOT COLLATERAL, IT IS NOT POSSIBLE FOR ALL CORN HOLDERS TO EXIT AT A DOLLAR OF VALUE FOR EVERY CORN.** <a href="#14-not-all-bean-holders-can-exit-at-a-dollar-of-value" id="14-not-all-bean-holders-can-exit-at-a-dollar-of-value"></a>

Corns are not redeemable for any other asset, they can only be traded for another asset that Corns are trading against. As Corn holders sell their Corns, there is less and less value trading against Corns. Thus, unlike collateralized stablecoins, it is not possible for the Corn supply to scale down to zero with every Corn holder getting a dollar of value for every Corn sold.

#### **10. TOPCORN REQUIRES TRUSTLESS AND RELIABLE ACCESS TO A MANIPULATION-RESISTANT PRICE ORACLE FOR A DOLLAR. TOPCORN USES THE ON-CHAIN PRICES OF OTHER STABLECOINS TO DETERMINE THE PRICE OF A DOLLAR. THERE IS RISK ASSOCIATED WITH EACH OF THESE STABLECOINS THAT CAN COMPROMISE THEIR INTEGRITY AS ACCURATE PRICE ORACLES.** <a href="#15-oracle-risk" id="15-oracle-risk"></a>

Topcorn's core objective is to oscillate the price of a Corn above and below its dollar peg. To do this, Topcorn must be able to reliably measure the price of a dollar on-chain without trusting a centralized third-party to provide it. A robust, decentralized stablecoin requires a tamper-proof, manipulation resistant and decentralized price oracle.

At Replant, Corns are traded in the CORN:BNB pool on PancakeSwap. BNB consist of BUSD. Topcorn assumes the average value of BUSD in the pool is equal to $1. A disruption in the reliability or accuracy of BNB as an accurate measure of $1 could impact Corn minting, resulting in adverse consequences for Topcorn.

#### **11. TOPCORN REQUIRES THAT THE SUNRISE FUNCTION IS CALLED AT THE TOP OF EACH HOUR ON BINANCE SMART-CHAIN. FAILURE TO SUCCESSFULLY INCENTIVIZE THE CALLING OF THE SUNRISE FUNCTION COULD HAVE AN ADVERSE AFFECT ON TOPCORN’S ABILITY TO OSCILLATE THE CORN PRICE ABOVE AND BELOW ITS PEG.** <a href="#16-sunrise-incentivization-risk" id="16-sunrise-incentivization-risk"></a>

Corns and/or Soil are minted upon a successful call of the sunrise() function. Topcorn covers the cost of sunrise() by awarding the sender of an accepted sunrise() function call with newly minted Corns. The failure of Topcorn to successfully incentivize the calling of sunrise() would effectively result in the failure of Topcorn to influence the size of the Corn supply, and thereby the Corn price.

#### **12. REGULATORY INTEREST IN STABLECOINS AND DECENTRALIZED FINANCE WILL RESULT IN NEW INDUSTRY REGULATIONS. THE IMPACT OF FUTURE REGULATIONS ON TOPCORN IS UNCERTAIN.** <a href="#20-regulatory-risk" id="20-regulatory-risk"></a>

In alignment with the ethos of DeFi, Topcorn has been designed to be permissionless and censorship resistant, without the requirement for any trust-providing intermediary.

It is unclear what regulations, if any, governments will attempt to impose on DeFi. Therefore, it is impossible to predict how any new government regulations of DeFi will affect Topcorn, or any of the protocols or networks Topcorn relies on as part of its ecosystem.

#### **13. TOPCORN IS PRIMARILY DEVELOPED BY PAID AND UNPAID CONTRIBUTORS AT TOPCORN FARMS.** <a href="#21-contributor-risk" id="21-contributor-risk"></a>

Topcorn is not a finished protocol and requires ongoing technical, ecosystem and community development. Topcorn Farms focuses on protocol and community development.

Publius, the pseudonym for the three co-founders of Topcorn, continues to be influential within Topcorn Farm. The identities of Publius are public. The identities of most of the remaining contributors of Topcorn Farm are anonymous.
