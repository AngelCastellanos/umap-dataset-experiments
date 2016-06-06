# Filling the gap between users and goods through a FCA-based common representation space: Top-N Rec-ommendation Experimentation and Evaluation
=================================================================================

Results and specific detail used for the paper "Filling the gap between users and goods through a FCA-based common representation space: Top-N Rec-ommendation Experimentation and Evaluation" by [Ángel Castellanos](http://nlp.uned.es/~acastellanos/), [Ana García-Serrano](http://nlp.uned.es/web-nlp/index.php?option=com_content&view=article&id=11) and [Juan Cigarrán](http://nlp.uned.es/~juanci/)

## Dataset
For the experimentation we have made use of the dataset presented by [Abel et al. (2011)](http://fabianabel.de/papers/2011-wis-twitter-um-umap.pdf). The dataset includes Twitter information streams of more than 2.000 users have been crawled. The gathered tweets have been linked to the news articles appearing in them. To that end, more than 60 RSS feeds of prominent news media (e.g., BBC, CNN or New York Times among others) have been monitored and more than 77,000 news articles have been aggregated.

In order to enhance the item representation, thus expecting to improve the content-based recommendation process, each tweet and news report has been semantically enriched to identify topics and entities mentioned in them by means of the [Open Calais](http://www.opencalais.com/) service.

As remarked by [Abel et al. (2011)](http://fabianabel.de/papers/2011-wis-twitter-um-umap.pdf), the Twitter messages per user follow a power-law distribution: the majority of users published less than 100 messages and only a small fraction of users wrote more than 1.000 tweets. Consequently, a sample of 1,619 user, who posted at least 20 tweets, containing more than 2.3 million tweets was gener-ated by the authors of Abel et al. (2011). 


## Results

Results are named according to the different features and item types (as explained in the paper). For each approach, there are 5 different files, one per each of the folds generated in the Cross-Validation process.

[results/fca](https://github.com/AngelCastellanos/umap-dataset-experiments/tree/master/results/fca) includes the results for our FCA-based recommendation proposal

[results/state-of-the-art](https://github.com/AngelCastellanos/umap-dataset-experiments/tree/master/results/state-of-the-art) includes the results for the state-of-the-art approaches.

[results/umap-2011-approaches](https://github.com/AngelCastellanos/umap-dataset-experiments/tree/master/results/umap-2011-approaches) includes the results for the UMAP 2011 approaches (cosine, jaccard, pearson).


## Code

The baselines as well as the state-of-the-art approaches to which our FCA-based approach has been compared have been implemented with the help of MyMediaLite Recommender System Library proposed by Gantner et al. (2011):

[https://github.com/zenogantner/MyMediaLite](https://github.com/zenogantner/MyMediaLite)

