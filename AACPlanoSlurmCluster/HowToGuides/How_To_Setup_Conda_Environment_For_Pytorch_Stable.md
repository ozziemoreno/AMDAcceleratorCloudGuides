# How To Setup a PyTorch Conda Environment on Plano Slurm Cluster
Allocate an Ubuntu 8GPU MI210 job from the partition `1CN128C8G2H_2IB_MI210_Ubuntu22`
```
salloc --exclusive --mem=0 --gres=gpu:8 -p 1CN128C8G2H_2IB_MI210_Ubuntu22
```
In the allocated session, load ROCm 5.5.1 Environment
```
module load rocm-5.5.1
```
Load anaconda3 modulefile `4.12.0` 
```
module load anaconda3/4.12.0
```
Source the `conda.sh` file
```
. $CONDA_ROOT/etc/profile.d/conda.sh
```
Create conda environment named `pt-stable` with python 3.8
```
conda create -n pt-stable python=3.8 -y 
```
Activate the conda environment that was just created 
```
conda activate pt-stable
```
Install Stable Release of Pytorch
- https://pytorch.org/get-started/locally/
![image](https://github.com/ozziemoreno/AMDAcceleratorCloudGuides/assets/109979778/67e9a1b2-39fb-4a13-abd6-5fad3b83e5e9)
```
pip3 --no-cache-dir install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.4.2
```

