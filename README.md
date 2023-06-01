# Diffraction Simulator

## Standalone viewer associated with *Methods in Enzymology* Volume 687
**Supported platforms**. Optimal performance requires Linux_x86_64, accelerated with an Nvidia GPU, either Volta or Ampere architecture.  

**Installation**. Please navigate on [this page](https://github.com/cctbx-xfel/erice_2022) to the "+1 release" URL.  There follow the instructions for download and install.  Find the binary bundle listed under "Assets" and click the link for the [cctbx.xfel-2023.5.26-Linux-x86_64.sh](https://github.com/cctbx-xfel/erice_2022/releases/download/v2023.5.22/cctbx.xfel-2023.5.26-Linux-x86_64.sh).

**Running the program**.  Start from the command line with:

```simtbx.sim_view``` 

**Documentation**.  Read the docs on Github at the [sim_erice](https://github.com/dermen/sim_erice#readme) page including explanations of the controls and the tunable parameters. You can also launch the viewer with `-h` or `--help` to see the help message.  More details on which parameters are tunable is visible by typing:

```simtbx.sim_view -c -e5 -a2```

**Community input**.  The [source code repository](https://github.com/dermen/sim_erice) makes provision for users to report bugs, request features, and contribute code. 

**Developer build**.  Find the source bundle listed under "Assets" and click the link for [Source code](https://github.com/cctbx-xfel/erice_2022/archive/refs/tags/v2023.5.22.tar.gz)

## Google Colab notebook
*Due to mismatched CUDA driver versions between Google Colab and conda, the notebook is not currently functional. Please check back.*

<!--The quickest way to get started is to run the [Google Colab notebook](https://colab.research.google.com/drive/1dXWW7ptKDxWVmfMGFKeXq9cagALLH5i4?usp=sharing) directly from your browser. The compute nodes are hosted and allocated by Google, so you can simply connect with the default settings and begin executing cells. The first cells set up the environment (the notebook, a conda environment, and the cctbx.xfel installation) and the rest set up the simulation viewer. After running all the cells in order, you should see a set of widgets controlling the parameters of the diffraction experiment and an image of the simulation that updates in lockstep with these parameters. More detailed instructions can be found in the notebook itself.-->

## Jupyter notebook
*Future implementation as a Jupyter notebook is contemplated.*

<!--As an alternative to the above, you can run a derivative of the Colab notebook using Jupyter. Download the Colab notebook -- this should already be an .ipynb file. Remove the cells at the very beginning that give instructions to Colab, and run the installation of cctbx.xfel in a conda environment locally instead, as follows: You will first need to install [conda](https://conda.io/projects/conda/en/stable/user-guide/install/download.html) and then run `conda install mamba`. Then you can run `mamba install -q -c xfel cctbx.xfel`. Activate the new conda environment and run Jupyter with the cctbx-xfel build of python. In the simplest case, this means running `jupyter-notebook simtbx.sim_view.ipynb`. The steps from "Load modules" onward should work identically to how they work in the Colab notebook.-->

# Erice 2022 International School of Crystallography, 57th Course
## Diffuse Scattering: The Crystallography of Dynamics, Defects, and Disorder

This repository holds the software for the tutorials used during the
2022 International School of Crystallography held in Erice, Italy on
the topic of [Diffuse Scattering: The Crystallography of Dynamics, Defects,
and Disorder](https://crystalerice.org/2022/).

### Installation
There are installers for each platform. You can run the installer on
linux and macOS by typing
```
chmod u+x cctbx.xfel-<version>-<platform>-<architecture>.sh
./cctbx.xfel-<version>-<platform>-<architecture>.sh -b -p <prefix>
```
Then add the `bin` directory to your path in `bash` with
```
export PATH=<prefix>/bin:${PATH}
```
or in `csh` with
```
setenv PATH <prefix>/bin:${PATH}
```
For Windows, run the executable and select a directory for installation.
To add the commands to your `%PATH%` in the Command Prompt, type
```
set PATH=<installation path>\Library\bin;<installation path>\Scripts;<installation path>;%PATH%
```
By default, the `<installation path>` is `C:\Users\<user name>\cctbx.xfel`.
The commands exist in 3 locations which is why 3 directories are added to the `%PATH%`.

### Installer Notes
The installers for Apple Silcon (`MacOSX-arm64`) and Windows do not have
dependencies for molecular dynamics.

### Juptyer Notebook
Once the software is installed and your path updated, you can start
Jupyter lab with
```
jupyter lab
```

### Advanced Usage
The installed software is essentially a `conda` environment, so if you
have `conda` installed, you can activate the environment with
```
conda activate <prefix>/
```
Then you can modify or add dependencies.
