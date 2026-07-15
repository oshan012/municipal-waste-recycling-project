# 🌍 Municipal Waste and Recycling Efficiency

An end-to-end data analysis project exploring municipal waste and recycling trends across countries, using real-world datasets from **Our World in Data** and **Eurostat**.

## 📌 Project Overview

This project combines database design, SQL, data analysis, and machine learning to answer a simple question: *how has global recycling efficiency changed over time, and which countries lead the way?*

**Key findings:**
- 🇰🇷 **Korea** has the highest municipal recycling rate globally, at nearly **60%**
- 🇩🇪 **Germany** ranks second, at nearly **47%**
- 📈 Global recycling rates have been **steadily increasing since 1990**
- 🔮 A linear regression model (97% accuracy) predicts the global recycling rate will reach **~33.78% by 2028**

## 🛠️ Tools & Skills Used

- **Database Design:** Designed a normalized relational schema (ER diagram) with 4 linked entities
- **SQLite:** Built and queried a relational database
- **Python / Pandas:** Cleaned and loaded raw CSV data into SQL tables
- **SQL:** Wrote queries to aggregate and rank countries by recycling performance
- **scikit-learn:** Trained a linear regression model to forecast recycling trends
- **Matplotlib / Seaborn:** Visualized trends and model predictions

## 🗂️ Database Schema

The project uses a relational database with the following structure:

| Table | Description |
|---|---|
| `countries` | Country metadata (name, region, income group) |
| `income_groups` | World Bank income classification |
| `waste_production` | Waste generated per capita, by country and year |
| `recycling_rates` | Recycling rate (%), by country and year |

See [`diagrams/ER_Diagram.drawio`](diagrams/ER_Diagram.drawio) for the full entity-relationship diagram (open with [draw.io](https://app.diagrams.net/)).

## 📁 Repository Structure

```
├── notebooks/
│   ├── 01_data_loading_and_analysis.ipynb   # Data loading, SQL queries, ML model, visualizations
│   └── 02_database_schema.ipynb             # SQLite table creation (schema definitions)
├── diagrams/
│   └── ER_Diagram.drawio                    # Entity-relationship diagram
├── data/                                    # Raw datasets (see note below)
└── Project_Summary.pdf                      # One-page project summary
```

> **Note:** Raw CSV source files (from Our World in Data / Eurostat) are not included in this repo. Add them to the `data/` folder to fully reproduce the notebooks.

## 📊 Data Sources

- [Our World in Data — Municipal Waste & Recycling](https://ourworldindata.org/)
- [Eurostat](https://ec.europa.eu/eurostat)
- World Bank Income Group Classifications

## 🚀 What I Learned

Through this project I learned how to:
- Design and normalize a relational database schema
- Create an SQLite database and write SQL queries for aggregation and analysis
- Perform data cleaning and transformation with Pandas
- Build and evaluate a machine learning model with scikit-learn
- Visualize data effectively using matplotlib and seaborn

---
*Part of my studies in Sustainable Resources Engineering and Management at Hochschule Magdeburg-Stendal.*
