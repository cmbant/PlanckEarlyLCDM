# Planck PR4 TTTEEE+lowE+lensing Early ΛCDM Parameter Chains

This repository contains the early ΛCDM cosmological parameter chains derived from the Planck from the paper **"CMB Constraints on the Early Universe Independent of Late-Time Cosmology"** by Pablo Lemos and Antony Lewis ([arXiv:2302.12911](https://arxiv.org/abs/2302.12911)).

## Overview

The early ΛCDM parameter chains allow for robust constraints on the early universe's physics while being minimally influenced by assumptions about late-time cosmology. By leveraging empirical constraints on CMB lensing and weak priors on integrated effects such as the Sachs-Wolfe effect and foreground contributions, these chains provide insights into the early universe that are independent of the complexities of late-time structure growth.

## Data

The chains were generated using [Cobaya](https://github.com/CobayaSampler/cobaya) and use:
- Planck PR4 CamSpec likelihood
- Temperature and polarization data (TTTEEE) at ℓ ≥ 30
- Low-ℓ EE polarization data
- Planck PR4 lensing likelihood

## Methodology

Parameters are constrained using an approach that:
- Models CMB lensing empirically using a spline fit to the lensing power spectrum
- Excludes low-ℓ temperature data (ℓ < 30) to avoid ISW sensitivity
- Models residual ISW at ℓ ≥ 30 with a template
- Uses empirical foreground templates
- Treats reionization through a single τ parameter

## Usage

Chains can be analysed or visualized using [GetDist](https://getdist.readthedocs.io/).

The .covmat file has the parameter covariance for Gaussian approximations.


## Citation

If you use these chains or the associated analyses in your work, please cite:
```
@article{Lemos:2023xhs,
    author = "Lemos, Pablo and Lewis, Antony",
    title = "{CMB constraints on the early Universe independent of late-time cosmology}",
    eprint = "2302.12911",
    archivePrefix = "arXiv",
    primaryClass = "astro-ph.CO",
    doi = "10.1103/PhysRevD.107.103505",
    journal = "Phys. Rev. D",
    volume = "107",
    number = "10",
    pages = "103505",
    year = "2023"
}ar={2023}
}
```


 
