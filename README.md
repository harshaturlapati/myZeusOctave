# myZeusOctave
Testing zeus-octave on Windows

## Open Powershell as admin and install WSL
```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
wsl --set-default-version 2
wsl --install -d Ubuntu-20.04
```
## Open WSL terminal
```
wget "https://github.com/conda-forge/miniforge/releases/latest/download/Miniforge3-$(uname)-$(uname -m).sh"
bash Miniforge3-$(uname)-$(uname -m).sh
conda activate
source .bashrc
```
## Set up xeus-octave
```
mamba create -n myenv -c conda-forge xeus-octave
mamba activate -n myenv
mamba install -c conda-forge jupyterlab
```
## Open Jupyter lab and code away
```
jupyter lab
```
