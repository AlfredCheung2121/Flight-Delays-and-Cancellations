# Flight Delays and Cancellations Analysis

A comprehensive data analysis project examining the relationships and patterns in flight delay times using airline data from 2015.

## 📊 Project Overview

This project analyzes flight delay patterns and their relationships with various factors such as time, airlines, and flight characteristics. The analysis focuses on understanding what factors contribute to flight delays and identifying patterns in delay times across different dimensions.

## 🎯 Objectives

- Analyze the relationship between different variables and delay times
- Identify seasonal patterns in flight delays
- Examine airline performance differences
- Investigate the correlation between flight distance and delays
- Create comprehensive visualizations to understand delay patterns

## 📁 Dataset Structure

The project uses three main datasets:

### 1. Flights Dataset (`flights.csv`)
- **Size**: Over 5.8 million flight records from 2015
- **Key Variables**:
  - `YEAR`, `MONTH`, `DAY`, `DAY_OF_WEEK`: Flight dates
  - `AIRLINE`: US DOT airline identification code
  - `ORIGIN_AIRPORT`, `DESTINATION_AIRPORT`: IATA airport codes
  - `SCHEDULED_DEPARTURE`, `SCHEDULED_ARRIVAL`: Planned departure/arrival times
  - `DEPARTURE_TIME`, `ARRIVAL_TIME`: Actual departure/arrival times
  - `DEPARTURE_DELAY`, `ARRIVAL_DELAY`: Delay in minutes from scheduled times
  - `DISTANCE`: Flight distance in miles
  - `FLIGHT_NUMBER`, `TAIL_NUMBER`: Flight identification details

### 2. Airlines Dataset (`airlines.csv`)
- Contains airline IATA codes and full airline names
- Maps airline codes to readable airline names

### 3. Airports Dataset (`airports.csv`)
- Comprehensive airport information including:
  - IATA codes, airport names, cities, states
  - Geographic coordinates (latitude/longitude)
  - Country information

## 🔍 Analysis Approach

### Data Quality Assurance
- **Delay Calculation Verification**: Validated that recorded delays match calculated differences between scheduled and actual times
- **Data Cleaning**: Removed rows with incorrect delay calculations and missing values
- **Final Dataset**: 3,460,894 clean flight records after quality filtering

### Analysis Components

#### 1. Monthly Delay Patterns
- **Focus**: Seasonal variations in flight delays
- **Key Findings**:
  - September shows best performance (negative delays = early arrivals)
  - June has highest departure delays
  - Overall system shows slight early arrivals on average

#### 2. Airline Performance Comparison
- Comparative analysis of delay patterns across different airlines
- Identification of consistently performing vs. problematic carriers

#### 3. Distance vs. Delay Relationship
- Investigation of correlation between flight distance and delay likelihood
- Understanding if longer flights are more prone to delays

## 📈 Key Findings

### Overall Statistics
- **Total Flights Analyzed**: 3,460,894
- **Average Departure Delay**: 0.27 minutes (essentially on-time)
- **Average Arrival Delay**: -4.46 minutes (early arrivals on average)

### Monthly Performance Highlights
- **Best Month**: September (early arrivals by 6 minutes on average)
- **Worst Month**: June (highest departure delays)
- **Peak Travel**: October (309,117 flights)
- **Lowest Travel**: February (237,155 flights)

## 🛠️ Technical Implementation

### Tools Used
- **Python**: Primary analysis language
- **Pandas**: Data manipulation and analysis
- **Matplotlib & Seaborn**: Data visualization
- **NumPy**: Numerical computations
- **Jupyter Notebook**: Interactive analysis environment

### Key Functions
- `analyze_flight_delays()`: Monthly delay statistics calculation
- `create_comprehensive_visualization()`: Multi-panel visualization suite
- `print_summary_statistics()`: Detailed performance reporting

## 📊 Visualizations

The analysis includes comprehensive visualizations:
- **Line Charts**: Monthly delay trends
- **Bar Charts**: Side-by-side delay comparisons
- **Box Plots**: Delay distribution analysis
- **Flight Count Charts**: Volume patterns by month
- **Summary Tables**: Key performance metrics

## 🚀 Getting Started

1. **Clone the repository**
2. **Install dependencies**:
   ```bash
   pip install pandas matplotlib seaborn numpy jupyter
   ```
3. **Open the Jupyter notebook**: `Untitled-1.ipynb`
4. **Run the analysis**: Execute cells sequentially

## 📝 Project Structure

```
Flight-Delays-and-Cancellations/
├── airline_dataset/
│   ├── airlines.csv          # Airline information
│   ├── airports.csv          # Airport details
│   └── flights.csv           # Main flight data (5.8M+ records)
├── Untitled-1.ipynb          # Main analysis notebook
└── README.md                 # This file
```

## 🔬 Data Insights

### Delay Patterns by Month
- **Winter Months** (Dec-Feb): Moderate delays, fewer flights
- **Spring** (Mar-May): Stable performance, increasing volume
- **Summer** (Jun-Aug): Peak travel, higher delays
- **Fall** (Sep-Nov): Best performance, high volume

### System Performance
- The aviation system shows remarkable efficiency with early arrivals on average
- Seasonal patterns clearly visible with summer months showing increased delays
- September emerges as the optimal travel month for punctuality

## 📋 Future Enhancements

- [ ] Weather data integration for delay correlation
- [ ] Airport-specific delay analysis
- [ ] Route-specific delay patterns
- [ ] Machine learning models for delay prediction
- [ ] Interactive dashboard development

## 🤝 Contributing

This is an educational data analysis project. Feel free to use the code and insights for your own analysis or learning purposes.

## 📄 License

This project is for educational and research purposes.