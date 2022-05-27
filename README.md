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
