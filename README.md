# Home Sales

In this assignment, we used SparkSQL to create temporary tables, partition data, and cache a temporary table  
to see the difference in performance time between cached and partitioned data. Using SQL format, the data will  
be queried to different criteria to scale the data. Use the scaled data to perform your analysis on.  

---

## Getting Started

1. Create a new repository for this project called `Home_Sales`.
2. Grab the [Starter_Code](https://github.com/Kaileycar/Home_Sales/files/12838542/Starter_Code.zip).
3. Use Google Colab if `PySpark` is not locally downloaded.

---

## Installation 

### MAC
  * **Java**
      * Use Homebrew. In terminal run `brew install openjdk`.
      * Download the `x64 Installer` from [Oracle](https://www.oracle.com/java/technologies/downloads/#jdk20-mac)
  * **PySpark**
      * Run `pip install pyspark==3.4.0` in terminal.
  * **FindSpakr**
      * Run `conda install -c conda-forge findspark` in terminal.
  * **PyArrow** and **Fastparquet**
      * Run `conda install -c conda-forge pyarrow` and `conda install -c conda-forge fastparquet` in terminal.

---

## Usage

1. Read in [home_sales_revised.csv](https://github.com/Kaileycar/Home_Sales/files/12838564/home_sales_revised.csv).
2. Convert to a DataFrame.
3. Create a temporary table called `home_sales`.
4. Query your data to the apropriate questions.
5. Cache your temporary table `home_sales`.
6. Using the cached data, run the query that filters out the view ratings with an average price of greater
   than or equal to $350,000. Determine the runtime and compare it to uncached runtime.
7. Partition by the `"date_built"` field on the formatted parquet home sales data.
8. Create a temporary table for the parquet data.
9. Run the same query as above and compare the runtime to the cached data.
10. Uncache the `home_sales` temporary table.

---

## Links

[Aggregate in SQL](https://www.codecademy.com/learn/learn-sql/modules/learn-sql-aggregate-functions/cheatsheet)
