# Cinema Audience Forecasting

A machine learning project for forecasting cinema audience attendance using historical booking, theater, date, and visit data from a Kaggle competition.

## Problem Statement

The objective of this competition is to **predict the number of cinema visitors for a given theater and date** based on historical audience and booking information.

The challenge involves identifying temporal patterns, theater-level trends, and booking behavior to build a model capable of generating accurate audience forecasts.

## Dataset

The project uses multiple datasets containing cinema visit, booking, theater, and date information.

### Files Used

* `booknow_visits.csv` — Historical cinema visit data
* `booknow_booking.csv` — BookNow booking information
* `cinePOS_booking.csv` — Cinema POS booking information
* `movie_theater_id_relation.csv` — Mapping between movie and theater identifiers
* `booknow_theaters.csv` — BookNow theater information
* `cinePOS_theaters.csv` — Cinema POS theater information
* `date_info.csv` — Date and calendar information
* `sample_submission.csv` — Submission format

## Approach

The project follows a structured machine learning workflow:

1. **Data Cleaning**

   * Handling missing values
   * Converting date fields
   * Removing inconsistencies
   * Preparing datasets for modeling

2. **Feature Engineering**

   * Date-based features
   * Day-of-week features
   * Historical visit patterns
   * Lag features
   * Rolling statistics
   * Booking trends
   * Theater-level historical features

3. **Model Development**

   * LightGBM
   * CatBoost
   * Random Forest

4. **Model Evaluation**

   * Models were evaluated using the competition's Kaggle evaluation metric.
   * Multiple feature-engineering strategies were tested to improve leaderboard performance.

## Results

The initial modeling approach achieved a **Kaggle leaderboard score of 0.27**.

Further experiments were performed using:

* Lag-based features
* Rolling-window statistics
* Historical booking trends
* LightGBM
* CatBoost

## Tech Stack

| Category         | Tools                            |
| ---------------- | -------------------------------- |
| Language         | Python                           |
| Data Processing  | Pandas, NumPy                    |
| Machine Learning | LightGBM, CatBoost, Scikit-learn |
| Visualization    | Matplotlib                       |
| Environment      | Google Colab, Kaggle             |
| Competition      | Kaggle                           |

## Project Structure

```text
cinema-audience-forecasting/
│
├── cinema_forecasting.ipynb
├── README.md
└── requirements.txt
```

## Notebook

The complete data preprocessing, feature engineering, model training, evaluation, and prediction workflow is available in:

**`cinema_forecasting.ipynb`**

## Kaggle

This project was developed as part of a Kaggle cinema audience forecasting competition.

The notebook contains the experiments and modeling workflow used to develop the final predictions.

## Future Improvements

Potential improvements include:

* More advanced temporal feature engineering
* Theater-specific forecasting models
* Hyperparameter optimization
* Ensemble modeling
* More sophisticated time-series approaches
* Improved handling of sparse booking patterns

## Author

**Yaswanth Vaddi**

Mechanical Engineering & Data Science
