# Powerball Trends and Number Generator

This project explores historical Powerball data to uncover trends and patterns in winning numbers and uses these insights to create a statistically informed lottery number generator.

## Project Overview

The project was motivated by the question: **Are there identifiable trends in Powerball draws?** Using historical draw data from 2020 to 2024, we performed an exploratory data analysis (EDA) to identify patterns in winning numbers and jackpot trends. The findings informed the development of a Python-based Powerball number generator that blends statistical insights with the inherent randomness of lottery draws.

## Key Components

### 1. **Data Collection and Cleaning**
- Historical Powerball data was gathered using a custom-built web scraper.
- Data included draw dates, jackpot amounts, winning numbers, and prize details.
- Cleaning involved removing duplicates, standardizing formats, and parsing numeric values for analysis.

### 2. **Exploratory Data Analysis (EDA)**
- **Macro Trends:**
  - Seasonal variations: Higher jackpots during winter months, particularly around the holidays.
  - Jackpot amounts increase during rollover streaks but stabilize around ~$250 million on average.
  - On average, six jackpot winners occur per year, with time between winners averaging 54 days.

- **Micro Trends:**
  - Frequently drawn numbers: Some numbers, like 33, appear significantly more often.
  - Odd/Even patterns: Draws typically feature a mix of odd and even numbers, with splits like 3 odd/3 even being the most common.
  - Positional analysis: Specific number ranges (e.g., 1–10) are more likely to appear in certain positions.

### 3. **Number Generator Development**
- Built in Python, the generator:
  - Produces **5 white-ball numbers (1–69)** and **1 red Powerball number (1–26)**.
  - Uses weighted probabilities based on historical frequency to reflect real-world patterns.
  - Enforces constraints, such as odd/even balance and limiting consecutive numbers, to align with observed trends.
  - The red Powerball is generated randomly due to a lack of discernible trends.

### 4. **Technical Challenges**
- Initial recursive algorithms caused stack overflow errors; resolved by adopting an iterative approach with retry limits.
- Constraints were refined to balance statistical realism with the flexibility needed for randomness.

### 5. **Final Output**
The generator creates statistically informed yet random combinations, such as:
- **White balls:** [4, 15, 23, 36, 42]
- **Red Powerball:** 12

## Key Takeaways
- Data analysis revealed identifiable trends in Powerball draws, demonstrating that even highly random systems can exhibit patterns.
- The generator showcases the application of data science in combining historical trends with randomness.
- This project highlights the value of turning raw data into actionable insights and practical tools, offering a deeper understanding of probabilistic systems.

## Future Work
- Test the generator’s outputs by purchasing tickets and observing results over time.
- Explore additional features, such as adjusting weights dynamically based on updated historical data.
- Expand analysis to include other lottery systems for comparative studies.

## How to Use
1. Clone the repository.
2. Run the Python script to generate Powerball numbers.
3. Adjust constraints or weights in the code for customized results.

This project blends statistical modeling, programming, and exploratory analysis to delve into the fascinating intersection of randomness and patterns.
