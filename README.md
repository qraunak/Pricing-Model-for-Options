**Option Pricing Project**

This project implements various option pricing models and provides functionality to fetch stock data from Yahoo Finance.

**Project Structure**

```
option_pricing_project/
├── main.py
├── option_pricing/
│   ├── __init__.py
│   ├── black_scholes.py
│   ├── binomial_tree.py
│   ├── monte_carlo.py
│   ├── option_pricing_model.py
│   └── ticker.py
├── test_script.py
└── README.md
```

**Installation**

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/option_pricing_project.git
   cd option_pricing_project
   ```
2. **Install dependencies:**
   Create a `requirements.txt` file with:
   ```
   pandas
   pandas-datareader
   numpy
   scipy
   matplotlib
   ```
   Then install:
   ```bash
   pip install -r requirements.txt
   ```

**Usage**

* **Run the main script:**
  ```bash
  python main.py
  ```
* **Run the test script:**
  ```bash
  python test_script.py
  ```

**Option Pricing Models**

* **Black-Scholes Model:**
  - Implemented in `option_pricing/black_scholes.py`.
  - Calculates prices of European call and put options.
* **Binomial Tree Model:**
  - Implemented in `option_pricing/binomial_tree.py`.
  - Uses a binomial tree approach for European option pricing.
* **Monte Carlo Simulation:**
  - Implemented in `option_pricing/monte_carlo.py`.
  - Uses simulation to estimate prices of European options.

**Stock Data Fetching**

The `Ticker` class in `option_pricing/ticker.py` uses `pandas-datareader` to fetch stock data from Yahoo Finance. It provides methods to:

- Get available data columns for a stock.
- Fetch the last closing price.
- Plot historical stock data.
