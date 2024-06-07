# Cell-Segmentation-Using-Yolo-v8-and-Azure

This repository contains the code and workflows for a cell segmentation project utilizing YOLO v8 and Azure services. The project is structured to handle data ingestion, validation, model training, and deployment using Docker and GitHub Actions for CI/CD.

## Workflows

1. constants
2. entity
3. components
4. pipelines
5. app.py


## Data Ingestions
![Data Ingetions](https://github.com/KhushJani/Cell-Segmentation-Using-Yolo-v8-and-Azure/assets/88198216/c86f9356-4f92-4cad-95b2-9944b93b4cba)

## Data Validation
![Data validation](https://github.com/KhushJani/Cell-Segmentation-Using-Yolo-v8-and-Azure/assets/88198216/f83b757f-ea9c-4f4a-a1a9-9c6241cca5a2)

## Model Trainer
![Model trainer](https://github.com/KhushJani/Cell-Segmentation-Using-Yolo-v8-and-Azure/assets/88198216/b20280bb-eec4-45c7-a3d4-602d8410d02b)


# How to run?
### STEPS:

Clone the repository

```bash
[https://github.com/KhushJani/Cell-Segmentation-Using-Yolo-v8-and-Azure.git]
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n cell python=3.8 -y
```

```bash
conda activate cell
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```


# AZURE-CICD-Deployment-with-Github-Actions

## Save pass:

S6tXzK7IxUHz9O/9jkhciLsseddeQ++E+OcD7nQYy8+ACRDtEgUW


## Run from terminal:

docker build -t cellseg.azurecr.io/cell:latest .

docker login cellseg.azurecr.io

docker push cellseg.azurecr.io/cell:latest


## Deployment Steps:

1. Build the Docker image of the Source Code
2. Push the Docker image to Container Registry
3. Launch the Web App Server in Azure 
4. Pull the Docker image from the container registry to Web App server and run 
