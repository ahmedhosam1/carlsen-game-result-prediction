🧠 Predicting Magnus Carlsen's Chess Game Results
📌 Project Overview

This project explores whether it is possible to predict the outcome of Magnus Carlsen’s chess games using basic game metadata and machine learning techniques.

The goal was not just to build a model, but to understand how feature quality affects model performance.

📊 Dataset

The dataset contains historical chess games with features such as:

Player color (White/Black)

Number of moves

Game format

Full move sequence

From the move sequence, I extracted the opening sequence (first two moves for each player) as a feature.

⚙️ Feature Engineering

Key features used:

player_color

num_moves

game_format

opening_sequence (extracted using regex from move list)

Categorical variables were encoded before training.

🤖 Model Used

Random Forest Classifier
Stratified Train/Test Split
Cross Validation applied for stability

📈 Results

Test Accuracy: ~69–70%
Cross Validation Mean Accuracy: ~68–70%
A baseline (Dummy Classifier) was also considered for comparison.

🔍 Key Insight

The model performance plateaued around 70%, even after multiple experiments.
This suggests:
The limitation was not model complexity.
The available features lacked strong predictive signal.
Chess outcomes depend heavily on deeper variables such as:
Rating difference
Engine evaluation
Blunders
Accuracy percentage

🎯 Conclusion

This project highlights an important machine learning lesson:
Model performance depends more on feature quality than model complexity.
Even strong models cannot compensate for weak or limited data signals.

🚀 Future Improvements

Add rating difference between players
Include engine evaluation scores
Include mistake/blunder counts
Try advanced feature selection

🛠 Tools Used

Python
Scikit-learn
Pandas
Matplotlib
Scikit-learn

Matplotlib
