# NLP-tutorials
Slides and code for the intro to NLP class at the Data Science Retreat  @ Berlin, 28 Oct 2019

## Installation

### Requirements
Besides python >= 3.7 and pip, the required libraries are listed in `requirements.txt`.

Code is cross-platform. Tested in Windows and Ubuntu 18.04.

### Setting up a virtual environment
Linux  | Windows
------------- | -------------
sudo apt-get install virtualenv / pip install virtualenv | pip install virtualenv
virtualenv --python /usr/bin/python3.7 venv	  | virtualenv venv
source venv/bin/activate  | venv\Scripts\activate.bat
pip install -r requirements.txt  | pip install -r requirements.txt 
pip install http://download.pytorch.org/whl/cpu/torch-0.4.1-cp36-cp36m-linux_x86_64.whl (1)* | pip install http://download.pytorch.org/whl/cpu/torch-0.4.1-cp36-cp36m-win_amd64.whl (1)*
pip install torchvision  | pip install torchvision
pip install torchtext==0.2.3  | pip install torchtext==0.2.3 
python -m spacy download en_core_web_sm | python -m spacy download en_core_web_sm

(1)* replace "cpu" in link if you plan to use GPU: "cu80" for CUDA 8, "cu90" for CUDA 9.0, "cu92" for CUDA 9.2, ...

_If you require a newer version,
please visit http://pytorch.org/ and follow their instructions to install the relevant pytorch binary._


## Text Classification 
[Text Classification with BoW + TF-IDF + Naive bayes and SVM](code/TextClassification.ipynb)
based on http://github.com/Gunjitbedi/Text-Classification

[Text Classification with word embeddings + neural network](code/TextClassificationNN.ipynb)

[Sentiment Analysis with specific word embeddings + neural network](code/SentimentAnalysis.ipynb)

## Recomendation 
[Recomendation using Colaborative filtering](code/Recomendation.ipynb)

## Named Entity Recognition 
[Named Entity Recognition](code/NamedEntityRecognition.ipynb)

## Bonus material
[Transformers: Attention is all you need](code/annotated-transformer/The_Annotated_Transformer.ipynb)

copied from http://nlp.seas.harvard.edu/2018/04/03/attention.html 
Paper: https://arxiv.org/abs/1706.03762
