Team-6:
- Raghavendra Devineni-21072747
- Charan Sai Prakash-21071658
- Sai Krishna Reddy Nanduri-21078449
- Syam Sundar Boina-21061898
- Akhil Kumar Matala-21073209

Features:
- PassengerId: A unique Id for each passenger. Each Id takes the form gggg_pp where gggg indicates a group the passenger is travelling with and pp is their number within the group. People in a group are often family members, but not always.
- HomePlanet: The planet the passenger departed from, typically their planet of permanent residence.
- Age: Age of the passenger.
- VIP: Whether the passenger is a VIP.
- CryoSleep: Indicates if the passenger is in cryo-sleep.
- Cabin - The cabin number where the passenger is staying. Takes the form deck/num/side, where side can be either P for Port or S for Starboard.
- Deck: Deck of the ship where the passenger is located.
- Destination: Intended destination of the passenger.
- RoomService, FoodCourt, ShoppingMall, Spa, VRDeck - Amount the passenger has billed at each of the Spaceship Titanic's many luxury amenities.
- Name - The first and last names of the passenger.
- Transported - Whether the passenger was transported to another dimension. This is the target, the column you are trying to predict.

 Data Preprocessing:
- Handle missing values using Iterative Imputer and group-based imputation.
- Analyze group consistency for specific columns like HomePlanet, Destination, and Cabin.
- Predict missing values using RandomForestClassifier.
- Perform one-hot encoding for categorical variables.

Model Building:
- Utilize RandomForestClassifier for initial predictions.
- Implement a neural network using TensorFlow/Keras for comparison.
- Evaluate model performance using accuracy metrics.
- Save the model and make predictions on the test dataset.

Files:
- kaggle_machine_lrnmodel.ipynb: Google Colab containing the code for data preprocessing, model building, and evaluation.
- train.csv: Training dataset.
- test.csv: Test dataset.
- sample_submission.csv: Sample submission file for Kaggle competition.




 
