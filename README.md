## Assessing the Impact of Question Ambiguity in Question-Answering (QA) System

### Overview
The __objective__ of this project is to assess how does ambiguity (lexical-semantic) in question affects models performance in QA systems. 

### Short description of the phenomena
Lexical ambiguity relates to words having multiple possible meanings in question (e.g., in question 'Where is the bank?', *bank* can be related to one of the meanings 'finantial institution' or a 'riverbank').

### Experimental Setup
We created a new custom dataset for lexical ambiguity evaluation. It consists of 1,265 ambiguous, same amount of non-ambiguous questions, and a corresponding ground truth answer. Dataset was derived from SQuAD 2.0 answerable questions. Six extractive transformer-based models were evaluated: BERT (base, large), RoBERTa (base, lagre), DeBERTa-V3 (base, large). We used fine-tuned on SQuAD 2.0 versions of the models. Models answer predictions were compared to gold answers. For that, we used Exact Match (EM) and F1 score as a standard metrics, and Sentence-BERT (SBERT) as a task-specific metrics for computing cosine similarity. We also performed a qualitative error analysis of predicted outputs, and based on findings, conducted two additional experiments - special [CLS] token masking and analysis of question length.

STEP 1: Dataset Generation
STEP 2: Dataset Analysis
STEP 3: Model Evaluation
STEP 4: Evaluation with CLS masking
STEP 5: Evaluation with Sentence-BERT

### Files submitted
There are two folders: Data and Figures. The _Data_ folder contains both the input datasets used in the experiments and the datasets generated during the exaluation process. The _Figures_ folder includes all plots and visualizations for the experiments.

### Note
Some plotting code was generated with the assistance of the GPT-40 model. This is indicated in the respective sections of the notebook. 

### A link to GitHub repository
[https://github.com/shmr-anna/assessing-the-impact-of-question-ambiguity-in-qa-systtems]
