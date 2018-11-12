# Job offer recommender prototype

This project consists on a prototype for a job offer recommendation system.

A clustering model is trained using a data set (named *skills* data set). The features of the
model are the words that appear in the skills of each offer (one-hot encoded). Then, all
the offers of another data set (named *offers* data set) are clustered. Finally, the prototype
asks the user for a list of skills and returns a list of the most similar offers from those in
the second data set.

## Files

The project contain the following files:

- **eda.ipynb**	Jupyter notebook with exploratory data analysis of the given datasets.
- **recommender.ipynb** Jupyter notebook with a prototype of recommendation application.
- **parse_offers_file.ipynb** Jupyter notebook with code to process the "candidatetest_df_off.csv" file.

The data files should be located in the **data** folder for the code to run properly.

## Settings

The options that can be set in the **recommender** notebook are:

- `FILE_SKILLS` Path of the CSV file containing the skills data set.
- `FILE_OFFERS` Path of the CSV file containing the offers data set.
- `PATTERNS_BEGINNING` Patterns to remove from the beginning of the skills.
- `PATTERNS_END` Patterns to remove from the end of the skills
- `NUMBER_OF_CATEGORIES` Number of words used for the feature engineering.
- `NUMBER_OF_CLUSTERS` Number of clusters.
- `NUMBER_OF_SIMILAR_OFFERS` Number of different offers to display.
