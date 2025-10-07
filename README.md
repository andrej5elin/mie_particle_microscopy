[![DOI](https://zenodo.org/badge/1070628061.svg)](https://doi.org/10.5281/zenodo.17283936)

# mie_particle_microscopy


A jupyterlab-based tool for simulating optical microscope image formation of small particles dispersed in liquid.


We apply principles of Fourier optics to compute image at the magnified side of the lens transform 
from the field in the Fourier plane of the microscope, which we derive using Mie scattering theory. The method allows one to set the microscope focal plane with respect to the capilary wall and set the numerical aperture and bandwidth of the illuminant to simulate temporal and spatial coherence of the illuminant. We also simulate sensor acquisition and convert the field to a measured intensity and apply photon shot noise, and we simulate ADC conversion. 

In the current implementation, the technique is restricted to small illuminant NA and unpolarized input (and output) light. Below is a simulation of 4000 Polystyren (PS) particles with a diameter of 300 nm placed inside a 400 micron thick capillary filled with water. Microscope magnification is 60x and we use a green diode with a bandwidth of 28 nm and with a central wavelength of 550 nm and we use 0.15 condenser NA.

![alttext](https://github.com/andrej5elin/mie_particle_microscopy/blob/main/particles.png?raw=true)


## Requirements

Implementation is done in python for the jupyter lab IDE. You must have a working jupyter lab environment and install the relevant python packages listed below.


* numpy
* scipy
* matplotlib
* miepython

Optional, but highly recommended for faster computation on GPUs:

* cupy (Windows, Linux)
* mlx (Apple)

## Installation and Usage notes

I recommend using anaconda to build [jupyter lab](https://jupyter.org/install).

```console
$ conda create --name microscope
$ conda activate microscope
$ conda install numpy scipy matplotlib numba miepython
$ conda install jupyter
$ jupyter lab
```

Download the jupyterlab notebook from the repository and run the code.

