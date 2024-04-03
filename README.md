# SNLP_Project 

This branch of the github implements the augmentation component of our project.

Augmentation: the process of inserting additional information such as sentiments to each sentence, phrase or even a word.

The main motivation behind this experiment is to investiate if there are any significant improvements by inserting more information (in our case, sentiments) to the input.

Since more context and/or information being supplied can increase higher quality generations, our team wanted to investigate if this is true for classification tasks through augmentating the inputs. Additionally, this experiment is inspired by the significant boost in specificity & accuracy when utilizing Retrieval Augmented Generation (RAG) systems compared to regular large language models. 

## Setting up

1) Do create a new environment - I used miniconda, any variants of conda or environment managers will do.

2) Perform the following for the required libraries in your preferred terminal:

```terminal
pip install -r requirements.txt
```

3) OPTIONAL: check your hardware if you want to use GPU acceleration - MPS, CUDA etc. Might need to do some tinkering for it work. If not, just use cpu which will work.

---
# Jupyter Notebooks

The notebooks should use the environment you have set up (see above).

There are two main note books for this branch:
1. augment_data.ipynb 
    - Augments data with sentiments in the data/train_2024.csv to augmented_data/train_2024.csv
    - Augments data with sentiments in the data/dev_2024.csv to augmented_data/dev_2024.csv
    - Augments data with sentiments in the data/test_2024.csv to augmented_data/test_2024.csv
2. XLNET_Prediction_Experimentation.ipynb
    - Does the prediction of the trained (without sentiments) model of the test data (augmented_data/test_2024.csv)
    - Does the prediction of the trained (with sentiments) model of the test data (augmented_data/test_2024.csv)

*Important*: The notebooks are currently set up to utilize MPS. For anybody that would like to replicate the process, do change the device to your compatible hardware e.g. CUDA or CPU.
