# Flight Delay Analytics with Apache Spark

## Project Overview
This project analyzes flight delay data to identify patterns, compare airline performance, and determine the most congested routes. The analysis is implemented using **Apache Spark**, utilizing both the **RDD API** and the **DataFrame API** to compare their performance, expressiveness, and optimization capabilities (Catalyst Optimizer).

## Key Features
* **Big Data Processing:** ETL operations on flight data using PySpark.
* **Comparative Analysis:** Benchmarking RDD vs. DataFrame execution times.
* **Data Visualization:** Insightful charts using Pandas, Matplotlib, and Seaborn.
* **Advanced Analytics:**
    * Top 10 routes with the highest average delays.
    * Hourly delay patterns (Time-series analysis).
    * Route-based Heatmaps (Origin vs. Destination).

## Technologies Used
* **Language:** Python 3.x
* **Engine:** Apache Spark (PySpark)
* **Libraries:** Pandas, Matplotlib, Seaborn
* **Environment:** Google Colab

## Key Insights & Visuals

### 1. Hourly Delay Patterns
Delays tend to accumulate throughout the day, peaking around 21:00 (propagation delay).
![Hourly Delay](images/plot_a_hourly)

### 2. Route Heatmap (Top Routes)
Specific routes show consistently higher delays compared to others.
![Heatmap](images/plot_c_heatmap)

## Performance Benchmark: RDD vs. DataFrame
A key part of this project was comparing the two Spark APIs.

| Approach | Average Execution Time | Why? |
| :--- | :---: | :--- |
| **DataFrame API** | **~0.5s** | Optimized by Spark's **Catalyst Optimizer**. |
| **RDD API** | ~2.5s | Opaque execution, slower Python-JVM serialization. |

## How to Run
1. Clone the repository:
   ```bash
   git clone [https://github.com/YOUR_USERNAME/Flight-Delay-Spark-Analytics.git](https://github.com/YOUR_USERNAME/Flight-Delay-Spark-Analytics.git)

## Tech Stack
* Python, PySpark
* Pandas, Matplotlib, Seaborn
* Google Colab
