# Range-Enhancement-Of-Drones

In this project, we conducted an experimental study to enhance the communication range of drones by optimizing the performance of the antennas used in their communication systems. Leveraging the powerful software-defined radio platform, GNU Radio, and the ADALM Pluto SDR hardware, we systematically explored various aspects of signal processing and synchronization to achieve our goals.

Our study began with the fundamental principles of digital communication, focusing on the modulation, transmission, demodulation, and synchronization processes. Using GNU Radio, we designed and implemented a comprehensive flowgraph that included several key components:

1. Pluto SDR Source: Captured the incoming signal from the ADALM Pluto SDR device, serving as the input for our processing chain.
2. Automatic Gain Control (AGC): Adjusted the signal gain to maintain a consistent power level, optimizing the signal for further processing.
3. Frequency-Locked Loop (FLL) Band Edge: Ensured frequency synchronization by tracking and aligning the carrier frequency of the received signal.
4. Root Raised Cosine (RRC) Filter: Shaped the signal to reduce intersymbol interference and control bandwidth, improving spectral efficiency.
5. Skip Head: Removed initial samples to eliminate transient effects and focus on the relevant signal portion.
6. Symbol Synchronization: Aligned the sampling instants with the transmitted symbol timing, enabling accurate symbol recovery.
7. Costas Loop: Provided phase synchronization by tracking and adjusting the phase of the received signal, crucial for coherent demodulation.

In our experiments, we modulated the transmitted signals using Quadrature Phase Shift Keying (QPSK) and analyzed the received signals to measure key performance metrics, including signal-to-noise ratio (SNR) and bit error rate (BER). We also calculated the beamwidth of the antenna at various frequencies to understand its directional characteristics.

The beamwidth measurements at different frequencies (5.15 GHz, 5.35 GHz, 5.725 GHz, and 5.825 GHz) provided insightful data:

- At 5.15 GHz, the beamwidth was 70 meters, corresponding to an angular beamwidth of approximately 20.24 degrees.
- At 5.35 GHz, the beamwidth was 80 meters, with an angular beamwidth of approximately 22.85 degrees.
- At 5.725 GHz, the beamwidth was 100 meters, corresponding to an angular beamwidth of approximately 27.77 degrees.
- At 5.825 GHz, the beamwidth was 130 meters, with an angular beamwidth of approximately 34.40 degrees.

These results highlighted the antenna's performance across different frequencies, indicating a broader coverage area at higher frequencies but with reduced directional accuracy.

Overall, this project provided valuable insights into enhancing the communication range of drones, demonstrating the effectiveness of systematic signal processing and synchronization techniques using GNU Radio and ADALM Pluto SDR. The findings contribute to the development of more capable and reliable UAV communication systems for various applications, including aerial surveillance, disaster response, and precision agriculture.
