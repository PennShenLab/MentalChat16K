
# MentalChat16K

## Overview
MentalChat16K is a benchmark dataset designed to support the development and evaluation of large language models (LLMs) for conversational mental health assistance. The dataset consists of 16,113 question-answer pairs, combining real anonymized interview transcripts from the PISCES clinical trial with synthetic dialogues generated by GPT-3.5 Turbo. This dataset covers a diverse range of mental health topics, including depression, anxiety, and grief, and aims to facilitate the creation of AI-driven mental health support tools.

## 📊 Data Composition
The dataset is divided into two main components:
1. **Real Interview Data**: 
   - Derived from the PISCES clinical trial.
   - Includes 6,338 question-answer pairs paraphrased from 378 transcripts.
   - Focuses on interactions between behavioral health coaches and caregivers of patients in palliative or hospice care.

2. **Synthetic Data**:
   - Generated using GPT-3.5 Turbo.
   - Contains 9,775 question-answer pairs.
   - Covers 33 mental health topics.

## 👥 Demographic Information
The interview data participants are primarily caregivers of patients in palliative or hospice care. Out of 421 caregivers who completed the information survey:
- The majority are female, with 88% identifying as White Caucasians and less than 1% as Hispanic.
- Male caregivers are a small minority, totaling 6, and are predominantly White Caucasians.
- Other racial categories include Asian American, Black/African American, Multi-racial, and others, each comprising smaller proportions of the caregiver population.

## 🛠️ Usage
MentalChat16K is intended for research purposes to advance the development of AI technologies in the mental health domain. It can be used for:
- Fine-tuning and evaluating large language models for mental health counseling.
- Developing empathetic and personalized AI solutions for mental health support.
- Conducting research on conversational AI in sensitive and critical domains.

## 📁 Repository Structure 

This repository includes the following three folders:

1. **[FastChat](https://github.com/ChiaPatricia/FastChat/tree/a85e4ec8975667eb3395d8350fdcc18ae13e879d)**: Contains modifications to the `llm_judge` module for model evaluation using both GPT and Google Gemini.
2. **[MentalChat16K_Main](https://github.com/ChiaPatricia/MentalChat16K_Main)**: The main repository involves paraphrasing interview data using `Mistral-Instruct` and an efficient fine-tuning technique for quantized large language models.
3. **[MentalChat16K_Synthetic_Data_Generation](https://github.com/ChiaPatricia/MentalChat16K_Synthetic_Data_Generation)**: Provides the pipeline for generating synthetic data.

## ⚖️ Ethical Considerations
The dataset prioritizes patient privacy, ethical considerations, and responsible data usage. All real interview data has been anonymized to protect the identities of the participants. Researchers are encouraged to handle the data with care and adhere to ethical guidelines in their work.

## 🔗 Access
MentalChat16K is available for download at [Hugging Face Datasets](https://huggingface.co/datasets/ShenLab/MentalChat16K).

## 📚 Citation
If you use MentalChat16K in your research, please cite the dataset as follows:
```
@dataset{MentalChat16K,
  author    = {Jia Xu, Tianyi Wei, Bojian Hou, Patryk Orzechowski, Shu Yang, Ruochen Jin, Rachael Paulbeck, Joost Wagenaar, George Demiris, Li Shen},
  title     = {MentalChat16K: A Benchmark Dataset for Conversational Mental Health Assistance},
  year      = {2024},
  url       = {https://huggingface.co/datasets/ShenLab/MentalChat16K},
}
```

---
