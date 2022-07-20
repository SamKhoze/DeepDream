# Run the app 
conda activate /Users/sam/aiProjects/deepdream/deepdream_env
streamlit run /Users/sam/aiProjects/deepdream/deepdream_app.py


# Streamlit Demo: Deep Dream First time installation

# Mac M1 installation 
# Step 1: Download and Install miniforge3
https://gist.github.com/mrdbourke/79aef5b47607c2306e6dc10830b54505

# Step 2: Activate miniforge3
# 
source ~/miniforge3/bin/activate

# Step 3: Create a working directory to setup environment
# or you can name any other project name directory
# 
# mkdir deepdream_venv
# cd deepdream_venv

# Step4: Make and Activate Conda Environment 
# Note: Python 3.8 is the most stable for using the following setup
# 
conda create --prefix ./deepdream_env python=3.8

# To activate conda environment 
# 
conda activate /Users/sam/aiProjects/deepdream/deepdream_env

# Step 5: Install TensorFlow
# To install TensorFlow dependencies from Apple Conda channel.
# 
conda install -c apple tensorflow-deps

# To install base TensorFlow (Apple's fork of TensorFlow is called tensorflow-macos)
# 
python -m pip install tensorflow-macos

# To install Apple's tensorflow-metal to leverage Apple Metal (Apple's GPU framework) for M1, M1 Pro, M1 Max GPU acceleration
# 
python -m pip install tensorflow-metal

# Step 6:  Install common AI and ML packages
# 
conda install pandas numpy matplotlib scikit-learn
# To install PyTorch 
# 
conda install pytorch torchvision torchaudio -c pytorch

# install streamlit
conda install -c conda-forge streamlit

# To run the app
streamlit run /Users/sam/aiProjects/deepdream/deepdream_app.py


## General instruction to run this demo 

```
# Make a venv 
# Activate venv
# Install dependencies 
pip install -r requirements.txt
streamlit run deepdream_app.py

### Questions? Comments?

Please ask in the [Streamlit community](https://discuss.streamlit.io).
