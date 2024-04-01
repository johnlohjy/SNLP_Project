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

