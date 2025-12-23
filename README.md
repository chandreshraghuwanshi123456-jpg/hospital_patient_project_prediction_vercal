🏥 Hospital Patient Risk Prediction System
A full-stack machine learning application that predicts patient health risks based on vitals using a Random Forest classifier. This project features a decoupled architecture with a FastAPI backend and a Streamlit frontend.

🚀 Live Demo
Frontend UI: [Paste your Streamlit Link Here]

API Documentation (Swagger): https://hospitalpatientprojectpredictionver-amber.vercel.app/docs

🛠️ Tech Stack
Machine Learning: Scikit-Learn (Random Forest Classifier)

Backend API: FastAPI (Python)

Frontend UI: Streamlit

Deployment: Vercel (Backend), Streamlit Cloud (Frontend)

Communication: REST API via requests library

💡 Key Features
Real-time Inference: Users can adjust patient parameters (Age, BMI) and receive an instant risk assessment.

Serverless Backend: Optimized the API environment to stay within Vercel's 250MB deployment limit.

Decoupled Architecture: The frontend and backend are hosted separately, allowing for independent scaling and maintenance.

Interactive UI: A user-friendly dashboard designed for healthcare professionals to visualize model output.

🏗️ How it Works
The Brain: A Random Forest model was trained on patient data and exported as a model.pkl file.

The Engine: The FastAPI server loads the pickle file and listens for POST requests at the /predict endpoint.

The Face: The Streamlit app takes user input, packages it into a JSON payload, and sends it to the Vercel-hosted API.

The Result: The API returns a prediction (0 or 1), which the UI displays as "Low Risk" (Success) or "High Risk" (Warning).

📂 Project Structure
app.py: Streamlit frontend code.

main.py: FastAPI backend code.

model.pkl: The trained Random Forest model.

requirements.txt: Unified dependency list for both cloud platforms.

data.json: Local storage for patient records (demonstrating CRUD functionality).

🙏 Acknowledgments
Special thanks to my instructors at Sherians Coding School, Tanishq Vyas and Akarsh Vyas, for the training and support in building production-ready AI applications.
