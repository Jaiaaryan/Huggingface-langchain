# Huggingface-langchain
Running 1000s of LLMs locally

## Huggingface
- **transformers** - opensource python library, which lets us to use tons of model from huggingface
- **Hugging face** is a platform
    - Free and 
    - paid models
- If need one can fine tune these models and use in the needed projects


## Langchain
- Python package makes it easy to work with LLMs
- Has features such as 
    - memory
    - connect multiple models

## Requirements.txt:
- langchain
- transformers
- langchain-huggingface

# To get started:
## Fetch access token:
1. Make an account on huggingface.co, because many of the models expect us to agree some terms and license agreements, before we can download and use them
2. Access token - create new, name as wanted and copy it

## Setup project
3. Create a new venv and install packages
    - python -m venv venv
    - ./venv/Scripts/activate
    - pip install -r requirements.txt
4. **Adding Huggingface token**:
    - In the venv terminal type the followin
    - *huggingface-cli login --token INSERT_YOUR_TOKEN --add-git-credentials*


## Running models using GPU:
By default when you run the programm it will display the following in the output
**Device set to use cpu**
- To use nvidia-GPUs for this
    - download and install cudatoolkit
- To check if it is installed
    - *nvcc --version* or
    - *nvidia-smi*
- install pytorch specifically for GPU
    - get the link that is appropriate for you in the pytorch page
    - it creates a combo of installation line based on your device
