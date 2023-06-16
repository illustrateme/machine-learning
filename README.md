# Machine Learning

## Recommendation Systems Tensorflow
Recommendation Systems This is a workshop on using Machine Learning and Deep Learning Techniques to build Recommendation systems Tensorflow  

**Theory:** ML &amp; Deep Learning, TensorFlow, TensorFlow Recommenders

**Paradigms:** Content-Based filtering, Collaborative filtering, Knowledge-based

**Data:** Illustrator Fiverr

**Models:**  TensorFlow Recommenders (TFRS), Client Model, Item Model, Rating Model

**Methods:** Recommender, Ranking, Embeddings, Brute Force

**Process:** Setup, Embed, Train &amp; Predict, Test &amp; Improve

**Tools:** python-data-stack: tensorflow, tensorflow_recommenders, numpy, pandas, scikit learn, sklearn-learn, keras, string, typing, 

**Collecting Data:** Data Mining, Web Scrapping Python


## Daftar Isi

- [Project Overview](#project-overview)
<!-- - [Business Understanding](#business-understanding) -->
<!-- - [Description](#description) -->
- [Data Understanding](#data-understanding)
<!-- - [Data Preprocessing](#data-preprocessing)
- [Data Preparation](#data-preparation)
- [Modeling](#modeling)
- [Evaluation](#evaluation)
- [Kesimpulan](#kesimpulan)
- [Referensi](#referensi) -->

## Project Overview

Currently there are many requests for illustrations from various industries, for example the creative industry and social media. Therefore, the opportunity for an illustrator to sell his services is getting bigger. According to Mulyandi & Puspitasari’s journal (2018), the rapid progression of digital lifestyles where access to information and communication technology has reached more than 90% of Indonesia's population. The increase in the middle class is also an opportunity to develop the creative industry. Besides that, there are also many clients who want to look for illustration services according to their preferences, such as a certain illustration style, a certain theme or concept, or the preferred technique and color.
We plan to develop a product for illustrators to provide illustration services to clients. And prospective clients can look for illustration services through this product. This product provides recommendations to clients for the desired illustration based on the preferences given. This app is expected to help illustrators, especially freelancers, sell their services through the works they exhibit through this app.

Machine Learning: In order to aid clients in finding the suitable illustration services, we planned to build a content-based filtering model. The dataset required to build the model was scraped from Fiverr’s website with a total of 1686 rows. We built the model based on the TensorFlow Recommender System library. The model was trained on two embeddings, namely the client embeddings and the item embeddings which are the candidates for recommendation. Predictions were made by passing a query model to a BruteForce layer. We saved the model as a SavedModel format which was deployed in the machine learning API.

## Data Understanding

The dataset used in this project is a dataset taken from the Fiverr Website with the name `fiverr_data.csv` as the dataset used.

- **Place**

  **Tabel 1. Informasi Dataset fiverr_data.csv**

  | #   | Column       | Non-Null Count | Dtype   |
  | --- | ------------ | -------------- | ------- |
  | 0   | Place_Id     | 437 non-null   | int64   |
  | 1   | Place_Name   | 437 non-null   | object  |
  | 2   | Description  | 437 non-null   | object  |
  | 3   | Category     | 437 non-null   | object  |
  | 4   | City         | 437 non-null   | object  |
  | 5   | Price        | 437 non-null   | int64   |
  | 6   | Rating       | 437 non-null   | float64 |
  | 7   | Time_Minutes | 205 non-null   | float64 |
  | 8   | Coordinate   | 437 non-null   | object  |
  | 9   | Lat          | 437 non-null   | float64 |
  | 10  | Long         | 437 non-null   | float64 |

  fiverr_data.csv consists of 1686 rows and 9 columns as follows:

  - illustrator_name: user name of illustrator
  - gig_rating: collective rating by clients
  - gig_price_from: gig starting price in US$
  - gig_img_url: gig display image URL
  - gig_url: gig page URL
  - gig_design_type: "logos", "illustrations", "pattern designs", "fonts & typography"
  - gig_design_style: "minimalist", "hand drawn", "vintage", "3d", "modern", "realistic", "sketch", "cartoon", "pop art", "abstract", "anime", "line art", "typography", "font design", "calligraphy", "hand lettering"
  - client_origins: client's country of origin
  - client_names: clients' usernames
  - illustrator_origins: illustrator's country of origin
  - illustrator_response_times: illustrator response time in hour(s)



<!--

# Python Libraries 
Deep Recommender Libraries  
1.Tensorrec - Built on Tensorflow 
2.Spotlight - Built on PyTorch 
3.TFranking - Built on TensorFlow (Learning to Rank) 
Matrix Factorisation Based Libraries  
1.Implicit - Implicit Matrix Factorisation 
2.QMF - Implicit Matrix Factorisation 
3.Lightfm - For Hybrid Recommedations 
4.Surprise - Scikit-learn type api for traditional alogrithms 

Similarity Search Libraries  
1.Annoy - Approximate Nearest Neighbour 
2.NMSLib - kNN methods 
3.FAISS - Similarity search and clustering 

<!--
# Algorithms &amp; 
Approaches Collaborative Filtering for Implicit Feedback Datasets 

Bayesian Personalised Ranking for Implicit Data 

Logistic Matrix Factorisation 

Neural Network Matrix Factorisation 

Neural Collaborative Filtering 

Variational Autoencoders for Collaborative Filtering Evaluations Evaluating Recommendation Systems
-->
