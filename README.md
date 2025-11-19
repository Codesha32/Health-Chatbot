# Health Chatbot

A Python-based chatbot that performs basic symptom analysis and disease prediction using machine learning. 

## Overview

This chatbot leverages natural language processing and a Random Forest classifier to:
- Extract symptoms from user descriptions.
- Predict potential diseases with associated confidence scores.
- Offer general descriptions, precautions, and self-care tips for predicted conditions.

## Requirements

- Python 3.6 or higher
- Required libraries: `pandas`, `numpy`, `scikit-learn`

Install dependencies via pip:
```
pip install pandas numpy scikit-learn
```

## Setup

1. Clone or download the repository.
2. Place the following CSV files in the specified directories:
   - `Training.csv` and `Testing.csv` in the `/Data/` folder.
   - Description, severity, and precaution CSV files in the `/MasterData/` folder.
3. Launch the chatbot:
   ```
   python Health_Chatbot.py
   ```

## Usage

Interact with the chatbot through a simple command-line interface:

1. **Provide basic information**: Enter your name, age, and gender when prompted.
2. **Describe your symptoms**: Input a natural language description (e.g., "I have a fever, cough, and fatigue").
3. **Respond to follow-ups**: Answer any clarifying questions to refine symptom extraction.
4. **Receive results**: View the predicted disease(s) with confidence levels, along with relevant descriptions, precautions, and tips.

Example interaction:
```
Bot: Hello! What's your name?
User: Alice
Bot: How old are you?
User: 28
Bot: What's your gender?
User: Female
Bot: Describe your symptoms.
User: Headache and nausea
Bot: [Processes and outputs prediction, e.g., "Possible Migraine (85% confidence). Precautions: Rest in a dark room..."]
```
