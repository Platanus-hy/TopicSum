Source code for [TopicSum: Topic Controllable Multi-Document Summarization via Hierarchical Attention Mechanism]

## Setup

```
pip3 install -r requirement.txt
```

### Download and preprocess the datasets

Our experiments are based on Multi-News dataset published by [Fabbri](https://paperswithcode.com/paper/multi-news-a-large-scale-multi-document).

### source structure
- files
	- stop_words.txt
- models
- src
	- utils
	- preprocess
	- modules
	- models
	- model-tpt
	- model_topic_kvs
	- model_mtsp
	- run.py
	- run_LDA.py
- vocab

### Trained Models
We will release our trained MDSTopicKVS model on [Google Drive](https://).

## Training Script
```
python run.py --mode train --model MDS/MDSTopicKVS --use_cuda 
```

## Test
```
python run.py --model test --model MDS/MDSTopicKVS --use_cuda 
```