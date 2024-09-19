### Sample Input

- **Number of Bits to Transmit:** 10000
- **SNR Range (in dB):** 0:5:30
- **Modulation Type:** 2 (QPSK)
- **Enable Rayleigh Fading:** 1 (Yes)
- **Enable Interference:** 1 (Yes)
- **Interference Type:** 1 (Sinusoidal)

### Sample Output

#### 1. **Bit Error Rate (BER) vs SNR Plot**

For this input, the output would show two plots:

- **Simulated BER**: Calculated using the QPSK modulation scheme under Rayleigh fading, AWGN, and sinusoidal interference.
- **Theoretical BER**: This represents the theoretical BER for QPSK in an AWGN-only channel, acting as a baseline.

**Key Observations:**
- At lower SNR values (0–10 dB), the simulated BER is significantly higher due to the combined effects of noise, fading, and interference.
- As SNR increases, the BER decreases, and the curve approaches the theoretical BER for higher SNR values (above 20 dB), indicating better signal quality.

#### BER vs SNR Plot Example:

![Example BER vs SNR Plot](https://i.imgur.com/Nl7lEwL.png)  


---

#### 2. **Received Signal Constellation**

For **QPSK**, the constellation diagram will consist of four points representing the symbol mapping. The received signal will show how noise, interference, and fading distort the signal points away from their ideal positions.

**Key Observations:**
- At low SNR values, the constellation points will appear more scattered, indicating severe signal degradation.
- At high SNR values, the points will cluster more closely around the ideal QPSK constellation points, indicating better signal recovery.

#### QPSK Received Constellation Plot Example:

![Example QPSK Constellation](https://i.imgur.com/fxMOG50.png)  


---

### Output Data Table (Sample):
This table shows some values of simulated and theoretical BER for different SNR levels.

| **SNR (dB)** | **Simulated BER (QPSK)** | **Theoretical BER (QPSK)** |
|--------------|---------------------------|----------------------------|
| 0            | 0.186                     | 0.1587                     |
| 5            | 0.083                     | 0.0786                     |
| 10           | 0.012                     | 0.0110                     |
| 15           | 0.0021                    | 0.0007                     |
| 20           | 0.0003                    | 0.000032                   |
| 25           | 0.00002                   | 0.0000004                  |
| 30           | 0.000001                  | 0.00000001                 |

### Conclusion:
- At **low SNR** (0–10 dB), the simulated BER is higher due to the interference and fading. 
- At **high SNR** (20–30 dB), the BER approaches the theoretical values, indicating successful signal recovery as the channel conditions improve.

