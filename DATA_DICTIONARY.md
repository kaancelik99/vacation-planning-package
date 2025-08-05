# Data Dictionary

This data dictionary provides descriptions of all variables included in the **Flights** and **Hotels** datasets used in the Vacation Planning Package project.

---

## ✈️ Flights Dataset

| Column                            | Description                                                                 | Data Type       | Example                     |
|-----------------------------------|-----------------------------------------------------------------------------|------------------|-----------------------------|
| `from_airport_code`              | IATA code of the departure airport                                          | String           | `JFK`                       |
| `from_country`                   | Country of the departure airport                                            | String           | `United States`             |
| `dest_airport_code`              | IATA code of the destination airport                                        | String           | `LAX`                       |
| `dest_country`                   | Country of the destination airport                                          | String           | `United States`             |
| `aircraft_type`                  | Model or type of aircraft used for the flight                               | String           | `Boeing 737`                |
| `airline_number`                 | Numeric identifier assigned to the airline                                  | Integer          | `1234`                      |
| `airline_name`                   | Name of the airline operating the flight                                    | String           | `Delta Air Lines`           |
| `flight_number`                  | Unique flight number (may include airline code)                             | String           | `DL456`                     |
| `departure_time`                 | Scheduled departure time (ISO 8601 format or datetime string)               | Datetime/String  | `2023-06-01T14:30:00Z`      |
| `arrival_time`                   | Scheduled arrival time (ISO 8601 format or datetime string)                 | Datetime/String  | `2023-06-01T17:45:00Z`      |
| `duration`                       | Duration of the flight in hours and minutes                                 | String           | `3h 15m`                    |
| `stops`                          | Number of stops on the flight (0 = nonstop)                                 | Integer          | `0`                         |
| `price`                          | Price of the flight                                                         | Float            | `250.00`                    |
| `currency`                       | ISO 4217 currency code                                                      | String           | `USD`                       |
| `co2_emissions`                  | Estimated carbon dioxide emissions for the flight (kg)                      | Float            | `150.5`                     |
| `avg_co2_emission_for_this_route` | Average CO2 emissions for this route (kg)                                   | Float            | `140.0`                     |
| `co2_percentage`                 | % difference from average route emissions (100 = average)                   | Float (%)        | `107.5`                     |
| `scan_date`                      | Date the flight data was retrieved or last updated                          | Date             | `2024-07-15`                |

---

## 🏨 Hotels Dataset

| Column            | Description                                                            | Data Type | Example                          |
|-------------------|------------------------------------------------------------------------|-----------|----------------------------------|
| `countyCode`      | Unique identifier code for the county                                  | String    | `001`                            |
| `countyName`      | Name of the county                                                     | String    | `Orange County`                  |
| `cityCode`        | Unique identifier code for the city                                    | String    | `OC123`                          |
| `cityName`        | Name of the city                                                       | String    | `Orlando`                        |
| `HotelCode`       | Unique identifier for the hotel                                        | String    | `H456`                           |
| `HotelName`       | Name of the hotel                                                      | String    | `Grand Beach Resort`             |
| `HotelRating`     | Rating of the hotel (e.g., out of 5 stars)                             | Float     | `4.5`                            |
| `Address`         | Street address of the hotel                                            | String    | `123 Ocean Dr, Orlando, FL`      |
| `Attractions`     | Notable nearby attractions or landmarks                                | String    | `Theme Parks, Beaches`           |
| `Description`     | Description or summary of the hotel and its offerings                  | String    | `Beachfront property with spa`   |
| `FaxNumber`       | Fax number of the hotel                                                | String    | `+1-555-123-4567`                |
| `HotelFacilities` | List of available facilities or services                               | String    | `Pool, Free WiFi, Gym`           |
| `Map`             | URL or embedded map link for hotel location                            | String    | `https://maps.example.com/h123`  |
| `PhoneNumber`     | Contact phone number                                                   | String    | `+1-555-987-6543`                |
| `PinCode`         | Postal or ZIP code of the hotel location                               | String    | `32801`                          |
| `HotelWebsiteUrl` | Official website URL of the hotel                                      | String    | `http://www.grandbeachresort.com` |

---

_Last updated: August 5, 2025_
