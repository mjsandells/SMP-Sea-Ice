# SMP-Sea-Ice


This repository contains the algorithms and descriptions of techniques in support of the following publication:

```
King et al, 2019 placeholder dx.diy.dorg/numbers
```

## Abstract
Local-scale variations in snow density and layering on Arctic sea ice were characterized using a combination of traditional snow pit and SnowMicroPen (SMP) measurements. In total, 14 sites were evaluated within the Canadian Arctic Archipelago and Arctic Ocean on both first (FYI) and multi-year (MYI) sea ice. Sites contained multiple snow pits with coincident SMP profiles as well as unidirectional SMP transects. An existing SMP density model was recalibrated using manual density cutter measurements (n=186) to identify best-fit parameters for the observed conditions. Cross-validation of the revised SMP model showed errors comparable to the expected baseline for manual density measurements (RMSE=34 kg m<sup>-3</sup> or 10.9%) and strong retrieval skill (R<sup>2</sup>=0.78). The density model was then applied to SMP transect measurements to characterize variations at spatial scales of up to 100 m. A supervised classification trained on snow pit stratigraphy allowed separation of the SMP density estimates by layer-type. The resulting dataset contains 58,882 layer-classified estimates of snow density on sea ice representing 147 m of vertical variation and equivalent to more than 600 individual snow pits. An average bulk density of 310 kg m<sup>-3</sup> was estimated with clear separation between FYI and MYI environments. Lower densities on MYI (277 kg m<sup>-3</sup>) corresponded with increased depth hoar composition (49.2%), in strong contrast to composition of the thin FYI snowpack (19.8%). Spatial auto-correlation analysis showed layered composition on FYI snowpack to persist over long distances while composition on MYI rapidly decorrelated at distances less than 16 m. Application of the SMP profiles to determine propagation bias in radar altimetry showed the potential errors of 0.5 cm when climatology is used over known snow density.

```
Placeholder location to embed Figure 1?
```

## Getting Started
There are several Jupyter notebooks within this repository which reproduce the various algorithms and figures used in the publication. To run the notebooks yourself, there are a couple of options:
### a) Interactively in an Internet Browser on Binder
```
placeholder for binder button
```

### b) Locally using Conda
1) Download and install [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
2) Clone this repository:
    ```
    $ git clone https://github.com/kingjml/SMP-Sea-Ice.git
    ```
3) Create the `smp-sea-ice` environment using this repository's environment specification:
    ```
    $ conda env create -f environment.yml
    ```
4) Activate the `smp-sea-ice` environment, and launch Jupyter to explore the notebooks:
    ```
    $ conda activate smp-sea-ice
    (smp-sea-ice) $ jupyter notebook index.ipynb
    ```
5) (*Optional*) If you would like to run the brute-force measurement alignment routine in notebook [#1](./Part_1_Validation.ipynb) yourself, you will need to retrieve the SMP datasets from `placeholder for either AWS S3 or OpenDataPortal URL`