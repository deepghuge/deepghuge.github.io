---
title: "Characterizing Turbulence in CME Sheaths (Master's Project)"
excerpt: "<img src='/images/masters.png' width='615'>"
collection: portfolio
---

The ongoing master's project, under the guidance of Professor Prasad Subramanian (IISER Pune) is driven by the motivation that Earth-directed solar Coronal Mass Ejections (CMEs) often interact with the magnetosphere, causing geomagnetic
storms that disrupt a range of technologies we routinely rely on. A good understanding of the CME-magnetosphere
interactions are key to mitigating the consequences of such storms. The extent of CME-magnetosphere interaction is
governed substantially by conditions in the CME sheath (which is the leading part of Earth-directed CMEs). This
project aims to characterize turbulent magnetic field, density, and velocity fluctuations in CME sheaths.

Since high-frequency fluctuations are the drivers for turbulence in the solar wind and with the consideration that through the onset of turbulence, the scaling laws in the MHD range change slightly for CME Sheaths to ejecta or Magnetic cloud and background/ambient solar wind, we have attempted to separate the CME sheath (boundary) based on a comparison of power present inside the turbulent high-frequency fluctuations in CME sheaths to Magnetic Cloud (MC) and background Solar wind; this is based of a quantity (modulation index) is a measure of power inside these high-frequency fluctuations in the CME sheath to that of low-frequency fluctuation in the background solar wind. 

(Completed Part)
This statistical study involved data from 152 events with an identifiable shock present(this was included to check the bias) and 256 earth-directed CME events with mixed events (with and without shock), where the events span from 1995 to 2021. This analysis was done through open-source time series data [linked here](https://wind.nasa.gov/mfi_swe_plot.php)  from NASA's Wind Spacecraft, where each event contains about 3600 data points. Histograms of modulation index and spectral index for proton density, magnetic field, and velocity for all events (152 + 256) were produced for CME sheath, MC and solar wind background. Results from these have already proven that using modulation index is better when approaching to separate the CME sheath compared to looking into spectral indices.  

(Part I'm currently working on)
One of the key outcomes of this project is to relate it to the space weather conditions that are influenced by the interaction of CME sheath and MC to Earth's magnetosphere. This part of the project focuses on links between the modulation index and the Dst(disturbance storm time) Index for the same events. The granularity created through the separation of CME into CME sheath, MC, and Background solar wind lets us peek into the impact of these high-frequency turbulent fluctuations inside the sheath on the earth's magnetosphere individually and also as a whole. Plenty of possibilities exist where this high-frequency selection criterion changes can influence the modulation index and its correlation with the Dst Index and it would be interesting to look into. 

(I plan do this next)
-> I have used the Discrete Fourier Transforms of this time series data. Reproducing it with Wavelet transform might help to reduce the standard deviation in the histograms due to it's robustness in handling non-uniform time series data.
-> Try to create the smallest sliced time window to where the separation in CME sheath, MC and background solar wind is possible.
-> Explore the possibility of creating a statistics-based prediction model/algorithm using the modulation index to identify the sheath-MC boundary.
-> Look deeper into the connections between the modulation index and the Dst Index.
