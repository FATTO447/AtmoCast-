# AtmoCast-
AtmoCast is a smart weather app that turns NASA data into activity-based recommendations. It tells you not just if it will rain, but how suitable the weather is for your parade, hike, or stargazing. Get optimal timing, actionable insights, and alternative suggestions to plan your day confidently and safely.

🌤️ AtmoCast: Your Adventure, Weather-Optimized
AtmoCast is a smart weather forecasting application developed for the NASA Space Apps Hackathon 2025. It goes beyond standard forecasts to provide personalized, activity-based recommendations, helping you decide not just what the weather will be, but what you can do during your day.

🚀 The Challenge: "Will it rain on my parade?"
AtmoCast translates complex NASA Earth observation data into a tool that helps users make informed daily decisions. Standard weather apps only tell you if it might rain; AtmoCast tells you if it will impact your parade, hike, or stargazing session.

🌟 Why AtmoCast Matters
Enhances Safety: Prevents people from getting caught in unsafe weather during outdoor activities.
Promotes Well-being: Encourages healthier, more active lifestyles by making planning easier.
Reduces Uncertainty: Empowers users to plan confidently and make the most of their time.

✨ Key Features
Activity Suitability Score: Instant rating (e.g., "Excellent," "Good," "Poor") for your chosen activity.
Optimal Timing Suggestions: Recommends the best time of day based on forecast analysis.
Actionable Insights: Explains why the weather is or isn’t suitable.
Alternative Activity Recommendations: Suggests other great options if your chosen activity isn’t ideal.

🧠 Machine Learning Component
AtmoCast uses a machine learning model to predict activity suitability based on weather conditions.
Model Type: [e.g., RandomForestClassifier / XGBoost / Regression]
Features Used: Temperature, Humidity, Wind Speed, Cloud Cover, Precipitation, Visibility 
Adding : Weekends , holidays , seasons , month 
Target / Output: Activity suitability labels tailored to weather types, such as:
categoties : clear/sunny summer days
             cloudy days
            rainy or extreme weather conditions

Workflow:
Historical weather data is preprocessed and features engineered.
The model is trained and validated to predict suitability scores for activities.
Joblib saves the trained model for fast inference.
FastAPI serves predictions to Streamlit for user interaction.
This ensures real-time, actionable recommendations that reflect actual weather scenarios.

⚡ FastAPI + Streamlit + Joblib Integration
Joblib: Saves and loads the trained ML model for fast predictions.
FastAPI: Serves as the backend API, handling user inputs and returning model predictions.
Streamlit: Provides the interactive frontend, visualizing suitability scores, timing suggestions, and actionable insights.

Workflow:
User enters input on Streamlit UI.
Streamlit calls FastAPI endpoints.
FastAPI loads the model via Joblib and returns predictions.
Streamlit displays recommendations dynamically.

💻 Technology Stack
Data Analysis: Python (Pandas, NumPy, Scikit-learn) 
Backend : Java , framework(spring) 
Data Visualization: Matplotlib, Seaborn
Frontend Prototype: Streamlit, HTML, CSS, JavaScript
API: FastAPI
Model Serialization: Joblib
Design: Figma 

⚙ Setup and Installation
Clone the repository:
git clone https://github.com/FATTO447/AtmoCast-.git
cd AtmoCast-


Create and activate a virtual environment:
# Windows
python -m venv venv
.\venv\Scripts\activate

# macOS/Linux
python3 -m venv venv
source venv/bin/activate


Install dependencies:
pip install -r requirements.txt

Run the FastAPI backend:
uvicorn main:app --reload

Run the Streamlit frontend:
streamlit run app.py

🏆 NASA Space Apps Hackathon 2025
Challenge: Will it rain on my parade?

Team: AtmoCast

Members: 
Moataz Mohsan (AWS) 
Mohamed Nasser (BackEnd) 
Fawzya Said (FrontEnd) 
Omnia Mohamed (UI/UX Design) 
Fatma Badawy (Data Science And AI(ML)) 

📄 License
This project is licensed under the MIT License. See the LICENSE file for details.
https://disc.gsfc.nasa.gov/information/tools?title=OPeNDAP%20and%20GDS 
