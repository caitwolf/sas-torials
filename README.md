# sas-torials

This repo contains Python scripts and Jupyter notebooks that demonstrate the functionality of the [SasView](https://github.com/SasView/sasview) and [sasmodels](https://github.com/SasView/sasmodels) Python packages for fitting scattering data.

### getting_started

### mini_tutorials

### parallel_fitting

## Installation

### Python 3 Environment

Using a [Python 3 environment](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-environments.html) for all `sasmodels` tutorials in this work is recommended. If you need to install Python 3 on your machine, I recommned the Anaconda package. Installation instructions for the latest version for your operating system can be found at <https://www.anaconda.com/products/individual>. 

A new sasmodels environment can be created from either (1) the provided yml file or (2) by manually installing the required packages.

1. Creating from yml file:
`conda env create -f environment.yml`
2. Installing individual packages:

		conda create -n sasmodels python=3.8
		conda activate sasmodels
		conda install -c conda-forge numpy pandas matplotlib jupyter pyopencl scipy pillow lxml h5py ipykernel nb_conda_kernels pip
			

### `sasview` and `sasmodels`

The `sasmodels` and `bumps` packages ned to be installed using `pip` following the following commands:

	pip install sasmodels
	pip install bumps
	
Next, the source code for both `sasview` and `sasmodels` should be downloaded to your computer. You can either download the code direclty from GitHub, or clone the repos with the following commands:

	git clone https://github.com/sasview/sasmodels.git
	git clone https://github.com/sasview/sasview.git

Finally, `sasview` will need to be aded to your Python path variable so that it is accessible to import as a package. This can be accomplished by adding the following lines at the top of each Python script or Jupyter notebook. In many of these tutorials, these lines will be provided for you, simply uncomment and edit them as needed.

	import sys
	 sys.path.append("/path/to/sasview/src")
	 import sas
	 
