# AAMER: A Method For Extracting Aspect-Based Emotions From Online Product Reviews

We present our AAMER (Adaptable Aspect-based Multi Emotion Recognition) method for aspect-based emotion analysis of product reviews. AAMER focuses on addressing some shortcomings of previous aspect extraction and emotion analysis works by being adaptable to new datasets and will require no previous training data. The method can extract multiple emotion values towards a product aspect instead of a single polarity value. We test, and analyze results from 12 different variations of our method while using a new dataset of RC car reviews from amazon. The emotions we will detect will be fear, anger, anticipation, trust, surprise, generally positive, generally negative, sadness, disgust, and joy.

By doing so we hope to give users of the tool a better overview of how certain features of a product impacted the experience of that product more so than they may get from simply looking at a rating or trying to read many long reviews.


## Requirements
- [NLTK]( https://www.nltk.org/)
- [Scapy](https://scapy.net/)
- Standard scientific libraries like Numpy and matplotlib are also required.
## How to use
The data comes preprocessed in this repo so that it can be used directly with the notebooks. The review data is in the `dataset/top_car_reviews.pkl` file. Each notebook is used for a certain task in the project and must be run in the following order
1. `Feature extraction.ipynb`: This notebook will extract the features for each product using both a heuristic and rule based approach. These product features are then stored in files.
 
2. `Emotion detection.ipynb`: This notebook will calculate the emotion felt towards each feature of a product across all its reviews using two different averaging methods.  
3. `Emotion analysis.ipynb`: This notebook will compare the results from the different methods used (see report paper for more details about methods) and will also visualise emotion felt towards each feature of a product in bar charts. 

