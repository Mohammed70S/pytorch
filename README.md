Housing Price Prediction using Artificial Neural Network

Objective
The objective of this project is to predict housing prices based on a set of features such as area, road access, availability of a guest room, and other factors. We use an Artificial Neural Network (ANN) implemented in PyTorch to model the relationship between these features and housing prices. The model is trained to minimize the prediction error and is evaluated based on metrics such as Mean Absolute Error (MAE) and R-squared (R²).

Dataset Description
The dataset used in this project is from the file Housing-1.xlsx. It includes several features that influence house prices. These features include:

mainroad: Access to a main road (yes/no)
guestroom: Availability of a guest room (yes/no)
basement: Presence of a basement (yes/no)
hotwaterheating: Availability of hot water heating (yes/no)
airconditioning: Availability of air conditioning (yes/no)
prefarea: Whether the house is in a preferred area (yes/no)
furnishingstatus: The furnishing status of the house (semi-furnished, furnished, or unfurnished)
price: The target variable representing the price of the house.
The 'Yes/No' categorical features are converted into binary values (1/0), and the furnishingstatus is one-hot encoded. The dataset is split into training and testing sets, with 80% of the data used for training and 20% for testing.

Steps to Run the Code in Google Colab
Step 1: Upload your dataset
Place your dataset (Housing-1.xlsx) in your Google Drive and load it into your Colab environment.
Step 2: Install Dependencies
In the Google Colab environment, PyTorch, pandas, scikit-learn, and Matplotlib are pre-installed. If you are using a local environment or a different platform, install the required libraries using the following commands:

bash
Copy code
!pip install torch pandas scikit-learn matplotlib
Step 3: Clone or Download the Repository
Download this code as a ZIP file or clone it using Git:

bash
Copy code
git clone <repository-url>
Step 4: Upload the code and dataset to Colab
Upload the code file and dataset into your Colab workspace or link your Google Drive where the dataset is stored.

Step 5: Run the code
Execute the Python script by running each cell step-by-step in Colab:

Load the libraries and dataset
Preprocess the data
Define and train the ANN model
Evaluate the model on the test data
Plot the actual vs predicted prices
Step 6: Save and Download Results
Once the code finishes running, it will save the actual vs. predicted prices plot as actual_vs_predicted_prices.png in your environment. You can download this file for further analysis.

Dependencies and Installation Instructions
PyTorch: For building and training the ANN model
Pandas: For data manipulation and loading the dataset
scikit-learn: For data preprocessing (Standardization, train-test split, and evaluation metrics)
Matplotlib: For visualization
OpenPyXL: For reading .xlsx files (required by pandas)
Install all necessary packages in your environment using:

bash
Copy code
pip install torch pandas scikit-learn matplotlib openpyxl
Python Version
Ensure Python version 3.x is installed.
Colab Environment
If running on Google Colab, no further installation is necessary for the mentioned dependencies. Simply upload the dataset and execute the code.
