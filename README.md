# classif-retina

## Introduction 

Kaggle link : 
https://www.kaggle.com/datasets/tanlikesmath/diabetic-retinopathy-resized


## Setup Python environment using Docker

Build Docker image : 
```
docker build --tag classif-retina-image .
```

Create Docker container : 

```
docker run --name classif-retina-container --gpus all -it --shm-size=8gb -v $PWD:/workspace -v <path-to-your-data>:/data classif-retina-image
```