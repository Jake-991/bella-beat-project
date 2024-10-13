# Bellabeatproject
This case study is part of the Google Data Analysis Certification program, aimed at providing guidance for the fitness company, Bellabeat, to optimize their product offerings and marketing strategies.
Bellabeat Data Analysis Case Study

## Table of Contents
1. [Ask:Define the Business Problem and Objectives](#Ask)
2. [Prepare: Data Collection and Preparation](#prepare)
3. [Clean/Process](#cleanprocess)
4. [Analyze](#analyze)
5. [Act](#act)
6. [Share](#share)

## Ask: Define the Business Problem and Objectives
### Project Overview
This case study is part of the Google Data Analysis Certification program, designed to provide actionable insights to Bellabeat, a wellness technology company focused on empowering women. The aim of this analysis is to help Bellabeat enhance their product offerings and refine their marketing strategies based on users’ engagement data and health patterns.

### Business Context
Bellabeat is a company that develops wearable health products for women, including fitness trackers that provide users with insights into their daily activity levels, sleep patterns, and overall wellness. With the increasing competition in the smart wellness market, Bellabeat seeks to strengthen its position by leveraging data to understand user behavior and preferences. By identifying key trends and correlations within user data, Bellabeat can develop targeted product features and marketing campaigns to increase user engagement and satisfaction.

### Problem Statement
Bellabeat needs to understand how users interact with their wellness devices and the impact of these devices on users' activity levels and lifestyle habits. Specifically, the company wants to explore patterns and trends related to physical activity, sleep duration, calorie consumption, and heart rate data to optimize product features and marketing efforts. The ultimate goal is to increase user retention and engagement while enhancing the overall user experience.

### Key Questions to Address
To provide meaningful insights and recommendations, the following questions will guide the analysis:

### Activity Patterns:

What are the most popular types of physical activities users engage in (e.g., steps, active minutes)?
How do activity levels vary throughout the day, and are there peak times when users are most active?
### User Behavior Analysis:

How does user behavior differ between weekdays and weekends in terms of activity levels, calorie burn, and sleep duration?
What factors correlate with higher levels of physical activity (e.g., heart rate, sleep quality)?
### Calorie and Sleep Monitoring:

How do users’ calorie consumption and burn patterns align with their activity levels?
Are there specific sleep patterns or habits that correlate with increased activity levels or higher overall wellness scores?
### Demographic and Behavioral Segmentation:

Are there specific user segments (e.g., age groups, activity levels) that demonstrate higher engagement rates or consistent product usage?
How can Bellabeat better personalize recommendations and marketing campaigns to target these segments effectively?
### Project Objective
The objective of this case study is to provide Bellabeat with actionable insights that will:

Optimize Product Features: Identify areas for improvement in Bellabeat’s devices and app based on user activity and engagement patterns, including the introduction of new features or updates that align with user behavior.
Enhance Marketing Strategies: Develop data-driven marketing strategies aimed at increasing user engagement by targeting peak activity periods, promoting consistent usage, and emphasizing health benefits based on actual user outcomes.
Increase User Retention: Leverage findings to create tailored recommendations that enhance the overall user experience, leading to increased user satisfaction and retention.
Stakeholders
The primary stakeholders for this project include:

Bellabeat Management Team: Responsible for strategic decisions related to product development and marketing initiatives.
Product Development Team: Focused on incorporating user feedback and data insights into future updates and new product features.
Marketing and Sales Team: Tasked with designing and executing targeted campaigns to increase product adoption and user retention.
Deliverables
At the conclusion of this project, the following deliverables will be provided:

### Comprehensive Report: A detailed report summarizing findings, insights, and actionable recommendations.
### Interactive Dashboard: An interactive visualization tool displaying key insights on user behavior and engagement patterns.
### Presentation: A professional presentation for Bellabeat stakeholders, outlining strategic recommendations for product and marketing optimization.
By addressing these questions and delivering actionable insights, this case study aims to empower Bellabeat to make data-driven decisions that enhance their product offerings and marketing strategies, ultimately contributing to their growth and success in the wellness technology market.

## Prepare: Data Collection and Preparation
### Overview
The Prepare phase involves collecting, understanding, and preparing the dataset for analysis. In this case study, we use data from Bellabeat’s wellness devices, which track various health metrics such as daily activity, sleep patterns, heart rate, and calorie consumption. The purpose of this step is to ensure that the data is well-structured, accurate, and ready for the subsequent cleaning and analysis stages.

### Data Sources
The dataset consists of multiple CSV and Excel files that cover a wide range of wellness and activity metrics collected from Bellabeat users. Below is a summary of each data source:

Daily Activity Data: Contains information on daily steps, active minutes, and total distance traveled.
Sleep Data: Tracks users’ sleep duration and sleep quality metrics.
Heart Rate Data: Records heart rate readings at different intervals.
Calorie Data: Captures calorie burn details across various activities and time intervals.
Weight and BMI Logs: Provides details on users’ weight, body mass index (BMI), and related metrics over time.
### Data Understanding
Each dataset includes different variables that provide insights into user behavior and wellness. Below is a summary of the key variables:

Time-Based Variables:
Date: The date on which the data was recorded.
Time: The time interval for minute/hourly data (e.g., heart rate, calories, steps).
Activity Variables:
Steps: The number of steps taken in a day or minute/hour interval.
Active Minutes: Time spent in various activity intensities (e.g., lightly active, fairly active, and very active).
Calories Burned: Total calories burned per day or interval.
Sleep Variables:
Sleep Duration: Total time spent sleeping per day.
Sleep Quality: Indicators such as REM sleep, deep sleep, and wake times.
Health Metrics:
Heart Rate: The user’s heart rate recorded at different time intervals.
Weight and BMI: Users’ weight and body mass index over time.
### Data Preparation Steps
To ensure the data is ready for analysis, the following preparation steps were taken:

Data Importation:

All datasets were imported into the analysis environment (Excel, BigQuery Power BI).
Initial exploratory analysis was performed to understand the structure and content of each dataset.
Data Validation:

Checked for missing values, inconsistencies, and anomalies across datasets.
Verified the date and time formats for consistency, ensuring that all time-based variables were standardized.
Data Integration:

Merged datasets where necessary (e.g., merging daily activity data with sleep data) to create a comprehensive view of user behavior.
Ensured proper alignment of time intervals when combining minute-level data with daily summaries.
Data Documentation:

Each dataset was documented to capture variable descriptions, units of measurement, and data types.
Developed a data dictionary to ensure clarity and consistency throughout the analysis process.
Data Limitations
It is important to note the following limitations and considerations related to the dataset:

Sample Size: The data represents only a subset of Bellabeat users, which may not be fully representative of the overall user base.
Time Frame: The data covers a specific period; trends observed may be influenced by seasonality or other time-based factors.
Data Integrity: Some missing values and inconsistencies were observed, particularly in the sleep and heart rate datasets. Strategies such as imputation or filtering may be required during the cleaning process.

## Clean/Process: Data Cleaning and Transformation
### Overview
The Clean/Process phase involves cleaning the datasets and preparing them for in-depth analysis. This step ensures data integrity, consistency, and accuracy, allowing for meaningful insights to be derived during the analysis phase. In this case study, multiple datasets related to user activity, sleep patterns, heart rate, and other wellness metrics have been cleaned and processed to establish a reliable foundation for analysis.

### Cleaning and Transformation Steps
Remove Duplicates:

Checked each dataset for duplicate entries, particularly in time-based data (e.g., minute-level data) to avoid inflated results during analysis.
Applied filters in Excel/Power Query to remove any repeated rows.

Handle Missing Values:
Identified and addressed missing values using the following strategies:
Drop rows: Removed rows with missing values if they were minimal and did not significantly impact the dataset.
Impute values: For essential metrics like sleep duration and heart rate, imputed missing values using appropriate statistical methods such as the mean, median, or forward-fill approach.
Documented these methods to maintain transparency in the cleaning process.

Standardize Date and Time Formats:
Ensured all time-based variables (e.g., start_time, end_time, date) were standardized to a consistent format (e.g., YYYY-MM-DD HH:MM:SS).
Converted columns to appropriate data types using Excel functions consistency.

Data Transformation:
Normalize Units: Converted units where necessary (e.g., steps per minute to steps per hour) to create consistency across datasets.
Aggregate Data: Aggregated minute-level data into daily summaries for easier analysis of patterns over time, using functions such as GROUP BY in SQL.

Create Calculated Fields: Added calculated fields, such as:
Daily Active Minutes: Summed various intensity levels (light, moderate, high) to understand users’ total daily active time.
Total Calories Burned: Combined different calorie sources (e.g., resting vs. active) to give a holistic view of daily calorie expenditure.
These transformations helped streamline analysis and highlight key user behavior trends.

Merge Datasets:
Merged relevant datasets (e.g., daily activity with sleep and calorie data) to provide a comprehensive view of user health metrics.
Ensured proper alignment of keys (e.g., user_id, date) to maintain data integrity during merging, using tools like Excel’s LOOKUP function.

Outlier Detection and Treatment:
Identified outliers using visual techniques (e.g., box plots in Excel/Power BI).
Assessed whether outliers represented data entry errors or extreme but legitimate user behavior:
Removed extreme outliers that were likely due to data errors (e.g., negative step counts).
Retained legitimate outliers after verification, as they could provide valuable insights into user behavior patterns.

Data Consistency and Integrity Checks:
Ensured that data fields across merged datasets were consistent in format and meaning.
Conducted cross-checks, such as validating the sum of hourly activity against daily totals, to verify the accuracy of aggregated data.

Tools and Techniques Used
#### Excel: Utilized for initial data exploration, handling duplicates, aggregating data and merging tables efficiently and applying basic filters.
#### SQL: Employed to aggregate data and merge tables efficiently, especially for time-based data.
#### Power BI: Used to visualize data patterns and identify outliers for further cleaning.

Data Transformation Documentation
A detailed data dictionary has been developed to document transformations applied to each dataset:

Original Variable: Name and description of the original data field.
Transformed Variable: Name and explanation of any new variables created (e.g., total_active_minutes).
Transformation Method: The method used for any data modification (e.g., aggregation, imputation).
Data Limitations After Cleaning
Even after cleaning, the following limitations were noted:

Sample Size Variations: Some datasets have fewer entries than others, which may affect the accuracy of analysis when merged.
Inconsistent Recording Times: Certain activity metrics were not recorded consistently across all users, leading to potential biases in aggregated data.
Imputed Values: While imputation was used to handle missing values, these estimates may not fully capture the actual user behavior.

## Analyze: Exploratory Data Analysis and Insights
### Overview
The Analyze phase focuses on performing Exploratory Data Analysis (EDA) to uncover patterns, trends, and relationships in the data. This step helps in understanding how different factors such as activity levels, sleep patterns, and calorie burn align with user behavior and wellness outcomes. Using Excel, SQL, and data visualization tools, key insights are drawn to address the main business questions.

### Key Questions Addressed
Activity Patterns:

### What are the most popular types of physical activities users engage in (e.g., steps, active minutes)?
How do activity levels vary throughout the day, and are there peak times when users are most active?
User Behavior Analysis:

### How does user behavior differ between weekdays and weekends in terms of activity levels, calorie burn, and sleep duration?
What factors correlate with higher levels of physical activity (e.g., heart rate, sleep quality)?
Calorie and Sleep Monitoring:

### How do users’ calorie consumption and burn patterns align with their activity levels?
Are there specific sleep patterns or habits that correlate with increased activity levels or higher overall wellness scores?
Demographic and Behavioral Segmentation:

### Are there specific user segments (e.g., age groups, activity levels) that demonstrate higher engagement rates or consistent product usage?
1. Activity Patterns:
Analysis Approach:
Data Used: dailyActivity_merged.csv
Metrics Analyzed:
Total Steps
Active Minutes (very active, fairly active, lightly active)
Sedentary Minutes
Key Findings:
Most Popular Activities: The majority of users spend a significant amount of time in lightly active minutes and sedentary minutes. Only a smaller portion of the day is spent in very active minutes, indicating room for encouraging more high-intensity activities.
Peak Activity Times: Analysis of the minute-level steps data revealed that users are most active during the morning (7–9 AM) and late afternoon (5–7 PM), coinciding with commuting times and after-work hours.
Visualization:
A line chart was created to show activity peaks during the day. This can help Bellabeat target these periods with notifications or workout suggestions.
Insights:
#### Recommendation: Bellabeat could develop features that push for more high-intensity workouts during the afternoon peak times or introduce reminders for users who remain in sedentary minutes for too long.
2. User Behavior Analysis:
Analysis Approach:
Data Used: dailyActivity_merged.csv, dailyCalories_merged.csv, and sleepDay_merged.csv
Metrics Analyzed:
Activity levels, Calories burned, and Sleep duration across weekdays and weekends.
Key Findings:
Weekday vs. Weekend Activity: Users are generally more active on weekends, with higher steps and active minutes. Sleep duration is also longer on weekends, suggesting users compensate for lack of sleep during the week.
Correlation Analysis:
Calories vs. Steps: A strong positive correlation (r ≈ 0.69) was found between calories burned and total steps taken, confirming that more active users burn more calories.
Sleep vs. Activity: A weak correlation (r ≈ 0.3) was found between sleep duration and activity levels, suggesting that while good sleep is important, it is not the primary driver of higher activity levels.
Visualization:
Bar charts comparing average steps, calories burned, and sleep duration on weekdays vs. weekends.
Scatter plots showing the relationship between calories burned and active minutes.
Insights:
#### Recommendation: Bellabeat could develop specific weekend challenges or promote healthier sleep habits during the week to boost user engagement and activity levels during weekdays.
3. Calorie and Sleep Monitoring:
Analysis Approach:
Data Used: dailyCalories_merged.csv, dailyActivity_merged.csv, and sleepDay_merged.csv
Metrics Analyzed:
Daily calories burned, sleep duration, and active minutes.
Key Findings:
Calories and Activity Alignment: Users with higher very active minutes tend to burn significantly more calories. Those with lightly active minutes or sedentary behavior tend to burn fewer calories, even if they have long activity durations.
Sleep Patterns and Activity: Users with better sleep quality (i.e., higher REM sleep or fewer wake times) tend to engage in more intense physical activity the following day. However, longer sleep duration doesn’t always equate to higher activity levels.
Visualization:
A scatter plot visualizing the relationship between very active minutes and calories burned.
Correlation matrix showing the relationship between sleep quality metrics and physical activity.
Insights:
#### Recommendation: Bellabeat should encourage users to improve sleep quality rather than just sleep duration. Features like sleep hygiene tips or wake-up time consistency could be introduced to improve overall wellness scores.
4. Demographic and Behavioral Segmentation:
Analysis Approach:
Data Used: dailyActivity_merged.csv and sleepDay_merged.csv
Metrics Analyzed:
Segmenting Users: Users were segmented into Low Activity, Moderate Activity, and High Activity based on their average steps per day.
Key Findings:
High Activity Users: Users who took more than 10,000 steps per day showed consistently higher engagement with the app and had better wellness scores (calories burned, active minutes).
Low Activity Users: These users tended to spend more time in sedentary minutes and showed lower levels of engagement with Bellabeat’s fitness features.
Visualization:
A pie chart was used to represent the distribution of users in each activity segment.
Bar charts showing the comparison of engagement metrics (steps, active minutes, calories burned) across user segments.
Insights:
#### Recommendation: Bellabeat could create personalized recommendations for each user segment:
For Low Activity users: Provide motivational content and easier workout routines.
For High Activity users: Offer rewards, challenges, or advanced tracking features to maintain engagement.
General Insights and Recommendations for Bellabeat:
Encourage High-Intensity Activity: Since users with higher very active minutes burn more calories, Bellabeat could introduce features that encourage short, intense workout sessions.
Weekday vs. Weekend Engagement: To increase engagement during the weekdays, Bellabeat could launch weekday challenges or introduce reminders for users to stay active during work hours.
Improve Sleep Quality: Bellabeat can promote sleep hygiene features that focus on improving sleep quality rather than just sleep duration. Encouraging users to follow a consistent sleep routine could help them become more active during the day.
Segmented User Engagement: Personalizing the app experience based on user activity levels will increase overall engagement. Bellabeat could offer different types of recommendations, content, and incentives based on whether users fall into the low, moderate, or high activity segments.
### Act: Recommendations Based on Data Insights
#### Overview
The Act phase translates the findings from our analysis into actionable recommendations for Bellabeat. These recommendations focus on enhancing product offerings, user engagement, and marketing strategies to improve user wellness and satisfaction.

#### Key Recommendations
1. Encourage High-Intensity Activity for Better Calorie Burn
Insight:
The analysis showed a strong positive correlation between very active minutes and calories burned. Users who engaged in high-intensity activities burned significantly more calories than those who only participated in lightly active or sedentary behavior.
Recommendation:
Feature Suggestion: Introduce a “High-Intensity Boost” feature that encourages users to participate in short, high-intensity workouts. This feature could include:
Short Workout Routines: Quick 10-15 minute intense exercises.
Reminders: Notifications during the day (especially during peak activity hours like morning and evening) encouraging users to complete a high-intensity workout.
Progress Tracking: A specific tracker for high-intensity minutes that displays the impact on calorie burn in real-time.
2. Promote Weekday Activity Engagement
Insight:
User activity levels are significantly lower on weekends compared to weekdays. While users tend to be more active during weekdays, their activity drops off during workends, possibly due to busy schedules.
Recommendation:
Feature Suggestion: Implement a “Weekend Challenge”:
Daily challenges designed to increase engagement during the weekends. These could include simple fitness tasks, step goals, or mini-workouts that can be completed throughout the day.
Team Challenges: Encourage social engagement by introducing team-based weekend challenges where users can compete with friends or colleagues to hit activity milestones.
3. Improve Sleep Quality for Enhanced Wellness
Insight:
Although the correlation between sleep duration and activity levels was relatively weak, users with better sleep quality (measured by fewer wake-up times and higher REM sleep) tended to be more active and burn more calories.
Recommendation:
Feature Suggestion: Introduce a “Sleep Improvement Program”:
Provide personalized insights and tips to help users improve their sleep quality, not just duration. Focus on sleep hygiene, consistent wake-up times, and avoiding interruptions during sleep.
Offer sleep reminders: Notifications to remind users to wind down and prepare for bed (e.g., mindfulness practices or sleep-friendly routines).
Sleep Reports: A weekly summary of sleep quality with actionable tips on how users can improve their sleep to boost their wellness and energy levels.
4. Segment Users for Personalized Recommendations
Insight:
Users with higher daily step counts (over 10,000 steps/day) showed consistently higher engagement with the app and better wellness outcomes. On the other hand, low-activity users (under 5,000 steps/day) were less engaged.
Recommendation:
Feature Suggestion: Introduce User Segmentation and Personalized Recommendations:
Create Low, Moderate, and High Activity User Segments based on daily steps or activity levels.
Provide personalized recommendations for each segment:
Low Activity Users: Encourage them with beginner-level workouts, motivational content, and easy-to-achieve daily step goals.
Moderate Activity Users: Suggest more advanced workout routines and weekly challenges to push them to the next activity level.
High Activity Users: Offer advanced tracking features, fitness challenges, and rewards for maintaining high activity levels.
Implement goal-based incentives, such as unlocking achievements, earning badges, or gaining rewards for reaching certain milestones.
5. Target Marketing Campaigns for Each User Segment
Insight:
Each user segment (low, moderate, high activity) behaves differently in terms of engagement and activity levels, which means that marketing efforts need to be more personalized to target their specific needs.
Recommendation:
Marketing Strategy: Create segment-specific marketing campaigns to increase engagement and retention:
Low Activity Segment: Run campaigns focused on motivation, simple health tips, and rewards for hitting easy goals.
Moderate Activity Segment: Promote new fitness challenges or features that can push them to higher activity levels.
High Activity Segment: Focus on advanced fitness features, rewards, and exclusive content (such as guided workout plans).
Metrics for Success:
Measure the impact of these changes by tracking:
Daily and Weekly Active Minutes
User Engagement Rates (daily app opens, feature usage)
Increased Calorie Burn for users who engage with new features
Sleep Quality Improvement over time
Conclusion
By implementing the above recommendations, Bellabeat can enhance user engagement, improve wellness outcomes, and offer personalized features that cater to different user segments. Encouraging high-intensity activity, improving weekday engagement, and promoting better sleep quality will help Bellabeat position itself as a comprehensive wellness platform that meets its users' physical and mental well-being needs.
