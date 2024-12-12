---
language:
- ru
license:
- mit
multilinguality:
- russian
task_categories:
- text-classification
task_ids:
- sentiment-classification
- multi-class-classification
- multi-label-classification
pretty_name: RuIzardEmotions
tags:
- emotion
size_categories:
- 10K<n<100K
---

# Dataset Card for RuIzardEmotions

## Table of Contents
- [Dataset Description](#dataset-description)
  - [Dataset Summary](#dataset-summary)
  - [Supported Tasks and Leaderboards](#supported-tasks-and-leaderboards)
  - [Languages](#languages)
- [Dataset Structure](#dataset-structure)
  - [Data Instances](#data-instances)
  - [Data Fields](#data-fields)
  - [Data Splits](#data-splits)
- [Dataset Creation](#dataset-creation)
  - [Curation Rationale](#curation-rationale)
  - [Source Data](#source-data)
  - [Annotations](#annotations)
  - [Personal and Sensitive Information](#personal-and-sensitive-information)
- [Considerations for Using the Data](#considerations-for-using-the-data)
  - [Social Impact of Dataset](#social-impact-of-dataset)
  - [Discussion of Biases](#discussion-of-biases)
  - [Other Known Limitations](#other-known-limitations)
- [Additional Information](#additional-information)
  - [Dataset Curators](#dataset-curators)
  - [Licensing Information](#licensing-information)
  - [Citation Information](#citation-information)
  - [Contributions](#contributions)

### Dataset Summary

The RuIzardEmotions dataset is a high-quality translation of the [go-emotions](https://huggingface.co/datasets/go_emotions) dataset and the other [emotion-detection](https://www.kaggle.com/datasets/ishantjuyal/emotions-in-text/data) dataset. It contains 30k Reddit comments labeled for 10 emotion categories (__joy__, __sadness__, __anger__, __enthusiasm__, __surprise__, __disgust__, __fear__, __guilt__, __shame__ and __neutral__).
The datasets were translated using the accurate translator [DeepL](https://www.deepl.com/translator) and additional processing. The idea for the dataset was inspired by the [Izard's model](https://en.wikipedia.org/wiki/Differential_Emotions_Scale) of human emotions.

The dataset already with predefined train/val/test splits.

### Supported Tasks and Leaderboards

This dataset is intended for multi-class, multi-label emotion classification.

### Languages

The data is in Russian.

## Dataset Structure

### Data Instances

Each instance is a reddit comment with one or more emotion annotations (or neutral).

### Data Splits

The simplified data includes a set of train/val/test splits with 24k, 3k, and 3k examples respectively.

## Considerations for Using the Data

### Social Impact of Dataset

Emotion detection is a worthwhile problem which can potentially lead to improvements such as better human/computer
interaction. However, emotion detection algorithms (particularly in computer vision) have been abused in some cases
to make erroneous inferences in human monitoring and assessment applications such as hiring decisions, insurance
pricing, and student attentiveness

## Additional Information

### Licensing Information

The GitHub repository which houses this dataset has an
[Apache License 2.0](https://github.com/Djacon/russian-emotion-detection/blob/main/LICENSE).

### Citation Information

```
@inproceedings{Djacon,
 author={Djacon},
 title={RuIzardEmotions: A Dataset of Fine-Grained Emotions},
 year={2023}
}
```