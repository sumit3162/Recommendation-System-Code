# Recommendation System with Collaborative Filtering

## Overview

This project implements a basic recommendation system using collaborative filtering with Non-negative Matrix Factorization (NMF). The system analyzes user-item ratings to predict and recommend items that users might like based on their past preferences.

## Features

- **Matrix Factorization**: Uses NMF to decompose the user-item ratings matrix into latent features
- **Personalized Recommendations**: Generates recommendations specific to each user
- **Exclusion of Rated Items**: Only recommends items the user hasn't already rated

## Requirements

- Python 3.x
- NumPy
- pandas
- scikit-learn

## Installation

1. Clone the repository:
   ```bash
   git clone [repository-url]
   cd recommendation-system
   ```

2. Install the required packages:
   ```bash
   pip install numpy pandas scikit-learn
   ```

## Usage

1. Prepare your user-item ratings data in the same format as the example:
   ```python
   ratings = {
       'User1': [5, 3, 0, 1],
       'User2': [4, 0, 0, 1],
       # ... more users
   }
   ```

2. Run the recommendation system:
   ```python
   # The system will output recommendations for each user
   print("Recommendations for User1:", recommend_movies(0))
   ```

## Example Output

For the sample data provided, the output will be:
```
Recommendations for User1: ['Movie3']
```

## Customization

- Adjust the number of latent features by changing `n_components` in the NMF model
- Change the number of recommendations by modifying the `n_recommendations` parameter
- Replace the sample data with your own user-item ratings matrix

## Future Improvements

- Implement cross-validation for model evaluation
- Add hybrid recommendation approaches combining content-based filtering
- Develop a proper evaluation metric to assess recommendation quality
- Scale the system for larger datasets

## License

This project is open-source and available under the MIT License.

---
