# Recommender Systems Class - Project 2: Neural Network Hotel Room Recommender
### author: Dominik Mikołajczyk

The tasks given in this project:
- preprocess the data
- bucket important features to reduce the offer space size
- define user features based on reservations
- prepare numerical item features
- code fit and recommend function in neural network recommender class
- tune different NN models to find the best parameters which will improve model's score
- run the final evaluation of each NN model and present the results against the Amazon and Netflix recommender's results

## Requirements:
1. Install jupyter:
    <!-- -->
    
        pip install jupyter
        
2. Install other required python libraries:
    <!-- -->
    
        pip install numpy==1.20.1
        pip install pandas==1.2.3
        pip install scikit-learn==0.24.1
        pip install torch=1.8.0
        pip install hyperopt==0.2.7
        pip install livelossplot=0.5.5
        
* Alternatively if you have Anaconda installed, you can configure enviroment using conda command:
    <!-- -->
    
        conda env create --name rs-class-env -f environment.yml conda activate rs-class-env
        
## Dataset
- [original dataset](https://github.com/ShakinBruno/recommender-systems-class-project-2/blob/main/hotel_data/hotel_data_original.csv)

![image](https://user-images.githubusercontent.com/71774757/236560653-7c5fa218-282e-4887-9b58-7634e409956e.png)

- [preprocessed dataset](https://github.com/ShakinBruno/recommender-systems-class-project-2/blob/main/hotel_data/hotel_data_interactions_df.csv)

![image](https://user-images.githubusercontent.com/71774757/236560973-f847f14c-7bfd-4ba7-b917-188cb147c0a3.png)

## Results

![image](https://github.com/ShakinBruno/recommender-systems-class-project-2/assets/71774757/1fafd043-70f0-4432-8d6f-33e32bcef5ef)

My Neural Network recommender is based on General Matrix Factorization model (GMF). I was not able to beat Amazon Recommender nor Netflix Recommender.
