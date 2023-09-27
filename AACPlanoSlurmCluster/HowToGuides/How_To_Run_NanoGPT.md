# How To Build and Run NanoGPT on Plano Slurm Cluster
- https://github.com/karpathy/nanoGPT
- Examples below use `1CN128C8G2H_2IB_MI210_Ubuntu22` slurm partition which has MI210 compute nodes. 
# Setup Environment 
Allocate an Ubuntu 8GPU MI210 workload and SSH to a node from the partition `1CN128C8G2H_2IB_MI210_Ubuntu22`
```
salloc --exclusive --mem=0 --gres=gpu:8 -p 1CN128C8G2H_2IB_MI210_Ubuntu22
```
In the SSH session, load ROCm 5.5.1 Environment
```
module load rocm-5.5.1
```
Load anaconda3 modulefile
```
module load anaconda3/4.12.0
```
Source the `conda.sh` file 
```
. $CONDA_ROOT/etc/profile.d/conda.sh
```
Create conda environment named `nano` with python 3.8
```
conda create -n nano python=3.8 -y 
```
Activate the newly created `nano` environment 
```
conda activate nano 
```
Install Stable Pytorch Release 
- https://pytorch.org/get-started/locally/
```
pip3 --no-cache-dir install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/rocm5.4.2
```
Install nanoGPT dependencies
- https://github.com/karpathy/nanoGPT#install
```
pip3 install --no-cache-dir numpy transformers datasets tiktoken wandb tqdm
```
# NanoGPT Examples
Clone `nanoGPT` github repository 
```
git clone https://github.com/karpathy/nanoGPT.git
```
Change to `nanoGPT` directory 
```
cd nanoGPT/
```
The following steps can be found on the official nanoGPT page 
- https://github.com/karpathy/nanoGPT#quick-start

Prepare GPT shakespeare character dataset 
```
python3 data/shakespeare_char/prepare.py
```
Train GPT shakespeare character data 
```
python3 train.py config/train_shakespeare_char.py
```
Sample the model that was trained 
```
python3 sample.py --out_dir=out-shakespeare-char
```
## Reproducing GPT-2 
- https://github.com/karpathy/nanoGPT#reproducing-gpt-2

Prepare OpenWebText dataset 
```
python3 data/openwebtext/prepare.py
```
Train GPT-2 on OpenWebText dataset using torchrun  
```
torchrun --nnodes=1 --standalone --nproc_per_node=8 train.py config/train_gpt2.py
```
