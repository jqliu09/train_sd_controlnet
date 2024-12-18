# Sample codes of training stable diffusion on stivo
GPU storage: ~ 13 GB.  
Task: Filling the circle under instruction.  

## create conda environment
conda create -n train_sd python=3.9  
conda activate train_sd  
pip3 install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121  
pip install requirements.txt  

## running codes 
mkdir imgs_out  
accelerate launch train_sd_controlnet_simple.py  
