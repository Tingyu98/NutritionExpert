# Computer Vision Nutrition Tracker

## Overview 
In today's fast-paced world, maintaining a healthy diet has become increasingly challenging. NutritionExpert leverages **YOLOv8**, the **CalorieNinjas API**, **OpenAI GPT-4**, and **Streamlit** to deliver a user-friendly platform for real-time meal analysis and personalized diet planning. The system detects food items in uploaded images, extracts detailed nutritional information, and generates tailored diet plans using AI.

## Goal 
* Detect and classify food items in real time from meal images.
* Provide detailed nutrition insights including calorie counts and macronutrient breakdowns.
* Support personalized diet planning through AI-powered recommendations.

## Methodology
* Dataset Selection– UECFOOD-256 and School Lunch datasets (276 categories; 65 classes used for training). http://foodcam.mobi/dataset.html
* Data Preprocessing – Converted annotations to YOLO format, normalized images, and split data (Train:Val = 9:1).
* Model Training – Used YOLOv8, exploring different hyperparameters (epochs, learning rate, data split).
* Evaluation – Measured model performance using mAP (mean Average Precision) and precision-recall curves.
* Integration – Linked detection results with CalorieNinjas API for nutrition info and Streamlit for a user-friendly interface.
* Diet Planning – Integrated GPT-4 via OpenAI API to provide personalized meal recommendations.
  
## Results & Insights
* Detection Accuracy: YOLOv8 achieved mAP ≈ 73% on the combined UECFOOD-256 and School Lunch datasets.
* Bounding Box Quality: Most food items were labeled correctly with accurate bounding boxes. However, items partially cut off at image edges were more error-prone.
* Training Improvements: Increasing epochs (10 → 20) reduced validation and loss values, improving model stability.
* Precision-Recall Curve: Indicated precision above 0.7 across many classes, but recall decreased for underrepresented categories.
* User Impact: Integration with CalorieNinjas API ensured each detection came with real nutritional data, making the system actionable beyond classification.
* 
### Example Food Detection
<img width="687" height="459" alt="bee40815-e974-40f6-bd99-1fb5a27d3bca" src="https://github.com/user-attachments/assets/de96ab71-c7b4-4f20-ad19-693c4b8fbd5e" />

## Application
* Personal Use – Track meals, calories, and macronutrients.
* Healthcare & Fitness – Assist dietitians/trainers in monitoring diets.
* Food Industry – Enable smart canteens, nutrition tracking apps, and wellness platforms.

## Future Work
* Larger Datasets – Expand categories beyond Japanese/School Lunch food.
* Balanced Data – Address class imbalance for underrepresented food types.
* Weight Measurement – Incorporate methods to estimate portion size, volume, and weight.
* Deployment – Package into a mobile application for real-time usage.




