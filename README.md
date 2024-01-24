# Multi-Class Hate Speech Classification using NoahBERT

## Abstract

In this project, we address the challenge of hate speech detection, specifically focusing on the differentiation between hate speech, offensive language, and neutral content, an underexplored area in existing research. Distinguishing between hate speech and offensive language is vital for online platforms to effectively filter harmful content, safeguard users, and foster a more respectful online community. Combining datasets from Ousidhoum et al. and Davidson et al., we curated a comprehensive dataset with 4000 offensive, 3000 neutral, and 2000 hate speech instances. Fine-tuning BERT resulted in a baseline accuracy of 74.9%. In response, we introduced NoahBERT, a modified model incorporating an additional layer and dropout, achieving an enhanced accuracy of 78.9%. Our work contributes to the critical task of improving online toxicity detection and fostering a safer digital environment.

## Platform and Version

- Python: 3.10.9
- PyTorch: 1.10.0

## Required Python Libraries

- numpy
- transformers (BertForSequenceClassification, AdamW, BertConfig, BertTokenizer)
- PyDrive
- tqdm
- matplotlib
- scikit-learn

## Project Flow

We combined data from the MLMA English Hate Speech dataset and Davidson et al's Automated Hate Speech Detection data, sampling from the combined dataset. The classes used and other details are explained in the report. The data is divided into three folders: training, validation, and test. After fine-tuning the parameters, we applied the data to pre-trained BERT and the advanced NoahBERT model.

## File Structure

- **Implementation_Notebook_CS747_FinalProject_NoahBERT.ipynb**: Complete code implementation.
- **Plan.txt**: Ideation and project plan.
- **Report-FinalProject-CS747DL-Pratish_Sreeja-G01354094_G01360679.pdf**: Final report submitted to CS747 Deep Learning at GMU.
- **data/en_dataset.csv**: Dataset from MLMA Hate Speech Detection by Ousidhoum et al.
- **data/en_dataset_with_stop_words.csv**: Same dataset as above, but with stopwords included.
- **data/final_data.csv**: Our generated final dataset.
- **data/labeled_data.csv**: Data by Davidson et al from [GitHub](https://github.com/t-davidson/hate-speech-and-offensive-language/tree/master).
- **video_link.txt**: Link to the project's YouTube video.

## Declaration
Project submitted towards the partial procurement of credits for CS747 Deep Learning at GMU under Professor Daniel Barbara.


For a detailed understanding of the project, please refer to the [report](Report-FinalProject-CS747DL-Pratish_Sreeja-G01354094_G01360679.pdf).

## Video Presentation

[Watch the project video](https://youtu.be/grzI3VPdG7M).
