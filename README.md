[![<a-hekker>](https://circleci.com/gh/a-hekker/udacity-microservice-api.svg?style=svg)](https://circleci.com/gh/a-hekker/udacity-microservice-api)

## Project Summary

A given a pre-trained, `sklearn` model that has been trained to predict housing prices in Boston according to several features, such as average rooms in a home and data about highway access, teacher-to-pupil ratios, and so on. You can read more about the data, which was initially taken from Kaggle, on [the data source site](https://www.kaggle.com/c/boston-housing). This project operationalizes a Python flask app—in `app.py`—that serves out predictions (inference) about housing prices through API calls. This project could be extended to any pre-trained machine learning model, such as those for image recognition and data labeling.

## Instructions

* Create a virtualenv and activate it `python3 -m venv ~/.devops` `source ~/.devops/bin/activate`
* Run `make install` to install the necessary dependencies

### Running `app.py`

1. Standalone:  `python app.py`
2. Run in Docker:  `./run_docker.sh`
3. Run in Kubernetes:  `./run_kubernetes.sh`
4. Make prediction using an example: `./make_prediction.sh` 

## Short Explanation of Files   
* folder model_data contains the pretrained model.
* output_txt_files contain log files from running the app in docker and in kubernetes.
* app.py contains the application as an api loading a pretrained model and offering the user to predict houserprices.
* .circleci contains the required config file for continous integration usuing circleci


