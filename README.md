# PQQ: A Novel Question Data Augmentation Method for Low-Resource Question-Answering Tasks

## Overview

The Question-Answering (QA) domain faces unique challenges in low-resource settings due to data scarcity and lack of domain-specific training. PQQ is designed to effectively augment QA datasets, enhancing performance especially in low-resource scenarios.
![screenshot20231019](https://github.com/andongBlue/PQQ_QA/assets/33241971/bec6b819-ccff-4124-8509-38ed4b26b37a)

*Figure 1: An overview of the PQQ approach, utilizing Bert-large for prompted answers, a Question Generation model for generating questions, and Bert as a question filter.*

## Key Contributions

- Introduction of **Prompt Answer** to generate diversified but contextually similar answers.
- Application of **Question Generation** models to produce a diverse set of questions.
- Utilization of a **Question Filter** to refine the generated questions, retaining those that are logically coherent with the original dataset.

## Research Context

- **Data Augmentation in QA**: Addresses data scarcity issues in low-resource QA tasks.
- **Utilization of Large Models**: Harnesses the internal knowledge of large models to improve the quality of augmented data.
- **Content Consistency**: Strives for a balance between content consistency and noise introduction.


## Installation
## The source code for this project will be released soon.
```bash
git clone https://github.com/yourusername/PQQ.git
cd PQQ
pip install -r requirements.txt
```

## Usage

```bash
python run_pqq.py --input_data "path/to/your/data"
```

## Experimental Results

- **Underperformance of ChatGPT**: ChatGPT significantly underperformed on our experimental dataset.
- **PQQ Outperforms**: Our methodology surpasses conventional data augmentation methods.
- **High-Resource QA Tasks**: PQQ also shows efficacy on high-resource tasks like SQUAD1.1 and TriviaQA~\cite{rajpurkar2016squad, joshi2017triviaqa}.
- **Benchmarking**: Bert-base with PQQ outperforms Bert-Large without PQQ, establishing its efficacy.

## Dependencies

- Python 3.x
- PyTorch
- Transformers Library
- NLTK

## Citation

If you find our work useful, please consider citing:

TODO


