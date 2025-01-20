### Exploratory Data Analysis of Udemy Sales Trends

This repository contains an exploratory data analysis (EDA) project on sales and popularity trends of courses available on Udemy. The analysis leverages a dataset of 10,000 business-related courses to uncover insights such as course popularity, pricing strategies, and subscriber trends.

---

#### Features

1. **Dataset Overview**:
   - The dataset includes features like course title, URL, number of subscribers, ratings, reviews, pricing details, and publication dates.
   - Initial exploration reveals key attributes such as `num_subscribers`, `avg_rating`, `discount_price__amount`, and more.

2. **Preprocessing**:
   - Handled missing values in `discount_price__amount` by replacing them with `0`.
   - Removed irrelevant columns such as `url`, `is_paid`, and `is_wishlisted` to focus on meaningful analysis.

3. **Correlation Analysis**:
   - Found a perfect correlation (1.0) between `avg_rating_recent` and `rating`, indicating duplicate information.
   - Highlighted a strong positive correlation (0.79) between `num_reviews` and `num_subscribers`.

4. **Key Insights**:
   - Courses with discounts attract significantly more subscribers.
   - Courses with higher numbers of reviews tend to have higher subscriber counts.
   - Monthly trends in course publishing and subscriber acquisition were analyzed.

5. **Visualizations**:
   - Correlation heatmaps.
   - Distribution of subscribers for discounted and non-discounted courses.
   - Top 10 courses by subscriber count.
   - Monthly subscriber trends.

---

#### Dataset
The dataset used in this project contains 10,000 entries of business courses scraped from Udemy. Key features include:
- **`title`**: Course name.
- **`num_subscribers`**: Total number of students enrolled.
- **`avg_rating`** and **`avg_rating_recent`**: Ratings for the course overall and recently.
- **`num_reviews`**: Count of user reviews.
- **`discount_price__amount`** and **`price_detail__amount`**: Discounted and original prices of the courses.

---

#### Setup Instructions

1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. Install required libraries:
   ```bash
   pip install pandas matplotlib seaborn scipy
   ```

3. Place the dataset (`udemy_output_All_Business_p1_p626.csv`) in the project directory.

4. Run the script to generate insights and visualizations:
   ```bash
   python sales_analysis_udemy.py
   ```

---

#### Key Analysis and Findings

1. **Course Pricing**:
   - Mode of `discount_price__amount` is $455, with most courses having a standard discounted price.
   - Courses with discounts outperform non-discounted courses in attracting subscribers.

2. **Top Performing Courses**:
   - The top 10 courses by subscriber count include SQL, Tableau, PMP exam preparation, and financial analysis topics.

3. **Monthly Trends**:
   - Analysis of publishing dates reveals subscriber trends by month, highlighting peak months for course enrollments.

4. **Review-Subscriber Correlation**:
   - Courses with higher numbers of reviews show a positive relationship with subscriber counts, suggesting reviews as a key driver of popularity.

---

#### Visualizations

1. **Bar Chart**: Average number of subscribers for courses with and without discounts.
2. **Heatmap**: Correlation between key numerical features.
3. **Top 10 Courses**: A bar plot displaying subscriber counts for the most popular courses.
4. **Monthly Trends**: Bar chart showing total subscribers by month, with percentages labeled.

---

#### Contributions
Feel free to fork this repository, add new analyses, or propose enhancements to the existing workflow. Contributions are welcome to expand the scope of this analysis!

---

#### Disclaimer
This project is intended for educational purposes. The dataset used is publicly available and solely for non-commercial use.
