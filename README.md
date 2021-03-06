# Tensorflow Tutorial 
## Example with Face Embeddings

### Setting up an environment 
Clone this repo and cd into it.
```bash
git clone https://github.com/abaybektursun/tf_tutorial
cd tf_tutorial
```
Make sure that you have virutalenv
```bash 
pip3 install virtualenv
```

Now we will create a virtualenv. Follow the steps for your operating system
#### Linux
```bash 
virtualenv --system-site-packages -p python3 ./venv
source ./venv/bin/activate
pip3 install --upgrade pip
```
#### Windows
```PowerShell
virtualenv --system-site-packages -p python3 ./venv
.\venv\Scripts\activate
```

### Installing Tensorflow and the other dependencies
If you have an NVIDIA card and want it to be utilized by TF, you can follow the instructions for GPU. Otherwise follow the CPU instructions. 
#### CPU 
```bash
pip3 install -r requirements_cpu.txt
```
#### GPU
```bash
pip3 install -r requirements_gpu.txt
```
In addition, you will have to have CUDA 9.0 and cuDNN installed.
 * Install CUDA 9.0 from here: https://developer.nvidia.com/cuda-90-download-archive
 * Install cuDNN by following instructions for your specific platform here. Make sure to downlad the cuDNN specifically for CUDA 9.0: https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html
 * On Windows, GPU version of Tensorflow only supports Python 3.5.x
 
## Jupyter Notebook
Install new kernel for the jupyter notebook
```bash
ipython kernel install --user --name=tf_tutorial
```
Star the jupyter notebook
```bash
jupyter notebook
```
