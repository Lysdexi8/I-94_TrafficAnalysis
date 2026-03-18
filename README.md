# I-94_TrafficAnalysis
Analysing the westbound traffic data using indicators such as weather type, time of the day,  time of the week etc on the I-94 Interstate highway.

This project analyzes a dataset from the UCI Machine Learning Repository that records westbound traffic on the I-94 Interstate Highway between Minneapolis and Saint Paul. The goal is to identify what conditions lead to heavy traffic, such as time of year, time of day, day of week, or weather patterns.

---

## Dataset

* **Source:** UCI Machine Learning Repository
* **Rows:** ~48,000 hourly observations
* **Columns include:**

  * `traffic_volume` — cars per hour (target)
  * `date_time` — timestamp
  * `temp`, `rain_1h`, `snow_1h`, `clouds_all`
  * `weather_main`, `weather_description`

---

## Project Objectives

1. Analyze traffic distribution during day vs night
2. Identify monthly, weekly, and hourly traffic patterns
3. Examine correlation between weather and traffic
4. Determine indicators of heavy traffic conditions

---

## Tools Used

* Python
* Pandas (data cleaning and analysis)
* Matplotlib (visualization)
* Jupyter Notebook

---

## Key Insights

### Time-Based Indicators

* Warm months (March–October) consistently show higher traffic.
* Weekdays have significantly heavier traffic than weekends.
* Rush hours occur around 7 AM and 4–5 PM on business days.
* Nighttime traffic is much lighter (average ~1,700 cars/hour vs ~4,700 during daytime).

### Weather-Based Indicators

Although no strong correlations were found, a few weather descriptions showed slightly higher averages:

* Shower snow
* Light rain and snow
* Proximity thunderstorm with drizzle

This may indicate more people choose to drive instead of walking or biking during mild adverse weather.

---

## Methodology

* Loaded and examined dataset structure
* Converted timestamps to datetime format
* Split records into day vs night
* Created new time columns (`month`, `dayofweek`, `hour`)
* Grouped data to analyze trends across time
* Calculated correlations for numeric weather variables
* Visualized weather categories and traffic averages

---

## Visualizations

The notebook includes the following charts:

* Histogram of overall traffic volume
* Day vs night traffic comparison
* Traffic by month
* Traffic by weekday
* Rush hour patterns (weekday vs weekend)
* Temperature vs traffic scatter plot
* Weather-type traffic comparison

---

## Conclusion

Heavy traffic on I-94 is strongly influenced by time factors such as seasonality, business days, and rush hours. Weather has limited impact overall, but certain weather descriptions correlate with higher-than-average traffic.

---

## Repository Structure

```
├── I94_Traffic_Analysis.ipynb
├── Metro_Interstate_Traffic_Volume.csv
└── README.md
```

---

## Future Improvements

* Add a regression model to predict traffic volume
* Explore anomaly detection for unusual traffic spikes
* Analyze eastbound traffic for comparison

---

## Contact

If you'd like to connect or discuss data analysis projects, feel free to reach out!

