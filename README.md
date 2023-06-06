# NER-Course-Nir

<h1 align="center">NER-Course-Nir</h1>
<h5 align="center">NER-Course-Nir: Development of a Benchmark Corpus to Support Entity Recognition in Job Descriptions</h5>

## The problem
Detecting and extracting salient entities is an important task in many real-world information extraction applications such as text classification,
Search algorithms and content recommendations.
Recruiting, companies today benefit from automated systems to acquire up-to-date information about job roles and detailed candidate profiles in terms of skills, qualifications and experience.
However, the development of entity recognition (ER) to perform these tasks suffers severely due to the lack of publicly available datasets.
Most of the available datasets consist of general news articles (newspapers, etc.).

## The solution
Developing better tools for searching for employees for open positions.
Learning NN algorithms that will classify words into categories such as skills, experience, degree, etc. (from a dataset we will prepare (connecting datasets)).
and running a benchmark between the different algorithms.

## Versioning
1. Python version 3.9
2. Pip version 23.1.2

## Installation
1. Download dataset https://www.kaggle.com/datasets/airiddha/trainrev1  to dataset/Train_rev1_2.csv
2. Download glove.6B.100d.txt if not exists: https://nlp.stanford.edu/projects/glove/ to embedding/glove.6B.100d.txt 
3. Install requirements

## Running
Follow the NER_JOB_DESCRIPTION jupiter notebook to understand how to run the algorithms.

## Datasets
train_rav_1 (https://www.kaggle.com/datasets/airiddha/trainrev1) which shows UK job descriptions, 
which is publicly available Build our data set above the data set defined above according to the three labels: skills, education, experience. 
Initially, we used text entity extraction tools to independently classify these three labels. 
Next, we present a benchmark between model x and model y.

The result datasets will include 3 tags:
SKILL - B-SKILL, I-SKILL
EDUCATION - B-EDU, I-EDU
EXPERIENCE - B-EXP, I-EXP
under dataset sample_dataset.conll file.

## Models
The benchmark will run on 2 models:
1. Flair
2. LM-LSTM-CRF
Both models taken from nlpprogress.com website.

## Model Results
![Screen Shot 2023-06-05 at 13.43.42.png](Screen%20Shot%202023-06-05%20at%2013.43.42.png)