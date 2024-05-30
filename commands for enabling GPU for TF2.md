wget https://repo.anaconda.com/archive/Anaconda3-2024.02-1-Linux-x86_64.sh
bash Anaconda3-2024.02-1-Linux-x86_64.sh -> Yes to T&C -> Yes to start Conda

conda create -n speaking python=3.10.4
conda activate speaking

sudo apt install ubuntu-drivers-common
sudo ubuntu-drivers devices
sudo apt install nvidia-driver-535 -> sudo reboot
nvidia-smi

sudo apt install nvidia-cuda-toolkit

https://www.tensorflow.org/install/source#gpu -> Check tensorflow version vs cudnn version required

conda install -c conda-forge cudnn=8.9
conda install -c conda-forge tensorflow=2.15.0
