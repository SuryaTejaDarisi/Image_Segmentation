# Image_Segmentation

Image Segmentation is a prominent application of Deep Learning, where the background is segmented/seperated from the objects/entities in the foreground. In this repo, we use Pytorch to perform the Image Segmentation.
<img width="1212" height="411" alt="image" src="https://github.com/user-attachments/assets/c3076bb0-aa57-431c-ba74-64213d5c7f03" />

## Implementation
Initially, let's set up a virtual environment.
### 1. Setting up a Virtual Environment
To create an environment:
```
python -m venv <env_name>
```
To access it:
```
<env_name>\Scripts\activate
```
To deactivate it:
```
deactivate
```

### 2. Installing required Libraries
This repo contains a requirements.txt file which contains all the python libraries required.
```
pip install -r .\requirements.txt
```

### 3. Working on Code
Now, one can work on the notebook.

Various parameters can be changed. More specifically, the below cell in the notebook are configurations and can be chosen from a lot of possibilities.
```
FILE = 'Human-Segmentation-Dataset-master/train.csv'

DEVICE = "cuda" if torch.cuda.is_available() else "cpu"
EPOCHS = 25
LR = 0.03
BATCH_SIZE = 16
IMAGE_SIZE = 320

ENCODER = 'timm-efficientnet-b0'
WEIGHTS = 'imagenet'
```
All other instructions about downloading the dataset are provided in the notebook.

Relevant resources are provided below:  
albumentation documentation : https://albumentations.ai/docs/  
segmentation_models_pytorch documentation : https://smp.readthedocs.io/en/latest/  
