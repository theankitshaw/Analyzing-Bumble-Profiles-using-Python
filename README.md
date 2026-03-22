# Analyzing-Bumble-Profiles-using-Python
A detailed exploratory data analysis of user profiles to uncover insights into demographics, lifestyle preferences, and behavioral trends for optimizing the matchmaking experience.

# 2. Short Description / Purpose
The Bumble Profile Analytics project is a comprehensive Python-based exploratory data analysis (EDA) designed to help product and marketing teams understand the platform's user base. By analyzing nearly 60,000 user profiles, this project focuses on rigorous data cleaning, handling missing optional fields, and uncovering relationships between lifestyle habits, physical attributes, and demographics. This analysis is intended for data-driven strategists seeking to enhance user engagement, optimize matchmaking algorithms, and personalize platform features for improved user satisfaction and platform growth.

# 3. Tech Stack
The analysis was built using the following tools and technologies:

Python - The core programming language used for the data analysis.

Pandas - Main data manipulation and analysis layer used for cleaning, reshaping, and exploring the tabular dataset.

NumPy - Used for numerical computing and handling mathematical operations.

Matplotlib & Seaborn - Visualization libraries utilized to create publication-quality charts such as missing data heatmaps, bar charts, and scatterplots.

Jupyter Notebook - Interactive development environment used to step-by-step document the code, methodology, and business insights.

# 4. Dataset Information
Data on roughly 59,946 Bumble users consisting of 17 distinct columns. It includes details on demographics (age, status, gender), physical attributes (body_type, height), lifestyle preferences (diet, drinks), educational/financial details (income), and user activity/location (last_online, location).

# 5.  Features / Highlights
Business Problem: Dating platforms rely on user-generated information to foster connections, but this data is frequently messy, incomplete, or contains anomalies. Key questions include:

Which profile fields do users most commonly skip, and how should we handle them?

How can we deal with invalid or extreme data (e.g., negative incomes or 110-year-old users) without destroying our sample size?

What are the underlying relationships between a user's age, income, and lifestyle habits?

Goal of the analysis: To logically Clean, Process, Explore, and Visualize the user data to provide clear comparisons and insights for stakeholders.

Walk through of key steps:

Data Cleaning & Missing Values: Identified that columns like Diet, Pets, and Religion had the most missing values (33–40%), indicating these are often treated as optional. Handled missing physical data contextually by imputing missing heights with the median height of the user's specific gender.

Data Processing & Outlier Handling: Converted the last_online column into a proper datetime format for time-based analysis. Filtered out extreme outliers in age, height, and income by isolating the middle 80% of the data to calculate accurate statistics (e.g., finding realistic mean/median ranges) and replaced invalid -1 income entries with 0.

# 6. Business Impact & Insights
Matchmaking Refinement: Understanding the distributions and correlations between demographics (like gender and age) and lifestyle habits allows the product team to heavily optimize the recommendation and matchmaking algorithms for better compatibility.

Marketing Optimization: Insights into the geographical distribution of active users and prevailing age groups enable marketing teams to launch highly targeted regional and demographic-specific campaigns.

Feature Personalization: Grouping continuous variables (like age into ranges and income into brackets) helps UI/UX teams design more intuitive user search filters and personalized discovery pages.

Platform Growth: By utilizing cleaned, standardized data to understand exactly who the users are and what they prefer, Bumble can make data-driven decisions that improve overall user satisfaction and retention.
