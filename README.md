# create conda environment
conda create -n train_test python=3.9
pip install requirements.txt

## running codes 
mkdir imgs_out
accelerate launch train_sd_controlnet_simple.py
