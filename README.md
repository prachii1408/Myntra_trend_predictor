# Myntra_trend_predictor
This is a model trained on deepfashion dataset to analyse the type of outfit in an image

## Overview 
In the fast-paced world of fashion, the allure of celebrity style is irresistible. The glamorous outfits seen in movies, TV series, and social media posts captivate audiences, making many aspire to emulate their favourite stars. Whether it's the iconic dress worn by a leading actress in a blockbuster film or the effortlessly chic outfit of a TV character, celebrities set the trends that millions seek to follow.

## Objective 
In the competitive landscape of fashion and entertainment, staying ahead of trends is crucial. Our objective is to gather posters of top trending movies and web series before their actual release, enabling us to anticipate and capitalize on emerging fashion trends inspired by these media. By feeding these posters into a machine learning (ML) model, we can predict the types of outfits present, which can then be used to inform fashion collections and marketing strategies.

## Trend Prediction 
•	We start by gathering data on trending movies and web series from the TMDB API. The posters, trailers, and teasers of the top three movies are saved into our database

•	To achieve this, we use a pre-trained ResNet34 model and train it on the DeepFashion dataset for outfit class recognition. This model identifies the general class of outfits. 

•	Next, to gain deeper insights from the posters, we use another ResNet34 model trained on the DeepFashion dataset for outfit type recognition. This model analyzes patterns on outfits, such as striped, floral, or printed designs.

•	With our models ready, we fed the data into them to detect the outfit class and type. Once the labels were obtained, they were sent to the Myntra MUSE app via a Flask API, ensuring smooth data transfer. Myntra MUSE then matches these predicted tags with actual tags on clothing items in its catalog, providing accurate recommendations.

#Results


