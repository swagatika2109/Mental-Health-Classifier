# PROJECT TITLE
Mental Health Classifier
# PROBLEM OVERVIEW
1. Manual classification of mental health phrases is time-consuming.
2. Human judgment is subjective and inconsistent.
3. Users express emotions in text (chats, journals) that are hard to analyze at scale.
4. Lack of automated tools to quickly identify stress, anxiety, motivation, or neutral states.
5. Need for a system that provides real-time, reliable classification for textual mental health insights.
# OBJECTIVES
1. Classify text into stress, anxiety, motivation, or neutral.
2. Provide real-time predictions with confidence scores.
3. Handle low-confidence inputs using fallback rules.
4. Enable automated analysis of mental health phrases.
# TOOLS AND TECNOLOGIES USED
1. Programming language-
 a. python3.10.11- Used to implement the Mental Health Classifier.
2. Python Libraries-
 a. pandas – For data handling and manipulation.
 b. scikit-learn – Machine learning library (TF-IDF, Logistic Regression, model training).
3. Machine Learning & NLP-
 a. TF-IDF Vectorization – Feature extraction from text.
4. Model Persistence-
 a. pickle – To save and load trained models and vectorizers.
5. Data Storage-
 a. CSV files – For storing dataset of mental health phrases.
6. Augentation and Processing-
 a. Data Augmentation Techniques – To expand dataset variations.
# REQUIREMENTS
1. Software Requirements-
  a. Python 3.10.11
  b. pandas
  c. scikit-learn
  d. pickle
  e. Command-Line Interface (CLI)
2. Hardware Requirements-
  a. Processor: 1.5 GHz or higher
  b. RAM: 4 GB minimum
  c. Storage: 100 MB (for code, dataset, and models)
3. Functional Requirements-
  a. Accept text input from user
   b. Classify into: stress, anxiety, motivation, neutral
   c. Show prediction with   confidence score
  d. Save/load trained model
  e. Handle low-confidence inputs using fallback rules
4. Non-Functional Requirements-
  a. Real-time predictions (<1 sec)
  b. Easy to use CLI
  c. Cross-platform portability
  d. Reliable predictions with fallback
  e. Scalable for larger datasets
# PROJECT MODULES
1. Dataset Module-
 a. Load mental health phrases from CSV.
 b. Augment dataset to increase variations.
2. Preprocessing Module-
 a. Clean and preprocess text.
Vectorize phrases using TF-IDF (unigrams + bigrams).
3. Model Training Module-
 a. Train Logistic Regression classifier with class balancing.
 b. Evaluate model using accuracy and classification metrics.
 c. Save trained model and vectorizer.
4. Prediction Module-
 a. Take user input and vectorize it.
 b. Predict category using trained model.
 c. Calculate confidence score.
5. Fallback Rules Module-
 a. Apply keyword-based rules for low-confidence predictions.
 b. Ensure robust classification for unknown or ambiguous phrases.
6. User Interaction Module-
 a. Command-Line Interface (CLI) for input and output.
 b. Loop until user exits.
# ALGORITHM
1. Start
2. Load dataset (mental_health_phrases.csv)
3. Augment dataset with variations (optional)
4. Vectorize text using TF-IDF (unigrams + bigrams)
5. Train Logistic Regression model with class balancing
6. Save model and vectorizer (.pkl)
7. For each user input:
 a. Transform input using vectorizer
 b. Predict class using the model
 c. If confidence < 0.5, apply fallback rules
 d. Display predicted category and confidence
8. Repeat until user exits
9. End
# HOW TO INSTALL AND RUN THE PROGRAM
1. Install Python (if not already installed)
2. Download or clone this project to your computer
3. Open a terminal or command prompt and navigate to the project folder
4. Run the program:python mental_health_app.py
5. Enter phrases when prompted:
   Type any sentence describing your mental state.
6. View the output:
The program will display:
->Predicted Category (stress, anxiety, motivation, neutral)
->Confidence Score
7. Exit the program:
   Type exit and press Enter
# INSTRUCTIONS FOR TESTING
1. Ensure mental_health_app.py and mental_health_phrases.csv are in the same folder.
2. Open terminal/command prompt and run:
   python mental_health_app.py
3. Enter sample phrases representing different categories: stress, anxiety, motivation, or neutral.
4. Verify the program outputs the predicted category and confidence score.
5. Test edge cases (unknown phrases, empty input) to check fallback rules.
# FUTURE ENHANCEMENT
1. Add web/mobile interface
2. Expand dataset
3. Use advanced NLP models
4. Support multiple languages
5. Add analytics and alerts
