# Arabic Climate Sentiment Analysis Experiments

This repository contains a collection of notebooks and experiments for Arabic sentiment analysis, with a focus on climate-related data and cross-dataset generalization.

## Available Experiments
All fine-tuning notebooks include data preprocessing script and model training and evaluation pipelines used to run the core experiments. 
Processed datasets can be generated using the scripts. All scripts are shared as Jupyter notebooks were they can be easily accessed.

#### Climate-Tuned Models

- Climate-tuned-AraBERT.ipynb
  This file includes the script used to fine-tune the AraBERT model on ClimaSentAR and evaluate it on testing samples from ClimaSentAR, ASAD, ASTD, and SemEval. The file also includes: 
  - The script used for the preprocessing steps applied on the datasets before fine-tuning and inference
  - The script used for the feature engineering to transform dataset into numerical representations throgh AraBERT tokenizer.
  - The script used to draw confusion matrices, ROC, precision recall curves of the AraBERT model across all datasets.
  - The script used to generate macro and weighted average precision, recall, and F1 score and, and per-class classification performance.

- Climate-tuned-ALLaM.ipynb  
  This includes the script used to fine-tune the ALLaM on ClimaSentAR and evaluate it on testing samples from ClimaSentAR, ASAD, ASTD, and SemEval. The file also includes:
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh ALLaM tokenizer.
  - The script used to generate macro and weighted average precision, recall, and F1 score.

- Climate-tuned-Fanar.ipynb  
  This includes the script used to fine-tune the Fanar on ClimaSentAR and evaluate it on testing samples from ClimaSentAR, ASAD, ASTD, and SemEval. The file also includes:
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh Fanar tokenizer.
  - The script used to generate macro and weighted average precision, recall, and F1 score.


- Climate-tuned-Jais.ipynb  
  This includes the script used to fine-tune the Jais on ClimaSentAR and evaluate it on testing samples from ClimaSentAR, ASAD, ASTD, and SemEval. The file also includes:
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh Jais tokenizer.
  - The script used to generate macro and weighted average precision, recall, and F1 score.

#### ASAD-Tuned Models

- ASAD-tuned-AraBERT.ipynb  
  This file includes the script used to fine-tune the AraBERT model on ASAD and evaluate it on testing samples from ASAD, ClimaSentAR. The file also includes: 
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh AraBERT tokenizer.
  - The script used to draw confusion matrices, ROC, precision recall curves of the AraBERT model across all datasets.
  - The script used to generate macro and weighted average precision, recall, and F1 score and, and per-class classification performance.

- ASAD-tuned-ALLaM.ipynb  
  This includes the script used to fine-tune the ALLaM on ASAD and evaluate it on testing samples from ASAD, ClimaSentAR. The file also includes:
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh ALLaM tokenizer.
  - The script used to generate macro and weighted average precision, recall, and F1 score.

- ASAD-tuned-Fanar.ipynb  
  This includes the script used to fine-tune the Fanar on ASAD and evaluate it on testing samples from ASAD, ClimaSentAR. The file also includes:
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh Fanar tokenizer.
  - The script used to generate macro and weighted average precision, recall, and F1 score.

- ASAD-tuned-Jais.ipynb  
  This includes the script used to fine-tune the Jais on ASAD and evaluate it on testing samples from ASAD, ClimaSentAR. The file also includes:
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh ASAD tokenizer.
  - The script used to generate macro and weighted average precision, recall, and F1 score.

### Similarity Experiments

- Cosine_Similarity_Using_TF_IDF.ipynb  
  This file includes the script used to evaluate the cosine similarity using TF-IDF between ClimaSentAR, ASAD, ASTD, SemEval

- Cosine_Similarity_Using_AraBERT.ipynb  
  his file includes the script used to evaluate the cosine similarity using AraBERT embeddings between ClimaSentAR, ASAD, ASTD, SemEval

### Data Analysis
- EDA.ipynb
  This file includes the script used for EDA experiments. The file includes:
  - The script used to evaluate distribution of classes in the data
  - The script used to evlyate summary of noise features (URLs, Emojis, Non-ASCII characters, Diacritics, Redundant punctuations, Line breaks/tab/extra whitespaces, hashtags, and usernames). 
  - The script used to plot the hashtag distribution image and token length distribution in ClimaSentAR.

### Data Balancing

- SMOTE_Climate-tuned_Change_Whole_AraBERT.ipynb
  This file includes the script used to fine-tune the AraBERT model on ClimaSentAR with SMOTE and evaluate it on testing samples from ClimaSentAR, ASAD, ASTD, and SemEval. This file also includes:
  - This script used to apply SMOTE procedure on the training samples from ClimaSentAR.
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh AraBERT tokenizer.
  - The script used to generate macro and weighted average precision, recall, and F1 score. 

### Domain Adaptation Experiments (Ablation Studies Conducted)

- DAPT_On_Unlabeled_Climate_Text_(Train_Set_=_ASAD).ipynb  
- DAPT_on_Unlabeled_Text_(Train_Set_=_ClimaSentAR).ipynb  
- Adapter_Fusion_(Train_set_=_ClimaSentAR).ipynb  
- Additional_Training_ASAD_ClimaSentAR.ipynb  
- Additional_Training_ASAD_ClimaSentAR_ASTD_SemEval.ipynb  

These files includes the script used to generate ablation study experiments throungh domain adaptation techniques (DAPT, adapter fusion, and additional training). These files also includes:
  - The script for the preprocessing steps applied on the datasets before fine-tuning and inference.
  - The script used for the feature engineering to transform dataset into numerical representations throgh AraBERT tokenizer.
  - The script to generate the macro and weigthed average precision, recall, and F1 score across all datasets.

### Comparison with Literature

- Climate_SVM_(Nabil_et_al).ipynb  
- Climate_AraBERT_(Alharbi_et_al).ipynb  
- Climate_SVM_(Mulki_et_al).ipynb  

These files includes the scripts used to replicate literature experiments to train literature models on ClimaSentAR and evaluate on test samples from ClimaSentAR, ASAD, ASTD, and SemEval. These files include the script used to generate F1 scroes across all datasets.

### Statistical Significance 

- pairwise AraBERT vs ALLaM.xlsx  
- pairwise AraBERT vs Fanar.xlsx  
- pairwise AraBERT vs Jais.xlsx  

These files includes the McNemar significance results.

### Predictions of AraBERT Fine-tuned
- ASAD-Climate.xlsx
  This file includes the predictions of ASAD-tuned AraBERT model on ClimaSentAR 

- Climate-ASAD.xlsx
  This file includes the predictions of Climate-tuned AraBERT model on ASAD

- Climate-ASTD.xlsx
  This file includes the predictions of Climate-tuned AraBERT model on ASTD

- Climate-SemEval.xlsx
  This file includes the predictions of Climate-tuned AraBERT model on SemEval

### Examples of ClimaSentAR across four discourse categories
- domain_tweets.csv
- mixed_tweets.csv
- policy_tweets.csv
- stance_tweets.csv

These files includes examples from ClimaSentAR across the four discourse categories: domain-descriptive, policy-oriented, mixed-sentiment, and stance-driven expressions.

Whole raw dataset can be downloaded from data availability link in the manuscript.