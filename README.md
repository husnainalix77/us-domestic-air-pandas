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

## Analysis Tasks

| Task | Description | Technique |
|------|-------------|-----------|
| Task 2 | Flights operated by Boeing 737-800 | Merge + Boolean Filter |
| Task 6 | Total passengers per month | GroupBy + Sum |
| Task 9 | Airlines serving both JFK and LAX | Set Intersection + Merge |
| Task 11 | Airbus vs Boeing segment counts | str.contains() + Boolean Mask |
| Task 20 | Airport hub connectivity analysis | pd.concat() + GroupBy |

## Key Findings
- **Boeing dominates** US domestic traffic with 38,588 segments vs Airbus 18,053
- **March and May** are the busiest months with ~57.7 million passengers each
- **19 airlines** serve both JFK and LAX simultaneously
- **Minneapolis–St Paul (MSP)** is the most connected airport with 202 unique connections
- **Chicago O'Hare (ORD)** is MSP's busiest partner with 249 combined flight segments

## Tools Used
- Python 3.12
- Pandas
- NumPy
- Jupyter Notebook

## How to Run
1. Clone the repository
2. Place the four JSON data files in the same folder as the notebook
3. Run all cells from top to bottom

## Author
**Husnain Maroof**  
Mechatronics and Control Engineering  
University of Engineering & Technology, Lahore  
GitHub: [husnainalix77](https://github.com/husnainalix77)
