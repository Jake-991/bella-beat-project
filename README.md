# Bellabeat Wellness Product Strategy

This project explores how Bellabeat, a smart wellness product company, can improve user engagement and inform product strategy by analyzing activity data from its fitness tracker users. Using behavioral data from wearable devices, the project identifies trends in sleep, activity, and sedentary behavior to support decisions in product design and marketing.

---

## Table of Contents

- [Project Objective](#project-objective)
- [Business Questions](#business-questions)
- [Tools and Techniques](#tools-and-techniques)
- [Data Preparation](#data-preparation)
- [Analysis Highlights](#analysis-highlights)
- [Strategic Insights](#strategic-insights)
- [Key Takeaways](#key-takeaways)
- [Power BI Visuals](#power-bi-visuals)
- [Contact](#contact)
- [License](#license)

---

## Project Objective

To help Bellabeat refine its product and marketing strategy by analyzing behavioral patterns in activity tracker usage, with the goal of increasing engagement, promoting healthier habits, and identifying high-value user segments.

---

## Business Questions

- How active are Bellabeat users on average, and how does that vary by weekday, time of day, or user segment?
- What correlations exist between sleep quality, activity levels, and sedentary time?
- Can usage patterns inform targeted recommendations or product features?

---

## Tools and Techniques

- Python (pandas, matplotlib, seaborn) for data wrangling and exploration
- Tableau for data visualization and storytelling
- Excel for early-stage cleaning and data validation

---

## Data Preparation

- Used public FitBit fitness tracker dataset (n = ~30 users over 30 days)
- Cleaned and merged multiple CSVs (activity, sleep, weight logs)
- Removed duplicates, invalid entries, and filled missing values where appropriate
- Standardized timestamps and derived new features: activity buckets, sleep efficiency, and weekday usage patterns

---

## Analysis Highlights

- Users who met or exceeded 10K steps/day had significantly higher sleep efficiency
- Weekends had the highest levels of sedentary time across most users
- Late-night device usage correlated with lower average sleep duration the following night
- A subset of users showed strong adherence to routines, making them ideal targets for habit-streak features

---

## Strategic Insights

Bellabeat can take action on several fronts:

- **Habit Reinforcement Features:** Users with consistent behavior patterns may respond well to streak-based rewards or progress tracking visuals
- **Sleep-Aware Nudges:** Push notifications could discourage device use late at night to improve sleep outcomes
- **Activity-Based Segmentation:** Target low-movement users with gentle encouragement; reward highly active users with challenges
- **Content Personalization:** Sleep-focused users may benefit from mindfulness/audio content integrations

---

## Key Takeaways

- Behavioral data reveals lifestyle segments and opens doors for targeted engagement
- Bellabeat can use usage patterns not only for user feedback but also for **product innovation**
- This project demonstrates a real-world application of analytics to support wellness tech growth strategy

---

## Power BI Visuals

Below are key dashboards created using Power BI. These visuals highlight:
- Weekly trends in calories burned
- Step count distribution across days
- Activity classification by intensity level
- Sleep vs. activity comparison plots
- Engagement breakdowns by user clusters

1. Activity Patterns
Finding: The most popular activities among users are lightly active minutes and sedentary minutes. High-intensity activities (very active minutes) occur less frequently.

Visualization: ![Activity_Patterns](Image/Popular_Types_of_Minutes.jpg)

Activity levels tend to peak during morning (7–9 AM) and evening hours (5–7 PM).

Visualization: ![Activity_level](Image/Peak_Steps_24_Hour.jpg)

2. Weekday vs. Weekend Behavior
Finding: Users are generally more active on weekends, with more steps taken and higher active minutes compared to weekdays. However, calorie burn is similar across both.
 ![Weekdays_vs_weekends](Image/Calories_Burn.jpg)

4. Correlation Between Sleep and Activity
Finding: While longer sleep duration does not strongly correlate with higher activity levels, users with better sleep quality tend to engage in more physical activity.
Visualization: ![Correlation](Image/Correlation_Sleepcaloriesburn.jpg)

5. Segmentation by Activity Level
Finding: Users can be segmented into low, moderate, and high activity groups based on daily steps, with high activity users demonstrating more consistent engagement and better wellness scores.
Visualization: ![Activity_Level](Image/Activity_Groups_Per.jpg)

The Power Bi Dashboard As Below:
![Dashoard](Image/Dashboard_Graph.jpg)

---

## Contact

Created by [Jake Ma](https://www.linkedin.com/in/jake-ma-0a4278282/)  
Let’s connect if you’re hiring or want to discuss data-driven product strategy in health tech.
