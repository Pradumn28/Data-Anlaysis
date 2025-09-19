# 📈 Stock Market Analysis (NSE) using Pandas & Plotly

This project analyzes **5 selected stocks from the NSE (National Stock Exchange of India)** and performs detailed studies on their **price trends, volatility, and cumulative returns**.  

The goal of this project is to **showcase my familiarity with Pandas and Plotly** — two powerful Python libraries for **data manipulation** and **interactive visualization**.  

---

## 🚀 Project Overview  

Using **Pandas**, I:  
✔️ Cleaned and pre-processed raw stock price CSV files  
✔️ Extracted useful insights (returns, volatility, trends)  
✔️ Prepared the data for visualization  

Using **Plotly**, I:  
✔️ Built **interactive stock price charts**  

 ![Opening_Price](images/opening_price_line_chart.png)

✔️ Visualized **Moving Averages**

 ![Moving_Averages](images/moving_averages.png)

✔️ Compared **cumulative returns** of the chosen stocks 

 ![Cumulative_Returns](images/cumulative_returns.png)

✔️ Compared **collinearity** of the chosen stocks 

  ![Collinearity](images/collinear_correaltions.png)

---

## 📂 Repository Structure  

```bash
Stock-Market-Analysis/  
│── html/  
│   └── project.html              # Full interactive notebook (download & open in browser)
|__ india_stocks_6years.csv       # Cleaned data of about 6 years of 5 stocks(2019-2025)
│  
│── images/  
│   ├── opening_prices.png          # Stock price trend chart  
│   ├── traded_value.png            # Volatility analysis chart  
│   └── cumulative_returns.png    # Cumulative returns visualization  
│  
│── technical_code.ipynb          # Jupyter Notebook with Pandas & Plotly code  
│── README.md                     # Project documentation (this file)  

```

---

## 🔍 Key Analysis  

📊 **Trends in Stock Prices** – Daily price changes across selected NSE stocks  
📉 **Volatility of Returns** – Measuring the ups and downs in daily returns  
📈 **Cumulative Returns** – Long-term performance comparison across stocks  

---

## 📌 How to Explore the Project  

👉 **1. Quick Look**  
- Open the `images/` folder for static snapshots of the charts.  

👉 **2. Full Interactivity (Recommended)**  
- GitHub does **not support interactive Plotly charts directly**.  
- To explore full interactivity:  
  1. Download the file: [`html/project.html`](./html/project.html)  
  2. Open it in your browser  
  3. You’ll be able to **zoom, hover, and interact** with the charts 🎉  

👉 **3. Technical Code**  
- Check `technical_code.ipynb` for the full Jupyter Notebook code (data cleaning + analysis + charts).  

---

## 🛠️ Technologies Used  

- 🐍 **Python**  
- 🗂️ **Pandas** – Data cleaning, manipulation, returns calculation  
- 📊 **Plotly** – Interactive charting and visualization  
- 📓 **Jupyter Notebook** – Analysis environment  


---

## ⚡ Getting Started (Optional: Run the Notebook Yourself)  

If you want to re-run the analysis:  

```bash
# Clone the repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

# Install dependencies
pip install pandas plotly jupyter

# Open Jupyter Notebook
jupyter notebook technical_code.ipynb
```
📬 Contact

If you’re a hiring manager, data enthusiast, curious learner, or you have any doubt feel free to connect:

💼 [LinkedIn](https://www.linkedin.com/in/pradumnchauhan)!

📧 [Email](pradumnchauhan2812@gmail.com)!


flowchart TD
    %% Define styles for clarity
    classDef user fill:#cde4ff,stroke:#333,stroke-width:2px;
    classDef role fill:#ffd8b4,stroke:#333,stroke-width:2px;
    classDef object fill:#d4edda,stroke:#333,stroke-width:2px;
    classDef action fill:#f8d7da,stroke:#333,stroke-width:2px;

    %% Admin Node
    A[🔐 Database Administrator<br/><sub>THE DECISION MAKER</sub><br/><sub>Defines WHO can do WHAT</sub>]

    %% Roles Section
    subgraph Roles [ROLES: Job Titles with Clear Responsibilities]
        direction LR
        R1[<b>👥 Role: Sales Analyst</b><br/><sub>Can work with sales data</sub>]
        R2[<b>👥 Role: Customer Support</b><br/><sub>Can view order & customer info</sub>]
        R3[<b>👥 Role: Application Developer</b><br/><sub>Can read & write to app tables</sub>]
    end

    A -->|GRANTS| R1
    A -->|GRANTS| R2
    A -->|GRANTS| R3

    %% Permissions Section
    P1[<b>SELECT</b><br/><sub>Can READ data</sub>]
    P2[<b>UPDATE</b><br/><sub>Can MODIFY existing data</sub>]
    P3[<b>INSERT</b><br/><sub>Can ADD new data</sub>]
    P4[<b>DENIED</b><br/><sub>Cannot access at all</sub>]

    %% Assign Permissions to Roles
    R1 --> |CAN DO| P1
    R1 --> |CAN DO| P2

    R2 --> |CAN DO| P1
    R2 --> |CANNOT DO| P4

    R3 --> |CAN DO| P1
    R3 --> |CAN DO| P3

    %% Objects Section
    subgraph Objects [OBJECTS: What is being protected?]
        direction LR
        O1[<b>📊 Table: Sales_Data</b><br/><sub>Contains all sales records</sub>]
        O2[<b>📋 Table: Customer_Info</b><br/><sub>Contains personal details</sub>]
        O3[<b>📦 Table: Order_Details</b><br/><sub>Contains all orders</sub>]
        O4[<b>🔐 Table: User_Accounts</b><br/><sub>Contains login info</sub>]
    end

    %% Link Permissions to Objects for each Role
    P1 --> |ON| O1
    P2 --> |ON| O1

    P1 --> |ON| O2
    P4 --> |ON| O2

    P1 --> |ON| O3

    P1 --> |ON| O4
    P3 --> |ON| O4


✨ Clone the repo, download the interactive HTML, and explore how Pandas + Plotly bring stock market data to life!


