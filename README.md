# NYC Airbnb Market Analysis
**Exploratory Data Analysis | Python | Pandas | Plotly**

An end-to-end EDA identifying what drives listing prices, which boroughs offer the best value, and where new hosts should list to maximize bookings.


### The Goal
This project tries to answers 4 business questions on listings:
1. What drives listing prices in NYC?
2. Which neighbourhoods offer the best value?
3. What separates high-performing hosts from low-performing ones?
4. Where should a new host list their property to maximize bookings?

### Data
**Source:** [NYC Airbnb Open Data — Kaggle](https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data)  
**Size:** 48,595 listings × 14 columns (after cleaning)  
**Coverage:** All 5 NYC boroughs — Manhattan, Brooklyn, Queens, Bronx, Staten Island


### Key findings:
- **Room type** is the strongest price driver — entire apartments average $194/night vs $85 for private rooms
- **Brooklyn** offers the best value — lower median price than Manhattan with comparable upside
- **Established hosts** (2–5 listings) generate more reviews/month than power hosts despite managing fewer properties
- **Queens, Bronx, and Staten Island** hold only 15% of listings — lowest competition for new hosts


### Methodology
1. **Data Cleaning** — handled missing values, removed outliers ($10–$1,000 price range), fixed dtypes
2. **Feature Engineering** — built 5 new features including host tier classification and days since last review
3. **Univariate Analysis** — price, room type, and neighbourhood distributions
4. **Bivariate Analysis** — price vs borough, room type, and host tier
5. **Geographic Analysis** — interactive maps of price distribution and borough density

### Tech stack
Project entirely written in the Jupyter notebook. 
Libraries used: pandas, numpy, matplotlib.pyplot, seaborn, plotly.express

### Project structure:
airbnb-nyc-eda/
├── data/
│   └── listings.csv        
├── notebooks/
│   └── airbnb_eda.ipynb    
├── visuals/ 
│   └── visuals .png, .html(for maps)             
├── reports/                
│   └── report.pdf
└── README.md

### How to run:
1. Download or copy this repository
2. Be sure, that all necessary libraries are downloaded. 
    To check it run in the terminal " pip install pandas numpy matplotlib seaborn plotly folium "
3. Open the Jupyter notebook in the ./notebooks/airbnb_eda.ipynb
4. Connect to the local or online kernel, and run all cells (or just scroll through all cells, since everything is already ran)