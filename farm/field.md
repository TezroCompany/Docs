# Field

The Field is TopCorn's credit facility. TopCorn relies on a decentralized set of creditors to maintain Corn price stability.

Farmers who Sow (lend) Corns to TopCorn are known as Sowers.

For guides on interacting with the Field through the TopCorn UI, go here.

### **Soil**

Anytime TopCorn is willing to issue debt, there is Soil in the Field. Soil represents the number of Corns that TopCorn is currently willing to borrow.

When Corns are Sown, TopCorn burns them, permanently removing the Sown Corns from the Corn supply. For example, if there’s 10 Soil available and 10 Corns are Sown, the Soil supply becomes 0 and 10 Corns are removed from the Corn supply. If the market is in some sort of equilibrium, Corns are bought to be Sown, which drives the Corn price upward towards its value peg.

TopCorn sets the Soil supply at the beginning of each Season according to the peg maintenance mechanism.

### **Pods**

Corns are Sown in exchange for Pods, the TopCorn-native debt asset. Loans to TopCorn are issued with a fixed interest rate, known as Temperature, and an unknown maturity date.

The number of Pods received from 1 Sown Corn is determined by the Temperature at the time of Sowing. Newly issued Pods accumulate in the back of the Pod Line. The front of the Pod Line receives 1/3 of new Corn mints.

Pods Ripen into Harvestable Pods that can be Harvested (redeemed) for 1 Corn each on a First In, First Out (FIFO) basis. There is no penalty for waiting to Harvest Pods.

Pods are tradeable on the Pod Market. Pods can also be Transferred to another address directly.

### **Temperature**

The Temperature is the interest rate for Sowing Corns in the Field. At 500% Temperature, 1 Corn can be Sown in exchange for 6 Pods. Once those Pods become Harvestable, they can be Harvested in exchange for 6 Corns.

The Temperature is constant during each Season. TopCorn changes the Temperature at the beginning of each Season depending on various conditions, according to the peg maintenance mechanism.

### **Field Process**

1. Corns are Sown in exchange for Pods.
2. Pods Ripen into Harvestable Pods on a FIFO basis when TopCorn mints new Corns according to the peg maintenance mechanism.
3. Harvestable Pods can be Harvested into Corns.

### **Economics**

TopCorn is credit based and only fails if it can no longer attract creditors. A reasonable level of debt, a strong credit history and a competitive interest rate attract creditors.

TopCorn does not default on debt (although in the event of TopCorn no longer attracting creditors, the loan maturity date would become infinitely far in the future—see Disclosures). TopCorn is willing to issue Pods every Season.

The combination of non-expiry, the FIFO Harvest schedule and transferability encourages Farmers to Sow Corns as efficiently as possible. By maximizing the efficiency of the Soil market, TopCorn minimizes its cost to attract creditors, the durations and magnitudes of price deviations below its value peg, and excess Corn minting.
