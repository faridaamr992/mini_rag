# mini_rag

This is a minimal implementation of the RAG model for question answering.

## Requirements 

- Python 3.8 or later

#### Install Python using MiniConda 

1) Download and Install MiniConda from [here](https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
)

2) Create a new environment using the following command:
```bash
$ conda create -n mini-rag python=3.8
```

3) Activate the environment:
```bash
$ conda activate mini-rag
```
## Installation

### Install the required packages 

```bash
$ pip install -r requirements.txt
```
### Setup the envirnment variables 

```bash
$ cp .env.example .env
```
Set your envirnment variables in the `.env` file like `LLM_API_KEY` value.

## Run the FastAPI server 

```bash
$ uvicorn main:app --reload --host 0.0.0.0 --port 5000
```
## POSTMAN Collection

Download the POSTMAN collection from [/assets/mini-rag-app.postman_collection_jason](/assets/mini-rag-app.postman_collection.json)

## Run Docker Compose Services

```bash
$ cd docker
$ cp .env.example .env
```

update `.env` with your credentials