# ReServe

Webapp Link: https://reserve-louisljz.streamlit.app/

## Inspiration
I am inspired by the abundance of leftover food that often goes to waste. I believe it would be great to create a web application that utilizes artificial intelligence (AI) to capture photos of leftover food and suggest ways to repurpose them into delicious dishes.

## What it does
The web application allows users to either take a photo of their leftover food or manually input the food items. The computer vision component of the application recognizes the available food tags present in the images. The recognized food items are then sent to a natural language chatbot which suggests various ways to repurpose the leftover food.

## How we built it
We incorporated a computer vision model from the [Clarifai food recognition API](https://clarifai.com/clarifai/main/models/food-item-recognition) into our web application. Additionally, we utilized the natural language processing capabilities of the [PaLM 2 for Chat API](https://console.cloud.google.com/vertex-ai/publishers/google/model-garden/chat-bison?project=lablabai) to create the chatbot component. These two models were integrated and packaged together within a [Streamlit web application](https://reserve-louisljz.streamlit.app/).

## Challenges we ran into
One of the challenges we encountered was ensuring the secure protection of the API keys used in the web application. However, we were able to overcome this challenge by encrypting the API keys using Streamlit secrets in TOML format.

## Accomplishments that we're proud of
We are proud to have successfully deployed an AI-powered product that combines computer vision and natural language processing. Our web application provides a simple and user-friendly solution for repurposing leftover food, contributing to sustainability efforts.

## What we learned
Throughout this project, we gained experience in using Object-Oriented Programming (OOP) to create classes for the FoodRecognizer and Chatbot components. This allowed us to organize our code effectively within the web application. We also learned how to make API calls to Clarifai and Google Cloud Platform (GCP), as well as the importance of securely serving API keys in a Streamlit application.

## What's next for ReServe
In the future, we plan to enhance our web application, ReServe, by training a custom object detection model using the PyTorch framework. This will enable ReServe to recognize multiple food items simultaneously, overcoming the current limitation of only classifying one item at a time. We will train the model on the [Food Recognition Dataset](https://www.kaggle.com/datasets/sainikhileshreddy/food-recognition-2022) available on Kaggle, improving the accuracy of food recognition. 
