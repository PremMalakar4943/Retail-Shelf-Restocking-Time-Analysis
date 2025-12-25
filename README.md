# Retail-Shelf-Restocking-Time-Analysis
# Retail Shelf Restocking Time Analysis
**Minor 1 – Pandas Project**

## 📌 Project Overview
This project analyzes inventory data for a retail store to optimize supply chain efficiency. The goal is to identify which product categories face the longest restocking delays and to recommend specific items for immediate reordering.

Since the original dataset did not contain specific delivery times, we used **stochastic simulation** to model restocking delays, allowing us to perform statistical analysis and visualization.

## 🛠️ Technologies Used
* **Python:** Core programming language.
* **Pandas:** For data loading, manipulation, and calculating statistics (Mean/Std Dev).
* **Matplotlib:** For creating visualizations (Bar charts and Line plots).
* **NumPy:** For data simulation (generating random delay scenarios).

## 📊 Key Features & Logic
1.  **Data Processing:** * Loads the top 100 records from `retail_store_inventory.csv`.
    * Cleans and prepares data for analysis.
2.  **Stochastic Simulation:** * Simulated a "Restocking Delay" column (1–7 days) using `random` logic to mimic real-world uncertainty.
3.  **Statistical Analysis:** * **Mean:** Calculated the average wait time (~4.2 days).
    * **Standard Deviation:** Measured the risk/volatility of the supply chain.
4.  **Visualization:**
    * **Bar Plot:** Compares average delays across categories (Clothing, Electronics, Toys, etc.).
    * **Line Plot:** Tracks daily delay fluctuations.
5.  **Rule-Based Decision System:** * Implements a logic check: `IF Inventory < 100 THEN Recommend Restock`.

## 📉 Insights Generated
* **Bottleneck Identification:** The **"Toys"** category was identified as having the highest average restocking delay.
* **Supply Chain Volatility:** The analysis shows a standard deviation of ~1.9 days, indicating moderate unpredictability in delivery times.
* **Restocking Alerts:** Generated a list of specific `Product IDs` that are critically low on stock.

## 🚀 How to Run the Project
1.  **Prerequisites:**
    Make sure you have Python installed. Install the required libraries:
    ```bash
    pip install pandas matplotlib numpy
    ```

2.  **Run the Code:**
    Execute the Python script:
    ```bash
    python main.py
    ```

3.  **Output:**
    * The script will print statistical insights to the console.
    * It will generate and save a graph image (e.g., `bar_chart_restocking.png`).

## 📂 Project Structure
* `main.py`: The source code containing data processing, simulation, and plotting logic.
* `retail_store_inventory.csv`: The dataset used for analysis.
* `README.md`: Project documentation.
* `*.png`: Generated graphs saved by the script.

---
*Submitted for Minor 1 Project | Data Analytics*
