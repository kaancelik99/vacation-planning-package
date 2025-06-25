# ✈️ Vacation Planning Package: Flight Affordability & Hotel Quality

This project analyzes two datasets—U.S. domestic flight data and hotel information—to build a **data-driven vacation planning tool**. The goal is to recommend a vacation package based on **affordable flights** and **high-quality hotel accommodations**.

## 🧭 Project Overview

This notebook walks through the following steps:

1. **Data Loading & Inspection**: Import flight and hotel datasets.
2. **Filtering & Cleaning**: Align flight destinations with hotel cities and remove irrelevant entries.
3. **City-Level Aggregation**: Calculate average hotel ratings and average flight prices per city.
4. **Detailed Case Study**: Compare multiple flight and hotel options for a specific destination.
5. **Final Decision-Making**: Select the best pairing based on price, rating, and availability.

## 📊 Selection Criteria

### Destination City
- **Minimum Frequency of Flights and Hotles**: City, State must have at least 16,000 flights and 800 hotels.
- **Top 3 in Flight Price and Hotel Rating**: City, State must measure in the top 3 among both flight price and hotel rating averages.

### Flights
- **Origin**: Must depart from outside the U.S.
- **Destination**: Must be a U.S. city with available hotel data.
- **Affordability**: Prioritize round-trip flights under **$200**.
- **Convenience**: Direct flights preferred.
- **Travel Window**: Summer months are prioritized.

### Hotels
- **Location Match**: City, State must correspond to flight destination.
- **Quality Threshold**: **5-star rating** preferred.
- **Price Awareness**: Balanced against flight cost for overall budget optimization.

## 🧾 Data Sources

- **Flights Dataset**: `flight_data_usa.csv`  
- **Hotels Dataset**: `hotels_usa.csv`

These datasets include information like city, state, flight prices, number of stops, hotel star ratings, and customer review scores.

## 📌 Example Result

> ✅ Selected Package:  
> - **Flight**: Bogotá to Miami (Direct, August, <$200)  
> - **Hotel**: The W South Beach (5 stars, high review score)  

## 🔧 Requirements

To run this project:

```bash
pip install pandas jupyter
```

Then launch the notebook:

```bash
jupyter notebook capstone_analysis.ipynb
```

## 📁 Folder Structure

```
project/
│
├── data/
│   ├── flight_data_usa.csv
│   └── hotels_usa.csv
│
├── notebooks/
│   └── capstone_analysis.ipynb
│
└── README.md
```

## 📬 Contact

For questions or suggestions, reach out to [Salim Kaan Celik](mailto:celik1999@gmail.com).
