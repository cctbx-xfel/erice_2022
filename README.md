# Erice 2022 International School of Crystallography, 57th Course
## Diffuse Scattering: The Crystallography of Dynamics, Defects, and Disorder

This repository holds the software for the tutorials used during the
2022 International School of Crystallography held in Erice, Italy on
the topic of Diffuse Scattering: The Crystallography of Dynamics, Defects,
and Disorder.

### Installation
There are installers for each platform. You can run the installer on
linux and macOS by typing
```
./cctbx.xfel-2022.4.23-<platform>-<architecture>.sh -b -p <prefix>
```
Then add the `bin` directory to your path in `bash` with
```
export PATH=<prefix>/bin:${PATH}
```
or in `csh` with
```
setenv PATH <prefix>/bin:${PATH}
```

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
conda activate <prefix>
```
Then you can modify or add dependencies.
