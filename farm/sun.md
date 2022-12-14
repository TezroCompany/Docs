# Sun

The TopCorn peg maintenance mechanism requires a protocol-native timekeeping mechanism and regular code execution on BSC. The Sun keeps time on the Farm in Seasons and incentivizes cost-efficient and timely calling of the sunrise() function.

TopCorn adjusts itself to return the Corn price to its value peg at the beginning of every Season. Each Season is \~1 hour long. The first Season began when TopCorn was deployed on September 29, 2022.

The exact beginning of each Season may vary as Seasons do not begin until the sunrise() function has been called through an BSC transaction. The first transaction that successfully calls the sunrise() function after the top of each hour UTC begins a new Season. TopCorn only accepts one sunrise() function call per Season.

TopCorn covers the cost of calling the sunrise() function by awarding the sender of an accepted sunrise() function call with newly minted Corns. To encourage regular sunrise() function calls even during periods of congestion on BSC while minimizing cost, the award starts at 1 Corns and compounds 1% every additional second that elapses for 100 seconds.

Upon acceptance of the sunrise() call, the Sun:

1. Increments the Season number;
2. Calculates deltaB, the sum of the time and liquidity weighted average shortage or excess Corns across liquidity pools on the Oracle Whitelist;
3. Changes the Weather;
4. Sets the new Soil supply;
5. Mints Corns if necessary; and
6. Awards Corns to the address that successfully called the sunrise() function.
