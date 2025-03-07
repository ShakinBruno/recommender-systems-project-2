# Recommender Systems Class - Project 2: Neural Network Hotel Room Recommender

### Author: Dominik Mikołajczyk

## Project Overview

This project focuses on building a neural network-based recommender system for hotel rooms. The primary goal is to preprocess data, reduce the dimensionality of the offer space, define user and item features, and implement a neural network model that can effectively suggest hotel rooms to users based on their preferences and past interactions.

## Tasks

The tasks undertaken in this project include:

- **Data Preprocessing**: Clean and prepare the dataset for analysis.
- **Feature Bucketing**: Bucket important features to reduce the offer space size.
- **User Feature Definition**: Define user features based on reservation history.
- **Item Feature Preparation**: Prepare numerical item features for the recommendation model.
- **Recommender Implementation**: Code the `fit` and `recommend` functions in the neural network recommender class.
- **Model Tuning**: Tune different neural network models to find the best parameters that improve the model's performance.
- **Evaluation**: Run the final evaluation of each neural network model and present the results compared to the Amazon and Netflix recommender's results.

## Requirements

To run this project, you need to have the following software and libraries installed:

1. **Jupyter Notebook**: For running and interacting with the project notebooks.
    ```bash
    pip install jupyter
    ```

2. **Python Libraries**: Install the required Python libraries using pip.
    ```bash
    pip install numpy==1.20.1
    pip install pandas==1.2.3
    pip install scikit-learn==0.24.1
    pip install torch==1.8.0
    pip install hyperopt==0.2.7
    pip install livelossplot==0.5.5
    ```

Alternatively, if you have Anaconda installed, you can configure the environment using the conda command:
```bash
conda env create --name rs-class-env -f environment.yml
conda activate rs-class-env
```

## Dataset

The project uses two main datasets:

- **Original Dataset**: [Download here](https://github.com/ShakinBruno/recommender-systems-class-project-2/blob/main/hotel_data/hotel_data_original.csv)

  ![Original Dataset](https://user-images.githubusercontent.com/71774757/236560653-7c5fa218-282e-4887-9b58-7634e409956e.png)

- **Preprocessed Dataset**: [Download here](https://github.com/ShakinBruno/recommender-systems-class-project-2/blob/main/hotel_data/hotel_data_interactions_df.csv)

  ![Preprocessed Dataset](https://user-images.githubusercontent.com/71774757/236560973-f847f14c-7bfd-4ba7-b917-188cb147c0a3.png)

## Implementation Details

The project includes several key components:

- **Data Preprocessing Toolkit**: Functions for cleaning and transforming the dataset, such as summing people counts, filtering data, and mapping features to buckets.
- **Neural Network Model**: Implementation of a neural network recommender model based on General Matrix Factorization (GMF).
- **Feature Engineering**: Methods for defining and extracting user and item features from the dataset.
- **Evaluation**: Scripts for evaluating the performance of the recommender models using metrics like HR@10 and NDCG.

## Results

The neural network recommender, based on the GMF model, was evaluated against the Amazon and Netflix recommenders. While it did not outperform these benchmarks, the project provided valuable insights into the application of neural networks in recommendation systems.

![Results](https://github.com/ShakinBruno/recommender-systems-class-project-2/assets/71774757/1fafd043-70f0-4432-8d6f-33e32bcef5ef)

## Conclusion

This project demonstrates the potential of neural network-based recommendation systems in the context of hotel room recommendations. Despite not surpassing existing benchmarks, the project highlights areas for further exploration and improvement.
