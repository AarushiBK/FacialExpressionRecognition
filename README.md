## Facial-Expression-Recognition
## Dataset
In our experiments, we use the dataset from [FER2013](https://www.kaggle.com/c/challenges-in-representation-learning-facial-expression-recognition-challenge/data).

Image Properties: 48 x 48 pixels, labels: 0=Angry, 1=Disgust, 2=Fear, 3=Happy, 4=Sad, 5=Surprise, 6=Neutral.

**Install dependencies using Anaconda:**
 ```bash
conda create -n fer python=3.8
source activate fer
pip install opencv-python==4.4.0.42 pillow==7.2.0
conda install pytorch==1.6.0 torchvision==0.7.0 cudatoolkit=10.2 -c pytorch
```

Note: the version of 'cudatoolkit' must match the running version of your machine.

## Train
Within ```./Landmark-Driven-Facial-Expression-Recognition``` directory, run following command:
 ```bash
    bash train.sh
```

## Test with Pretrained Model
**Prepare pretrained model:**
- You can download pretrained model here [Google Drive](https://drive.google.com/file/d/1bCIHS6GdTxMnfCjdopzrm5DXsk9bjeQg/view?usp=sharing), or [Baidu Drive](https://pan.baidu.com/s/14pDf39hEliSWmIjKDFYkzA) with password: v0zm.

- Unzip downloaded files and move 'resnet18.pth' into ```./model_save/``` directory.

**Test:**
- Within ```./Landmark-Driven-Facial-Expression-Recognition``` directory, run following command:
 ```bash
    bash test.sh
```
