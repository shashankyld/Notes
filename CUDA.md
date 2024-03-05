## Verify existing installations
1. To check existing Nivida Driver
```
nvidia-smi
```
2. To check existing CUDA version
```
nvcc --version
```

## Before installing from scratch, remove existing installations
1. Remove NVIDIA graphics driver
```
# To remove NVIDA driver packs
sudo apt purge nvidia*
```
```
# To remove any residual config files
sudo apt autoremove
```
```
# Reboot System
sudo reboot
```

2. Remove CUDA Toolkit
```
# To uninstall the CUDA Toolkit packages
sudo apt-get remove --autoremove cuda
```
```
# To remove any residual files and directories
sudo rm -rf /usr/local/cuda*
```
```
# To remove CUDA Toolkit installation directory
sudo rm -rf /usr/local/cuda
```
```
# Reboot System
sudo reboot
```
