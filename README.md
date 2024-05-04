# NutritionExpert

## Introduction: 
In today's fast-paced and busy world, maintaining a healthy diet has become increasingly challenging. We leveraged YOLOv8 trained on UECFOOD-256 and School Lunch datasets to empower NutritionExpert to accurately detect and categorize various food items within an uploaded meal image. Integration with CalorieNinjas API provides relevant nutritional analyses. The NutritionExpert web app powered by Streamlit also offers personalized dietary plans, furnishing users with real-time, reliable information tailored to their balanced diet needs.

## Problem statement: 
* Meal Analysis: To solve the problem of analyzing the Food256 dataset, the following methods will be applied
* Selecting the Desired Food Class: Selecting the desired food class helps narrow down the focus and allows for targeted training to achieve accurate results for the chosen food category.
* Data Preprocessing: Data preprocessing involves preparing the dataset for training, which includes tasks such as extracting annotation files and images, resizing images, and normalizing the values.
* Using yolov8 open-source method: Real-time performance and accurate detection capabilities. YOLOv8 divides the image into a grid and predicts bounding boxes and class probabilities directly on that grid.
* Data Training:  We split datasets into 80% for training, 10% for validation, and 10% for testing. The validation set helps in monitoring the model's performance during training and making any necessary adjustments. * Provide detailed nutritional information : Including detailed nutritional information in the analysis and results is important for a comprehensive understanding of the food items. This information includes calorie counts and other relevant nutritional details.

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




