# From None to Severe: Predicting Intensity in Movie Scripts
<p align="right"><i>Authors: Yigeng Zhang, Mahsa Shafaei, Fabio Gonzalez and Thamar Solorio</i></p> 
This repository hosts the dataset and the source code of the paper *From None to Severe: Predicting Intensity in Movie Scripts*.
## Dataset
Please find the dataset through this link.
This zipfile contains train/dev/test files of 5 aspects of age-restricted content.
The data is formated in the following columns in a Pandas Dataframe:
```
id | Aspect | None | Mild | Moderate | Severe | Total_votes | Aspect_rating | text
```
## Code
Please find the code in the code folder.
### Dependency libraries
In this work, we use `Python 3.7.9`. The dependency libraries are with the following versions:
```bash
NumPy 1.18.5
Pandas 1.1.3
PyTorch 1.6.0
PyTorch Lightning 1.0.2
Scikit-learn 0.23.2
Sentence-transformers 0.4.1.2
```
### Use of the code
#### Sentence BERT embedding
Use the following command to embed all text into utterance-level sentence embeddings.
```bash
python text_embedding.py --data_dir your-save-path
```
The reason of obtaining and saving sentence embeddings beforehand is to reuse and save experiment time. Otherwise getting embeddings together with training will drastically increase running time.
#### Training and testing the model
Use the following command to run the training-test script with default settings.
```bash
python RNN-Trans_S-MT.py
python TextRCNN_S-MT.py
```
To test the code correctness without running the full training cycle, a fast dev run on a single batch is available using the following command:
```bash
python RNN-Trans_S-MT.py --dev_run
```
## Citation
If you would like to use our work and code for research, please cite our paper with the following info:
```
Coming soon
```
## Contact
Please contact `yzhang168@uh.edu` for questions.
