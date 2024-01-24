# Multi-Class Hate Speech Classification using NoahBERT

## Abstract

In this project, we tackle the challenge of hate speech detection, specifically focusing on differentiating between hate speech, offensive language, and neutral content. We employ two models for comparison: the BERT NLP model, developed by Google in 2018, and our modified model, NoahBERT, designed for enhanced multi-speech classification.

Both models exhibit challenges in sensitivity to specific terms and difficulties in accurately interpreting the context of statements. However, our NoahBERT demonstrates a better grasp of distinguishing between offensive and hateful language in some instances. It shows potential improvement in differentiating between these two classes compared to BERT.

The implementation notebook is optimized for execution on Google Colab Pro with V100 High RAM.

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

For a detailed understanding of the project, please refer to the [report](Report-FinalProject-CS747DL-Pratish_Sreeja-G01354094_G01360679.pdf).

## Video Presentation

[Watch the project video](video_link.txt).
