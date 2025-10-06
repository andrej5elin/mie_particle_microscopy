# mie_particle_microscopy
A jupyterlab-based tool for simulating optical microscope images of small particles inside a capillary using Mie scattering theory.

![alttext](https://github.com/andrej5elin/mie_particle_microscopy/particles.png?raw=true)


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

$ conda create --name microscope
$ conda activate microscope
$ conda install numpy scipy matplotlib numba miepython
$ conda install jupyter
$ jupyter lab

Download the jupyterlab notebook from the repository and run the code.

