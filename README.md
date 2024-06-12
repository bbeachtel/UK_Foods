# UK Food Standards Agency Ratings Analysis

This project analyzes food hygiene ratings data from the UK Food Standards Agency to assist the "Eat Safe, Love" magazine in determining focus areas for future articles. The project involves setting up a NoSQL database, updating it with new data, and performing exploratory data analysis.

## Project Overview

### Database Setup
- Imported data from `establishments.json` into a MongoDB database named `uk_food`, with a collection named `establishments`.
- Verified the database setup by listing databases and collections, and displaying a sample document.

### Database Updates
- Added a new restaurant, "Penang Flavours", to the database.
- Updated the restaurant document with the appropriate `BusinessTypeID`.
- Removed all documents related to the Dover Local Authority.
- Converted certain fields (latitude, longitude, RatingValue) to the correct data types.

### Exploratory Analysis
- Identified establishments with a hygiene score of 20.
- Found establishments in London with a RatingValue of 4 or higher.
- Determined the top 5 establishments with a RatingValue of 5, sorted by lowest hygiene score, near "Penang Flavours".
- Aggregated data to find the Local Authorities with the most establishments having a hygiene score of 0.

## Technologies Used
- **MongoDB:** For database management and data storage.
- **PyMongo:** To interact with MongoDB from Python.
- **Pandas:** For data manipulation and analysis.
- **Jupyter Notebook:** To document and run Python code interactively.
