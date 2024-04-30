# 🌿 SARRA-O: Spatial Crop Model

This is the README file for SARRA-O.

## Description

SARRA-O is a spatial crop model that simulates crop processes at the plot scale. It is a tool developed by CIRAD and UMR TETIS that allows for crop simulation over large areas and in a variety of situations.

The model simulates biomass production limited by water and radiation, and considers various agricultural practices such as sowing strategy, seeding density, irrigation strategy, cultivar choices, and the overall level of intensification.

It is based on the formalisms of SARRA-H, which itself is a are more detailed version of the SARRA model, a simple dynamic water balance model used to estimate the impact of climate scenarios on annual crops. In SARRA-H, the plant is considered as a conduit that couples atmospheric demand (sink) with a "useful" water reserve in the soil (source) - a conduit with variable resistance depending on the physical constraint (stress). The SARRA-H model assume that crop performance is a simple function of accumulated water stress over a growing cycle.

SARRA-H has demonstrated good robustness across spatial scales (from plot to region) and for multiple applications, such as at the AGRHYMET early warning system for food security in the CILSS countries, local climate risk analysis, and water requirement estimation. However, its validity relies on the presence of strong water limitation and/or significant spatial or temporal variability of this limitation. In other words, this model is based entirely on growth reduction rather than simulating potential yield.

Compared to other models such as CERES, APSIM, and STICS, the SARRA-H model is deterministic and relatively simple, but simulates more processes than AQUACROP, which is a reference model proposed by FAO. SARRA-H is integrated into a flexible environment that manages a library of formalisms and a database. This model replicates plot-scale processes, enabling regional-scale analysis. Moreover, it can serve as a basic support for other scientific themes through complementary modules or interfaces with other models (meteorological, socio-economic, etc.).

SARRA-O performs SARRA-H spatialization by using a grid system, and encapsulates this computation capacity along West Africa in a Java software based on the Ocelet Modeling Platform (OMP).

## Installation

The SARRA-O software was developed in Java. To install it, you must have Java and follow these steps:

1. Download the installer at [this address](http://sarra-h.teledetection.fr/wp-content/SARRA-O_v1.11_hotfix_20230331_setup.exe)
2. Execute the installer

## Usage

The SARRA-O interface consists of different panels to manage the simulation study area, simulation scenarios, output variables, and the launch of simulations.

The software requires climatic input data such as precipitation, temperature, global radiation, and evapotranspiration, as well as information about agricultural practices. Results can be saved as GeoTIFF images for analysis.

You will find a climate and rainfall data starter pack for Niger 1982-2021 available on Zenodo [doi:10.5281/zenodo.11091602](https://zenodo.org/doi/10.5281/zenodo.11091602), that will allow you to run example simulations.

## Documentation

You can find comprehensive documentation of the software [at this address](https://github.com/SARRA-cropmodels/SARRA-O/blob/main/docs/Petit_manuel_SARRA-O_V7.pdf). ⚠️ Note, this is the documentation for the previous version, although most of the information is there, some points may differ from the current version of the software.

## Contribution and Support

Development forge is hosted by Cirad at https://gitlab.cirad.fr/sarrao, and maintained by @MathCastets.

Contributions to SARRA-O are welcome. You can contribute by reporting bugs, proposing new features by opening a ticket [in the Issues section](https://github.com/SARRA-cropmodels/SARRA-O/issues).

User support is also provided preferentiallt by opening a ticket [in the Issues section](https://github.com/SARRA-cropmodels/SARRA-O/issues). If needed you can reach us at sarra-h@cirad.fr. 

## License

SARRA-O is distributed under the CeCILL-C v1.0 license. Please consult the `LICENSE` file for more information.
