# Touche
Code for reproducing of our submission to the CLEF-2020 shared task on argument retrieval.

# Technical

This repository contains some approaches to information retrieval task.
Every approach corresponds to its own \*.py module.

To run some \*.py modules on the restarted machine, we need first to start bert-service which in turn needs restored graph in TensorFlow. Graph restoring and service starting are reproduced in the bash script before the main module starts (**restore_tf_graph.py**, **run_bash_tira3.sh**).
The one of possible Bert weights are on https://drive.google.com/file/d/17VC9ErQ-xRrmyCUf8Oy5gFF-LcsnJosZ/view?usp=sharing

The proper **Transformers**, **Fastai**, **Bert** libraries are in **requrements.txt**


## Degree of comparativeness and comparative structure extraction

**baseline_cam_obj.py**, **lstm_ulmfit_cam_obj.py**

Copy infersent.allnli.pickle(https://drive.google.com/file/d/1bmCg-jPWZ8M0X5RLWtZq0Xq7wYUqc_Og/view?usp=sharing) to "/touche/cam/data/", model.pkl(https://drive.google.com/file/d/1--REAj57WzYC36H6ji2vl7NH5O8fej25/view?usp=sharing) to "touche/cam/src/Backend/data/", glove.840B.300d.txt(https://yadi.sk/d/cgJPQ8RwpFgS-g) to "touche/cam/GloVe/", berttt.hdf5(https://drive.google.com/file/d/1kU_4pqWgJ29kAbhBoMbCrjGZDtQ0zLjY/view?usp=sharing) to "touche/external_pretrained_models"
