# Computer Vision Nutrition Tracker

## Overview 
In today's fast-paced world, maintaining a healthy diet has become increasingly challenging. NutritionExpert leverages **YOLOv8**, the **CalorieNinjas API**, **OpenAI GPT-4**, and **Streamlit** to deliver a user-friendly platform for real-time meal analysis and personalized diet planning. The system detects food items in uploaded images, extracts detailed nutritional information, and generates tailored diet plans using AI.

## Goal 
* Detect and classify food items in real time from meal images.
* Provide detailed nutrition insights including calorie counts and macronutrient breakdowns.
* Support personalized diet planning through AI-powered recommendations.

## Approach:
In order to address the challenge of personalized nutrition analysis and diet planning, we have incorporated three essential technologies: YOLOv8, Calorie Ninjas API, and Streamlit. These technologies collectively contribute to delivering a solution that is both precise and user-friendly.

* YOLOv8:
It segments the image into a grid and predicts bounding boxes and class probabilities directly on that grid. It is widely used in applications that require fast and precise object detection in real-time scenarios.

* Calorie Ninjas API:
The API clients application interacts with the Text Nutrition API by sending a GET request to its endpoint. The API utilizes its AI-powered algorithms to process the request and extract nutrition information. Once the data is extracted, it is formatted accordingly and sent back to the client as a JSON response, providing the required nutrition details.

* Streamlit:
Streamlit is an open-source Python library, with Streamlit, we create a multi-paged frontend that connects seamlessly with our backend APIs and the pre-trained YOLOv8 model. Allowing users to upload their plate, and view the analyzed results.

## Datasets:
UECFOOD-256 and School Lunch
http://foodcam.mobi/dataset.html 





