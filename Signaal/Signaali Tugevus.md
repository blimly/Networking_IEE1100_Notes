
## RSSI - Singaalitugevuse indikaator
- 2G
-  RSSI - *Received Signal Strenght Indicator*
- Vastuvõetava signaali tugevuse indikaator

## ASU 
- ASU - *Arbitrary Strength Unit*



### Seosed 
1. GSM (2G)

$$S[dBm] = 2 * ASU - 113$$
3. UMTS(3G) - (RSCP level (received signal code power))

$$S[dBm] = ASU - 116$$
5. LTE(4G) - (RSRP (reference signal received power))

$$S[dBm] = (ASU - 143) < dBm ≤ (ASU - 140)$$
*The value of 0 maps to RSRP below -140 dBm and the value of 97 maps to RSRP above -44 dBm.*
