# hl-sim

This is a collection of files needed to reproduce a simple hearing loss simulator based on a Raspberry Pi with Patchbox OS and Pure Data.

This includes the complete PD patch with all "abstractions" (subsystems) needed for a hearing loss simulation:
- hlsim (main patch)
- channelstrip (bundles most of the processing, used once for each channel/ear)
- filterbank (separates the audio signal into "critical frequency bands" according to Zwicker) 
- loss (used to reduce the level by x dB)
- recruitment (simulates abnormal loudness growth)
- spectral_smearing (simulates spectral smearing effect due to outer hair cell loss by a kind of ring modulation)
- temporal_smearing (simulates temporal smearing effect due to loss in temporal resolution by sliding the signal phase back and forth)

To reproduce this, you need a Raspberry Pi (any full format from 2 Mod B. to 5 should work), a Hifiberry DAC+ADC Pro audio interface (or similar), a Roland CS-10EM Headset (or similar) and an installation of Patchbox OS (https://blokas.io/patchbox-os/).

Setup instructions will be provided within this repository by Nov 2023.
