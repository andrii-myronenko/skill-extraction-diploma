# Master Thesis: Improving Skill Extraction from Job Postings Using Synthetic Data and Advanced Language Models

This repository contains the code developed during the experimentation phase of my Master Thesis titled **"Improving Skill Extraction from Job Postings Using Synthetic Data and Advanced Language Models."**

## Main Experiments with Synthetic Data Generation

The main experiments focusing on synthetic data generation can be found in the following files:

- [Synthetic Data Zero-Shot Generation.ipynb](./Synthetic%20Data%20Zero-Shot%20Generation.ipynb)
- [Synthetic Data Template-based Generation.ipynb](./Synthetic%20Data%20Template-based%20Generation.ipynb)
- [Synthetic Data Validation + Rephrase Generation.ipynb](./Synthetic%20Data%20Validation%20+%20Rephrase%20Generation.ipynb)
- [Synthetic Data Rephrases Without Skills Generation.ipynb](./Synthetic%20Data%20Rephrases%20Without%20Skills%20Generation.ipynb)

The data for the experiments can be found in the following directories:

- [Second Experiment](./data/experiments/second_experiment): Corresponds to 20% generation using template-based method.
- [Fourth Experiment](./data/experiments/fourth_experiment): Corresponds to 40% generation using template-based method.
- [Third Experiment](./data/experiments/third_experiment): Corresponds to 20% generation using template-based + rephrasing method.
- [Fifth Experiment](./data/experiments/fifth_experiment): Corresponds to 40% generation using template-based + rephrasing method.
- [Sixth Experiment](./data/experiments/sixth_experiment): Corresponds to 60% generation using template-based method.
- [Seventh Experiment](./data/experiments/seventh_experiment): Corresponds to 80% generation using template-based method.
- [Eighth Experiment](./data/experiments/eighth_experiment): Corresponds to 100% generation using template-based method.

Each experiment folder contains an `enriched_skillspan` folder, where the data is stored in BIO format. This includes both the original training data from SkillSpan and the added synthetic data. The file responsible for the mapping and enrichment process is:

- [Enrich SkillSpan Data With Synthetic Sentences.ipynb](./Enrich%20SkillSpan%20Data%20With%20Synthetic%20Sentences.ipynb)

The SkillSpan dataset used in this project is available at [SkillSpan Repository](https://github.com/kris927b/SkillSpan), and all synthetic data generated in these experiments was used to train models using the code in that repository.

## Mapping BIO to MRC

The file responsible for mapping BIO format data to MRC format is:

- [MRC from BIO.ipynb](MRC%20from%20BIO.ipynb)

The mapped dataset is used in the following repository to test the standalone performance of large language models in skill extraction:

- [GPT-NER Repository](https://github.com/andrii-myronenko/GPT-NER)

## Additional Files

### Initial Experiments on LLM Capabilities

The following files were used in initial experiments exploring the capabilities of LLMs for skill extraction:

- [Combine SkillSpan dataset entries into complete postings.ipynb](Combine%20SkillSpan%20dataset%20entries%20into%20complete%20postings.ipynb)
- [Extract skills from Job Postings using GPT-3.5.ipynb](Extract%20skills%20from%20Job%20Postings%20using%20GPT-3.5.ipynb)
- [Extract skills from Job Postings using GPT-4.ipynb](Extract%20skills%20from%20Job%20Postings%20using%20GPT-4.ipynb)
- [Extract skills from Job Postings using LLama.ipynb](Extract%20skills%20from%20Job%20Postings%20using%20LLama.ipynb)

### Analysis of Datasets

The following files were used for conducting descriptive analysis of the datasets:

- [Sentence embedding visualization + BLEU Calculation.ipynb](Sentence%20embedding%20visualization%20%2B%20BLEU%20Calculation.ipynb)
- [SkillSpan and ESCO dataset analysis.ipynb](SkillSpan%20and%20ESCO%20dataset%20analysis.ipynb)
