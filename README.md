# Data-Analysis-with-Python---Weather-Dataset

# Weather Data Analysis with Python

🧭 **Project Overview**

This project utilizes Python’s powerful data analysis to explore and analyze an hourly weather dataset for 2012. The primary goal is to extract patterns and insights related to weather conditions, which can support decision-making in sectors such as **agriculture, travel planning, and outdoor event management**.

📂 **Dataset**

The dataset contains **8784 hourly records** and includes the following attributes:

* **Weather Condition:** Descriptive labels such as 'Clear', 'Cloudy', 'Rain', 'Snow', etc.
* **Temperature (Temp\_C):** Recorded in degrees Celsius.
* **Dew Point Temp\_C:** Dew point in degrees Celsius.
* **Relative Humidity (Rel Hum\_%):** Percentage of humidity.
* **Wind Speed (Wind Speed\_km/h):** Speed in kilometers per hour.
* **Visibility (Visibility\_km):** Measured in kilometers.
* **Pressure (Press\_kPa):** Atmospheric pressure in kPa.

🔍 **Key Analysis Steps**

1. **Data Loading and Inspection**

   * Loaded the dataset using `pd.read_csv()` and used `df.head()` and `df.info()` to check data types and preview the data.

2. **Data Cleaning**

   * Converted relevant columns to proper numeric types.
   * Verified there were **no missing values**, ensuring complete data integrity.

3. **Exploratory Data Analysis (EDA)**

   * Computed **mean values of numeric columns** grouped by `Weather Condition`.
   * Filtered data for specific conditions, e.g., all instances of `Weather Condition = "Clear"` and occurrences of `Wind Speed > 24 km/h` with `Visibility = 25 km`.
   * Counted occurrences of particular weather types such as `Snow` or `Clear`.

4. **Data Visualization**

   * Generated **bar plots** for the distribution of `Weather Condition`.
   * Created **histograms and boxplots** to visualize numerical features like temperature, humidity, and wind speed.

📈 **Insights**

* **Weather Condition Distribution:**

  * The most frequent conditions were **Clear (1326 instances)**, **Mostly Cloudy (2069)**, and **Cloudy (1728)**.
  * Snow and Rain were less frequent but significant for certain months.

* **Wind and Visibility:**

  * Wind speed of 4 km/h was the most common (474 occurrences).
  * Higher wind speeds (>24 km/h) with limited visibility (25 km) occurred 308 times.

* **Grouped Statistics:**

  * Average temperature was highest under **Mostly Clear** (12.56°C) and lowest during **Snow** (-4.52°C).
  * Humidity was highest during **Rain** (83.62%) and lowest during **Mostly Clear** (60.67%).

* **Conditional Observations:**

  * There were specific patterns, such as **Clear weather with high visibility** or **Snow events with low temperature and high humidity**, which can help in predictive analyses.

🚀 **Conclusion**

This analysis highlights how Python can be leveraged to process, clean, and explore weather data effectively. Insights from this dataset can inform planning in agriculture, transportation, and event management. Future extensions could include **time-series analysis and predictive modeling** to forecast weather conditions based on historical patterns.

