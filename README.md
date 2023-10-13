# Multilingual_translation_dataset_processing_and_generation
This project processes and generates data from a multilingual translation dataset

## Task 1: Setup of Python3 Development Environment
This project is developed using Pycharm and the virtual environment used: venv

The relevant dependencies for this project are: 
* Pandas Library
* Json Library
* Skicit-Learn Library
* Jsonlines Library
* Xlsxwriter Library

The project uses the : [Massive Dataset](https://huggingface.co/datasets/AmazonScience/massive/viewer/af-ZA/train?p=1)

In task 1: 
* The folder **Combined_data** is generated which contains a list of files in the format *en-xx.xlx*, where *xx* is each of the languages specified in the massive dataset, matched to the **English** language which is the specified *pivot*.
* A script file *generate.sh* is used to call the python scipt **generate.py** which automatically produces the files specified above by adding the name of the folder holding the dataset. ie
  
<img width="1037" alt="generate" src="https://github.com/Abbymuso1/Multilingual_translation_dataset_processing_and_generation/assets/89918147/9552e84d-336e-4720-b83c-2e79bcded92d">


## Task 2: Generate separate jsonl files with test, train and dev respectively.
* This required the use of *Scikit-Learn* Library for the **train-test-split**, where chosen json files : Swahili, English and German had a training, testing and development sets generated from them and stored in the **Split_data**  Folder. 
* The files are named according to the split such that the files produced from the English json file are: '*en-US-dev.jsonl*', '*en-US-train.jsonl*', '*en-US-test.jsonl*'

## Task 3: Generate one large json file showing all the translations for train sets : Pivot language - English
* This basically produced a Json file in ***pretty print*** to view the translations from *English* to the other languages with train sets.


