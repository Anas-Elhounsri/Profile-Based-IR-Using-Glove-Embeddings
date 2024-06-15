# Profile Based Information Retrieval With GloVe Embedding:

This is a small information reteival project, where we generate 5 sets of users that have different interests in different categories of news, and using GloVe for word embedding, we trained two models (SVM and Random Forest) for classification, the script takes an input of corpus of an article, and determines which users would like the given article after classifying it.

The data processing and the results of the evaluation for both models are in the notebook as well. The dataset was obtained from [Kaggle](https://www.kaggle.com/datasets/sunilthite/text-document-classification-dataset?resource=download)

I used Google Colab when making this script (you can use Jupyter but you will have to upload the dataset and glove file to the notebook), so to use it:

## Data and Preprocessing
- Upload your data: Upload the dataset file (e.g., dataset.csv) containing news articles and their categories to your Google Drive.
- Specify Path: In your code, define the path to the dataset.csv file within your mounted Drive for example: 
  
  ```python
  path = "/content/drive/your/path/dataset.csv"
  
## GloVe Word Embeddings
- Download Pre-trained Model: Since we're using a pre-trained Glove model, navigate to [Standford university GloVe project repository](https://nlp.stanford.edu/projects/glove/) and download the appropriate Glove model file (In my case I used glove.6B.zip).

- Upload to Drive: Upload the downloaded glove.6B.zip file to the same location in your Google Drive where you uploaded the dataset.

- Specify Path: In your code, define the path to the downloaded glove.6B.zip file within your mounted Drive: 
```bash
!unzip /content/drive/your/path/glove.6B.zip
```

This project offers a starting point to learn about information retieval. There is still plenty room to explore further by:

- Training our own GloVe instead of implementing a pretrained one.
- Implementing additional features.
- Experimenting with different classification algorithms.
- Using a larger and more comprehensive dataset.
