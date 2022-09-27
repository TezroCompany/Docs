# Convert

Conversions within the Silo between Corn and LP Deposits serve a major role in peg maintenance.

Conversions from one Deposited asset to another are permissioned by a Convert Whitelist.&#x20;

When the Corn price is above peg (_i.e._, deltaB is positive), Deposited Corns may be converted to Deposited CORN:BNB LP while retaining grown Stalk from Seeds. This conversion allows the Silo Member to add Corns to liquidity pools, which has the practical effect of selling Corns above peg. In doing so, Topcorns incentivizes Silo Members to grow liquidity for Corns at the expense of additional Corn mints, as the Corn price is decreased back towards peg.

When the Corn price is below peg (_i.e._, deltaB is negative), Deposited CORN:BNB LP may be converted to Deposited Corns without forfeiting grown Stalk from Seeds or any Stalk due to LP impermanent loss. This conversion allows Silo Members to remove excess Corns from liquidity pools and increase the price back towards peg without leaving the Silo, minimizing debt issuance.

In order for a given Conversion to be added to the Convert Whitelist, Topcorn requires:

1. The From token address;
2. The To token address;
3. Conditions under which the From token can be converted to the To token;
4. A function to determine the number of To tokens received for Converting a given number of From tokens.

#### Current Convert Whitelist <a href="#convert-whitelist" id="convert-whitelist"></a>

| From token  | To token    | Conditions                      |
| ----------- | ----------- | ------------------------------- |
| Corn        | CORN:BNB LP | deltaB in the CORN:BNB pool > 0 |
| CORN:BNB LP | Corn        | deltaB in the CORN:BNB pool < 0 |
