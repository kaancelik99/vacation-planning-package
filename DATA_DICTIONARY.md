# Data Dictionary

This data dictionary provides descriptions of all variables included in the **Flights** and **Hotels** datasets used in the Vacation Planning Package project.

---

## ✈️ Flights Dataset

| Column                            | Description                                                                 | Data Type       | Example                     |
|-----------------------------------|-----------------------------------------------------------------------------|-----------------|-----------------------------|
| `from_airport_code`               | IATA code of the departure airport                                          | String          | `JFK`                       |
| `from_country`                    | Country of the departure airport                                            | String          | `United States`             |
| `dest_airport_code`               | IATA code of the destination airport                                        | String          | `LAX`                       |
| `dest_country`                    | Country of the destination airport                                          | String          | `United States`             |
| `aircraft_type`                   | Model or type of aircraft used for the flight                               | String          | `Boeing 737`                |
| `airline_number`                  | Numeric identifier assigned to the airline                                  | String          | `DL`                        |
| `airline_name`                    | Name of the airline operating the flight                                    | String          | `[Delta]`                   |
| `flight_number`                   | Unique flight number (may include airline code)                             | String          | `DL456`                     |
| `departure_time`                  | Scheduled departure time                                                    | Datetime/String | `6/1/2023 14:30`            |
| `arrival_time`                    | Scheduled arrival time                                                      | Datetime/String | `6/1/2023 17:45`            |
| `duration`                        | Duration of the flight in minutes                                           | Integer         | `195`                       |
| `stops`                           | Number of stops on the flight (0 = nonstop)                                 | Integer         | `0`                         |
| `price`                           | Price of the flight                                                         | Float           | `250.00`                    |
| `currency`                        | ISO 4217 currency code                                                      | String          | `USD`                       |
| `co2_emissions`                   | Estimated carbon dioxide emissions for the flight                           | Float           | `150.5`                     |
| `avg_co2_emission_for_this_route` | Average CO2 emissions for this route                                        | Float           | `140.0`                     |
| `co2_percentage`                  | % difference from average route emissions                                   | String (%)      | `-3%`                       |
| `scan_date`                       | Date the flight data was retrieved or last updated                          | Datetime/String | `5/31/2023 15:30`           |

---

## 🏨 Hotels Dataset

| Column            | Description                                                            | Data Type | Example                                             |
|-------------------|------------------------------------------------------------------------|-----------|-----------------------------------------------------|
| `countyCode`      | Unique identifier code for the Country (column misspelled)             | String    | `US`                                                |
| `countyName`      | Name of the Country (column misspelled)                                | String    | `United States`                                     |
| `cityCode`        | Unique identifier code for the City                                    | Integer   | `100328`                                            |
| `cityName`        | Location of hotel in City,   State format                              | String    | `Abbeville,   Louisiana`                            |
| `HotelCode`       | Unique identifier code for the hotel                                   | Integer   | `1125999`                                           |
| `HotelName`       | Name of the hotel                                                      | String    | `Budget Inn & Suites`                               |
| `HotelRating`     | Rating of the hotel (out of 5 stars, All = 0 stars)                    | String    | `TwoStar`                                           |
| `Address`         | Street address of the hotel                                            | String    | `2115 Charity Street AbbevilleLouisiana 70510`      |
| `Attractions`     | Notable nearby attractions or landmarks                                | String    | `Distances are displayed...`                        |
| `Description`     | Description or summary of the hotel and its offerings                  | String    | `Offering a free continental breakfast...`          |
| `FaxNumber`       | Fax number of the hotel                                                | String    | `+13378981463`                                      |
| `HotelFacilities` | List of available facilities or services                               | String    | `shared lounge/TV area...`                          |
| `Map`             | Geocoordinates for hotel location                                      | String    | `29.9806|-92.11452`                                |
| `PhoneNumber`     | Contact phone number                                                   | String    | `+13378981453`                                      |
| `PinCode`         | Postal or ZIP code of the hotel location (some include state code)     | String    | `LA 70510`                                          |
| `HotelWebsiteUrl` | Official website URL of the hotel                                      | String    | `https://www.booking.com/city/us/abbeville-us.html` |

---



