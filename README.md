# Extreme Summarization of Research Articles in Multiple Languages
This is a project to perform extreme summarization of research articles in multiple languages using transformer models such as mBart and mT5, implemented using the HuggingFace library. The project aims to generate high-quality summaries of research articles in languages such as German, French, and Spanish and translate them into English.

# Requirements
To run this project, you will need to have the following software installed:

* Python 3.7 or higher
* HuggingFace Transformers 4.2.2 or higher
* NumPy
* Pandas


You will also need to download the pre-trained transformer models for mBart and mT5 from the HuggingFace model hub.

# Dataset
Datasets used in this projects are [SciTLDR](https://github.com/allenai/scitldr), [Multi-XScience](https://github.com/yaolu/Multi-XScience) and [X-SCITLDR](https://github.com/sobamchan/xscitldr) which consists of research articles in multiple languages, including German, French, and Spanish. The dataset is preprocessed and tokenized using the HuggingFace tokenizer.

# Architecture
The project uses transformer models such as mBart and mT5 to perform extreme summarization of the research articles in multiple languages. The models are fine-tuned on the dataset using a sequence-to-sequence architecture, where the input is the research article and the output is the summary.

# Translation
The project also includes a translation step, where the summaries are translated from the original language (German, French, Spanish) into English using the HuggingFace translation pipeline. The translation step improves the readability of the summaries for English-speaking audiences.

# Evaluation
The project includes an evaluation step, where the quality of the summaries is evaluated using metrics such as ROUGE scores. The evaluation step helps to identify the strengths and weaknesses of the transformer models and fine-tuning process.

# Results
The project has been tested on research articles in multiple languages and has achieved good results in generating high-quality summaries and translating them into English.

| Language | Model | Rouge-1| Rouge-2 | Rouge-L | F1    |
| -------- | ----- | ------ | ------- | ------- | ----- |
| German   | mBart | 22.7   | 6.7     | 18.1    | 66.10 |
|          | mT5   | 20.8   | 5.3     | 1.64    | 61.40 |
| French   | mBart | 31.80  | 11.70   | 25.50   | 75.50 |
|          | mT5   | 30.60  | 9.80    | 23.10   | 73.20 |
| Spanish  | mBart | 36.30  | 14.40   | 27.30   | 75.93 |
|          | mT5   | 34.24  | 11.53   | 24.81   | 74.11 |


# Credits
This project was inspired by the work of Lewis et al., "BART: Denoising Sequence-to-Sequence Pre-training for Natural Language Generation, Translation, and Comprehension" (https://arxiv.org/abs/1910.13461) and Raffel et al., "Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer" (https://arxiv.org/abs/1910.10683). The implementation was done using the HuggingFace library.
