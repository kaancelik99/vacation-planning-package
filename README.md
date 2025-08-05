# ✈️ Vacation Planning Package: Flight Affordability & Hotel Quality

This project leverages **Python data analysis** tools to evaluate U.S. domestic flight prices and hotel quality ratings. The goal is to help users make smarter, data-driven decisions when planning a vacation by identifying cities that offer both affordable flights and highly rated hotels.

---

## 🗂️ Data Sources

Here are the datasets that were used for this project. Since these datasets were too large to upload to GitHub, this project limits the data to analyze flights to the US and hotels in the US.
- Flights: https://www.kaggle.com/datasets/polartech/flight-data-with-1-million-or-more-records
- Hotels: https://www.kaggle.com/code/raghavmaheshwarii/hotels-dataset

---

## 📌 Project Objective

Build an interactive vacation planning tool using real-world datasets to identify optimal city-hotel combinations based on:

- Low round-trip flight prices from international origins
- High hotel star ratings and customer reviews
- Matching city and state destinations for alignment

---

## 🧰 Tools & Technologies Used

| Tool / Library       | Purpose                                      |
|----------------------|----------------------------------------------|
| `pandas`             | Data cleaning, transformation, and grouping |
| `matplotlib`         | Static visualization                        |
| `seaborn`            | Enhanced scatter plots                      |
| `plotly`             | Interactive visualizations                  |
| `sqlite3`            | SQL-style data joining within Python        |
| `Jupyter Notebook`   | Exploratory analysis environment            |
| `Python 3.x`         | Core programming language                   |

---

## 🧭 Workflow Overview

The project workflow follows these key steps:

1. **Data Loading & Inspection**  
   Load and preview datasets using `pandas`.

2. **Filtering & Cleaning**  
   - Align city and state between flights and hotels.
   - Remove duplicates and null entries.
   - Standardize city naming formats.

3. **City-Level Aggregation**  
   - Group data by `City, State` to compute:
     - Average flight prices
     - Average hotel ratings

4. **Relational Data Join Using SQLite**  
   - Use the `sqlite3` library to simulate a relational database join.
   - Merge the flight and hotel datasets by matching city and state values.
   - Execute SQL queries within the notebook to filter and rank destinations.

5. **Selection Logic & Thresholds**  
   - Filter cities with at least 16,000 flights and 800 hotels.
   - Select cities ranking in the top 3 for both affordability and hotel quality.

6. **Case Study & Visualization**  
   - Plot relationships between hotel ratings and flight prices.
   - Drill into specific vacation routes (e.g., Bogotá → Miami).

---

## 📊 Selection Criteria

### Destinations
- Must be a U.S. city with:
  - **≥ 16,000 flights**
  - **≥ 800 hotels**
- Must rank in the **top 3** for:
  - Lowest average flight price
  - Highest average hotel rating

### Flights
- **Origin**: Must depart from outside the U.S.
- **Destination**: Valid U.S. city with hotel data
- **Budget**: Round-trip price under **$200**
- **Convenience**: Direct flights preferred
- **Timing**: Summer months prioritized

### Hotels
- Must match the flight's destination city
- 5-star or near-5-star ratings prioritized
- Review scores factored into quality
- Price considered in overall trip cost

---

## 🗂️ Folder Structure & 🛠 How to Run

```
vacation-planning-package/
├── data/
│   ├── flight_data_usa.csv
│   └── hotels_usa.csv
├── notebooks/
│   └── flights_hotels_analysis.ipynb
└── README.md
```

---

## 🔧 Setup Instructions

1. **Clone the repository**:

git clone https://github.com/kaancelik99/vacation-planning-package.git

cd vacation-planning-package

2. **Set Up the Virtual Environment**:

python -m pip install virtualenv

python -m venv venv

source venv/bin/activate      # On Mac/Linux

venv\Scripts\activate         # On Windows

pip install -r requirements.txt

3. **Install required libraries**:

pip install pandas matplotlib seaborn jupyter plotly

4. **Launch the notebook**:

notebooks/flights_hotels_analysis.ipynb

---

## 📈 Visualizations

- Tableau Public Link: https://public.tableau.com/app/profile/kaan.celik5338/viz/vacation_planning_package/Dashboard1

Flights Map: Represents all flight routes, connecting origin and destination locations, including price and frequency.

Number of Hotels by State: Represents hotel quantity standards for target area.

Average Hotel Rating by State: Represents hotel quality standards for target area.

---

## 📌 Final Result
✅ Selected Vacation Package:

Flight: Bogotá → Miami: Direct, August departure, Round-trip under $200

Hotel: The W South Beach, 5 stars, High customer reviews

This pairing meets both cost and quality thresholds.

Created ad.html to advertise the vacation package to the target market, in Spanish.

---

## 💬 Contact
For questions, collaboration, or feedback, feel free to contact:

Salim Kaan Celik
📧 Email: celik1999@gmail.com

