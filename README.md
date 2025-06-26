# ✈️ Vacation Planning Package: Flight Affordability & Hotel Quality

This project analyzes two datasets—U.S. domestic flight data and hotel information—to build a **data-driven vacation planning tool**. The goal is to recommend an ideal vacation package based on affordable flights and high-quality hotel accommodations.

---

## 🧭 Project Overview

The notebook walks through the following steps:

1. **Data Loading & Inspection** – Import flight and hotel datasets.
2. **Filtering & Cleaning** – Align flight destinations with hotel cities and remove irrelevant entries.
3. **City-Level Aggregation** – Calculate average hotel ratings and flight prices per city.
4. **Detailed Case Study** – Compare flight and hotel options for a selected destination.
5. **Final Decision-Making** – Select the best city-hotel pairing based on data insights.

---

## 📊 Selection Criteria

### Destinations
- **Minimum Volume**: City, State must have at least **16,000 flights** and **800 hotels**.
- **Top Performers**: City, State must rank in the **top 3** for both flight affordability and hotel rating.

### Flights
- **Origin**: Must depart from outside the U.S.
- **Destination**: U.S. city with matching hotel data.
- **Affordability**: Round-trip flights should cost **under $200**.
- **Convenience**: **Direct flights** are preferred.
- **Timing**: **Summer travel months** are prioritized.

### Hotels
- **Location Match**: Must correspond with flight destination.
- **Quality Threshold**: **5-star hotels** with strong review scores are prioritized.
- **Cost Balance**: Hotel cost is considered in relation to flight price for overall budget optimization.

---

## 🧾 Data Sources

- **Flights Dataset**: `flight_data_usa.csv`
- **Hotels Dataset**: `hotels_usa.csv`

Each dataset includes key variables like:
- City & State
- Flight price, stops, and timing
- Hotel star ratings and customer reviews

---

## 📌 Example Result

✅ **Selected Package**:

- **Flight**: Bogotá to Miami (Direct, August, <$200)  
- **Hotel**: The W South Beach (5 stars, high review score)

---

## 🔧 Requirements

To run this project:

pip install pandas jupyter matplotlib seaborn

Then launch the notebook:

jupyter notebook notebooks/flights_hotels_analysis.ipynb

---

📁 Folder Structure

vacation-planning-package/
├── data/
│   ├── flight_data_usa.csv
│   └── hotels_usa.csv
├── notebooks/
│   └── flights_hotels_analysis.ipynb
└── README.md

---

📬 Contact
For questions, suggestions, or collaboration inquiries, please reach out to Salim Kaan Celik.

🌐 GitHub
Explore the full repository: Vacation Planning Package