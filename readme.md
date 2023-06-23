# Mental Health Prediction using Machine Learning Algorithms

This project focuses on predicting mental health conditions using various machine learning algorithms. We utilize the OSMI Kaggle dataset, which is a supervised dataset based on a tech survey.

## Data Flow

1. **Questionnaire**: Users are presented with a set of basic questions, which correspond to the columns in the dataset.
2. **Input**: Users can provide their answers either in voice or text format.
3. **Conversion**: The user's answers are converted into a numerical format, mapping "yes" to 1, "no" to -1, and "maybe" to 0. This conversion aligns with the format of the dataset.
4. **Model Evaluation**: The converted answers are then fed into different machine learning models to evaluate their accuracy. The model that performs best in this scenario is the Support Vector Machine (SVM).
5. **Model Persistence**: The trained SVM model is saved as a pickle file, allowing for quick inference without the need to re-run the entire process.
6. **Prediction**: Users can input their answers into the trained model to determine their mental health status.
   
## Training the Model

1. **Dataset Preparation**: The OSMI Kaggle dataset is obtained, and the "yes," "no," and "maybe" values are converted to 1, -1, and 0, respectively.
2. **Model Comparison**: Several machine learning models are applied to the prepared dataset, and their accuracies are measured. The SVM model is identified as the best-performing algorithm.
3. **Model Persistence**: The trained SVM model is serialized and stored as a pickle file, enabling easy and efficient usage.
4. **Inference**: By utilizing the pickle file, users can quickly obtain predictions regarding their mental health and receive recommendations for potential actions.

## Getting Started

To get started with this project, follow these steps:

1. Clone the repository: `git clone https://github.com/your-username/your-repo.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Install the frontend dependencies by doing: `cd frontend` and then `npm i`.
3. Run the project: `python main.py`
4. Follow the prompts or provide voice/text input when prompted.
5. Receive the prediction and recommended actions based on the trained SVM model.


## Paper Publication

First Paper is published in this journal: https://fzgxjckxxb.com/volume-23-issue-5-2023/