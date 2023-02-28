# Scipy 2023 Description

## Gammapy: a Python Package for Gamma-Ray Astronomy Version v1.0

By observing the very high energy (VHE) range of the electromagnetic spectrum we can gain valuable insight into to the extreme universe, including remnants of supernova explosions and surroundings of black holes. In the past VHE gamma-ray astronomy was typically conducted by small, closed collaborations as a subfield of particle physics. However, with hundreds of sources now identified,
VHE gamma-ray astronomy has emerged as a new branch of Astronomy. This
field now provides the high energy context for understanding the physical processes occurring throughout the universe, across the entire electromagnetic spectrum.

The next generation of ground based gamma-ray instruments, particularly the Cherenkov Telescope Array (CTA), is set to revolutionize gamma-ray astronomy.
With an anticipated sensitivity ten times greater than current telescopes, it has the potential to attract a community of thousands of gamma-ray astronomers. Furthermore, it will operate as an open observatory, making both data and analysis tools readily available to the public.

This contribution introduces the inaugural stable version (v1.0) of Gammapy, a Python package for gamma-ray astronomy and the primary library for the future CTA science tools. Leveraging the scientific Python ecosystem, including Numpy, Scipy, and Astropy, Gammapy offers a comprehensive set of standard data analysis tools, making it an indispensable resource for most gamma-ray astronomers. By utilizing common open data formats, Gammapy also enables existing instruments such as VERITAS, H.E.S.S., or HAWC to export and archive their data, preserving it for future analysis using improved methods. Additionally, it facilitates the combination of data from multiple instruments, resulting in more sensitive analyses with greater statistics and a larger energy range.

Gammapy tackles the varied structure of gamma-ray data and science analysis cases by implementing a uniform API for N-dimensional sky maps. This API is independent of the underlying pixelization scheme and supports local WCS, allsky HEALPix, and region-based projections. These data structures prove useful for a broad range of applications and astronomers.

Building on these core data structures, Gammapy features a maximum likelihood fitting framework that enables simultaneous modeling of gamma-ray emission in four dimensions: space, energy, and time. By providing a general likelihood interface, Gammapy enables science users to integrate gamma-ray data with astronomical data from other wavelengths, as well as with neutrino data. Thanks to its straightforward Python API, Gammapy can be paired with other Python-based broadband emission modeling packages, allowing for direct measurement of parameters pertaining to common underlying astrophysical processes. This feature is crucial to realizing the full potential of true multi-wavelength and multi-messenger Astronomy.

Lastly, we will discuss the valuable lessons learned during our journey to achieve v1.0 quality for an openly developed package. This will involve addressing concerns regarding maintainability, selection of dependencies, and API design. We believe that sharing our experience will be helpful to other Python projects in the future.