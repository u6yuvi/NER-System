# NER-System
Build NER System from Scratch 

## Entity Extraction 
1. Data Creation
	1. Creating BIO scheme tags for Sequence Data
2. Data Augmentation using:
	1. Character Replacement
	2. Entity Replacement
	3. Neighbouring context Replacement
3. Model Training
	1. Using Vanilla Pytorch Datasets and Dataloaders
	2. Using HuggingFace Trainer Module
	3. Using Pytorch Lightning Framework
	4. Flair Training Framework
	5. Spacy Training Framework

4. Model Evaluation
5. Model Optimisation


## Entity Retreiver
1. Data Creation
	1. Sparse Labeling/Judgements
	2. Dense Labels/Judgements
2. Different approaches to explore:

	Lexical Based<BR>
	1. TFIDF
	2. BM25
	3. BM25F
	
	Semantic Based
	1. BiEncoder
3. Evaluation Metric
	1. Offline Metric
		1. Binary Relevance Metric
			1. Mean Reciprocal Rank[Focus on the 1st relevant document]
			2. Mean Average Precision [ Good for 
	2. Online Metric

## Model Development
### Available Frameworks we will be exploring
1. Spacy
2. Flair
3. HuggingFace Transformer

### Steps
1. Data Processing and Understanding

Our objective will be to take one of the NER dataset and do preprocessing to create NER training labels in BIO scheme and understand the nature of the text by doing some basic data analysis.

2. Data Clustering 
3. Model Training 
4. Model Evaluation

## Model Optimisation


## Building Model Inference Endpoint.


## Building Retreiver System
### Concepts
1. Represent document in the inverted index format.
2. TFIDF ,BM25 and BM25F 

### Lexical Search using ElasticSearch
    1. TFIDFRetriever
    2. BM25Retriever

#### [Elastic Search Installation Guide](https://www.elastic.co/guide/en/elasticsearch/reference/current/targz.html)


## Running Pipelines using Elyra

## Model Deployment using KServe/Kubeflow


# Getting Started 
# clone project 
```
git clone https://github.com/u6yuvi/NER-System.git nersystem
cd nersystem/
git checkout docker_template_exp
```
# create conda environment [ner_system]
```
conda env create -f environment.yml 
conda activate ner_system
```
