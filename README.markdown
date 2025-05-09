# Analysis of Factors Influencing the Box-Office Success of Films

[![Python Version](https://img.shields.io/badge/python-3.8-blue.svg)](https://www.python.org/downloads/release/python-380/)

## Project Description
This project investigates the key factors driving the box-office success of films. Using a dataset of 3,201 films from 2010 and earlier, the analysis explores how release dates, genres, IMDb and Rotten Tomatoes ratings, and production budgets influence financial performance. Through data cleaning, statistical analysis, and visualizations, the project uncovers actionable insights into movie industry trends.

## Objectives
- **Identify seasonal trends** in movie releases by genre.
- **Examine the relationship** between movie ratings and box-office success.
- **Analyze the impact** of production budgets on financial outcomes.

## Data Source
The dataset is sourced from publicly available film industry databases and includes:
- Movie titles
- Genres
- US and worldwide gross revenues
- IMDb and Rotten Tomatoes ratings
- Production budgets
- Release dates
- Additional attributes like MPAA ratings and distributors

## Methodology
The analysis was performed using Python with the following libraries:
- **Pandas**: For data manipulation and cleaning.
- **Matplotlib and Seaborn**: For generating visualizations.

The project is divided into three analytical sections:
1. **Release Date Analysis**: Exploring how genres are distributed across release months.
2. **Ratings vs. Success**: Investigating correlations between ratings and box-office revenues.
3. **Budget vs. Success**: Assessing the relationship between production budgets and financial performance.

Data cleaning involved handling missing values (replaced with means or "Unknown") and removing columns with excessive missing data. Visualizations include count plots, line plots, scatter plots with regression lines, and bar plots.

## Key Findings
- **Release Date Insights**: Action and Adventure films dominate summer releases, while family-oriented and holiday-themed movies peak in December, aligning with higher box-office revenues during these periods.
- **Ratings Impact**: Films with moderate IMDb ratings (6–7) and Rotten Tomatoes scores (70–80%) tend to achieve higher revenues, likely due to broader audience appeal.
- **Budget Correlation**: Higher production budgets (especially over $100M) strongly correlate with higher box-office revenues, though mid-budget films ($10M–$50M) also perform well, suggesting other factors like marketing and quality play a role.

## Visualizations

### 1. Release Date Insights
Action and Adventure films dominate summer releases, while family-oriented and holiday-themed movies peak in December. This alignment with seasonal demand contributes to higher box-office revenues during these periods.

![Number of Films Released per Month by Genre](visualization/number_of_movies_released_by_month_and_genre.png)
*Figure 1: Distribution of film releases by month and genre.*

![Average Worldwide Gross by Release Month](images/line_plot.png)
*Figure 2: Average box office revenue for films released in each month.*

### 2. Ratings Impact
Films with moderate IMDb ratings (6–7) and Rotten Tomatoes scores (70–80%) tend to achieve higher revenues, likely due to broader audience appeal. Very high or very low ratings do not consistently correlate with high earnings.

![IMDb Rating vs. Worldwide Gross](images/scatter_imdb.png)
*Figure 3: Relationship between IMDb ratings and box office success.*

![Rotten Tomatoes Rating vs. Worldwide Gross](images/scatter_rt.png)
*Figure 4: Correlation between Rotten Tomatoes ratings and financial performance.*

### 3. Budget Correlation
Higher production budgets, especially over $100M, strongly correlate with higher box-office revenues. However, mid-budget films ($10M–$50M) also perform well, indicating that other factors like marketing and quality play significant roles.

![Average Box Office Revenue by Budget Category](images/bar_budget.png)
*Figure 5: Comparison of average revenue across different production budget categories.*

![Production Budget vs. Worldwide Gross](images/scatter_budget.png)
*Figure 6: Positive correlation between production budgets and box office revenues.*

## Code
The analysis is implemented in the IPython notebook `Untitled1.ipynb`, available in this repository. The notebook includes:
- Data loading and cleaning.
- Code for all visualizations.
- Analysis of release dates, ratings, and budgets.

### How to Run the Notebook
1. Clone this repository to your local machine.
2. Install the required Python libraries:
   ```bash
   pip install pandas matplotlib seaborn
   ```
3. Open `Untitled1.ipynb` in Jupyter Notebook or Google Colab.
4. Run all cells to reproduce the analysis and visualizations.

## Contributors
- A K M Rezaul Hoque

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
