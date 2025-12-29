**📈 Mean-Variance Portfolio Optimization (Modern Portfolio Theory)**
**📌 Project Overview**

This project implements Mean-Variance Portfolio Optimization based on Modern Portfolio Theory (MPT) proposed by Harry Markowitz.
The goal is to construct optimal investment portfolios by balancing risk (volatility) and expected return using real historical stock data.

The project:

Fetches real market data

Analyzes risk-return tradeoffs

Simulates thousands of portfolios

Plots the Efficient Frontier

Optimizes portfolios using numerical optimization techniques
**
🎯 Objectives**

Understand and implement Modern Portfolio Theory

Analyze portfolio expected return, variance, covariance

Construct the Efficient Frontier

Find:

Minimum Risk Portfolio

Maximum Sharpe Ratio Portfolio

Visualize risk-return tradeoffs clearly

**🧠 Key Concepts Covered**

Expected Return

Portfolio Variance & Covariance

Diversification

Efficient Frontier

Sharpe Ratio

Capital Market Line (CML)

Constrained Optimization
**
🛠️ Technologies & Libraries Used
**
Python

NumPy – Numerical computation

Pandas – Data manipulation

Matplotlib – Data visualization

yfinance – Fetch historical stock prices

SciPy (optimize) – Portfolio optimization

**📂 Project Structure**

portfolio-optimization/
│
├── portfolio_optimization.py   # Main Python script
├── README.md                   # Project documentation
└── requirements.txt            # Required Python libraries

**📊 Methodology & Workflow**

1️⃣ Data Collection

Historical adjusted closing prices are fetched using yfinance

Daily returns are computed from price data

2️⃣ Risk & Return Calculation

Annualized expected returns

Annualized covariance matrix of returns

3️⃣ Portfolio Simulation

Random portfolio weights are generated

Risk, return, and Sharpe ratio calculated for each portfolio

Used to visualize the Efficient Frontier

4️⃣ Optimization

Using SciPy’s SLSQP optimizer:

Max Sharpe Ratio Portfolio

Minimum Variance Portfolio

Constraints applied:

Fully invested portfolio (weights sum to 1)

No short selling (weights ≥ 0)

5️⃣ Visualization

Efficient Frontier

Optimal portfolios highlighted

Capital Market Line plotted

📐 Mathematical Formulation
Expected Portfolio Return:
𝑅
𝑝
=
∑
𝑖
=
1
𝑛
𝑤
𝑖
𝑅
𝑖
R
p
	​

=
i=1
∑
n
	​

w
i
	​

R
i
	​

Portfolio Variance:
𝜎
𝑝
2
=
𝑤
𝑇
Σ
𝑤
σ
p
2
	​

=w
T
Σw
Sharpe Ratio:
Sharpe
=
𝑅
𝑝
−
𝑅
𝑓
𝜎
𝑝
Sharpe=
σ
p
	​

R
p
	​

−R
f
	​

	​


Where:

𝑤
w = asset weights

𝑅
R = expected returns

Σ
Σ = covariance matrix

𝑅
𝑓
R
f
	​

 = risk-free rate

📈 Output & Results

Efficient Frontier curve

Maximum Sharpe Ratio portfolio

Minimum Risk portfolio

Clear visualization of risk vs return tradeoff
**
🚀 How to Run the Project**

1️⃣ Install Dependencies

pip install numpy pandas matplotlib yfinance scipy

2️⃣ Run the Script

python portfolio_optimization.py

**🔍 Sample Use Case**

This model helps investors:

Compare multiple portfolios

Understand diversification benefits

Select optimal asset allocation based on risk preference

**🧩 Possible Extensions**

Add transaction costs

Include short selling

Use machine learning to forecast returns

Dynamic portfolio rebalancing

Add sector or ESG constraints
