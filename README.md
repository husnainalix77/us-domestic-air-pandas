# US Domestic Air Traffic Analysis 🛫

Analysis of US domestic air traffic data (January–May 2013) using Python and Pandas.

## Dataset
The dataset contains **136,000+ flight segments** across the United States, 
stored in four relational JSON files:

| File | Rows | Description |
|------|------|-------------|
| `flights.json` | 136,012 | Core flight segments data |
| `airlines.json` | 1,559 | Airline names and codes |
| `airports.json` | 6,267 | Airport names and IATA codes |
| `aircrafts.json` | 384 | Aircraft model names |

## Data Access
The dataset files are too large to host on GitHub directly.
Download all 4 JSON files from the link below and place them
in the same folder as the notebook before running.

📁 [Download Dataset from Google Drive](https://drive.google.com/drive/folders/1Mxlgx82MFGm6KPKu85ITm94suytDn8Ts?usp=sharing)

## Analysis Tasks

| Task | Description | Technique |
|------|-------------|-----------|
| Task 1 | Departures from Nashville International (BNA) | Merge + Boolean Filter |
| Task 2 | Flights operated by Boeing 737-800 | Merge + Boolean Filter |
| Task 3 | Maximum passengers in a single segment | idxmax() + Multiple Merges |
| Task 4 | Longest flight segment by distance | idxmax() + Two Merges |
| Task 5 | Airline with most flight segments | Merge + GroupBy + size() |
| Task 6 | Total passengers per month | GroupBy + Sum |
| Task 7 | Airlines serving Orlando (MCO) as destination | Merge + Filter + Unique |
| Task 8 | Aircraft types departing from Seattle (SEA) | Merge + Filter + Unique |
| Task 9 | Airlines serving both JFK and LAX | Set Intersection + Merge |
| Task 10 | High traffic airports (>1,000 segments) | pd.concat() + value_counts() |
| Task 11 | Airbus vs Boeing segment counts | str.contains() + Boolean Mask |
| Task 12 | Airlines operating both Boeing 737-800 and 737-900 | Set Intersection + Merge |
| Task 13 | Airlines in top 5 for both passengers and segments | GroupBy + nlargest() + Set Intersection |
| Task 14 | Airline with most diverse fleet | GroupBy + nunique() + Merge |
| Task 20 | Airport hub connectivity analysis | pd.concat() + GroupBy |

## Key Findings
- **Atlanta Hartsfield-Jackson** is the busiest airport with 8,489 total segments
- **Boeing dominates** US domestic traffic with 38,588 segments vs Airbus 18,053
- **Southwest Airlines** operated the most flight segments with 11,959 total
- **Delta Air Lines** has the most diverse fleet with **15 unique aircraft types**
- **Only 2 airlines** — Alaska Airlines and United Air Lines — operated both Boeing 737-800 and 737-900
- **3 airlines** — Delta, Southwest and United — rank in top 5 for both passengers and segments
- **March and May** are the busiest months with ~57.7 million passengers each
- **19 airlines** serve both JFK and LAX simultaneously
- **Hawaiian Airlines** carried the most passengers in a single segment — 82,812 on Kahului (OGG) → Honolulu (HNL) route in May
- **Honolulu (HNL) → New York JFK** is the longest domestic route at 4,983 miles
- **58 airports** handle more than 1,000 flight segments in this period
- **Minneapolis–St Paul (MSP)** is the most connected airport with 202 unique connections
- **Chicago O'Hare (ORD)** is MSP's busiest partner with 249 combined flight segments

## Tools Used
- Python 3.12
- Pandas
- Jupyter Notebook

## How to Run
1. Clone the repository
2. Download the dataset from Google Drive link above
3. Place all 4 JSON files in the same folder as the notebook
4. Run all cells from top to bottom

## Author
**Husnain Maroof**  
Mechatronics and Control Engineering  
University of Engineering & Technology, Lahore  
GitHub: [husnainalix77](https://github.com/husnainalix77)
