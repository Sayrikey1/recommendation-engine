# Movie Recommendation System

This project implements a movie recommendation system using collaborative filtering techniques. The system predicts user ratings for movies and recommends movies based on user preferences.

## Table of Contents

- [Movie Recommendation System](#movie-recommendation-system)
  - [Table of Contents](#table-of-contents)
  - [Installation](#installation)
  - [Usage](#usage)
    - [Example](#example)
  - [Project Structure](#project-structure)
  - [Contributing](#contributing)
  - [License](#license)

## Installation

To install the required dependencies, run the following command:

```bash
pip install -r requirements.txt
```

## Usage

1. **Load the Data**  
   Load the movie ratings and movie information datasets.

2. **Train the Model**  
   Train the collaborative filtering model using the provided datasets.

3. **Make Predictions**  
   Use the trained model to predict user ratings for movies.

4. **Get Recommendations**  
   Generate movie recommendations for a specific user.

### Example

```python
# Import necessary libraries
import pandas as pd
from sklearn.metrics.pairwise import cosine_similarity

# Load datasets
movies = pd.read_csv('movies.csv')
ratings = pd.read_csv('ratings.csv')

# Train the model and make predictions
user_predictions = train_model(ratings)

# Get recommendations for a specific user
user_id = 1
already_rated, recommendations = recommend_movies(user_predictions, user_id, movies, ratings, 10)

# Display recommendations
print(recommendations)
```

## Project Structure

```
.
├── data
│   ├── movies.csv
│   ├── ratings.csv
│   └── tags.csv
├── notebooks
│   ├── Build Recommendation Systems for Movies Like Netflix.ipynb
│   └── movie.ipynb
├── src
│   ├── model.py
│   └── utils.py
├── requirements.txt
└── README.md
```

## Contact 📧

- **Name**: Kamal Seriki
- **Email**: kamalseriki49@gmail.com
- **GitHub**: [Sayrikey1](https://github.com/Sayrikey1)
  
## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or bug fixes.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

