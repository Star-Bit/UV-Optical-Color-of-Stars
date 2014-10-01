UV-Optical-Color-of-Stars
=========================

Purpose: To predict the UV/optical colors of stars using models of stellar atmospheres by focusing on three different filters (U,B,and V)

Problem: When performing photometry upon an astronomical object, the spectrum of the star is modified by the transmission characteristics of the instrument. No two instruments are the same, so the differences in transmission must be taken into account. This can be done through calibration.

Johnson Photometric System: In this system Vega is assigned zero apparent magnitude in all filters (U,B,V,R, and I). The apparent magnitude of any other star can be found by determined by comparing the ratio of its flux to the flux of Vega measured by a particular instrument.

m = -2.5log(fstar/fvega)

We need to generate a mapping between the observed system and the standard system.

Goals of the lab: 
1. Simulate photometric observations of blackbodies through the Johnson U,B, and V filters.
2. Simulate observations of real stars using model stellar spectra and compare them to what we find for the blackbodies.

Summary of photomodel.sav folder:
    TEFF - effective temperature in Kelvin for 110 model stellar spectra
    METALLICITY - abudance of heavy metals in 110 model stellar spectra
    WAVELENGTH - 800 element array of wavelengths at which fluxes are calculated
    FLUX - 800 by 110 element array containing 800 fluxes for each of the 110 model stellar spectra
    UBV_TRANSMISSION- 800 by 3 element array containing the standard transmission functions for the Johnson U,B, and V filters. 
    VEGA - 800 element array containing the spectrum of Vega measured at the same wavelengths as in WAVELENGTH. 
