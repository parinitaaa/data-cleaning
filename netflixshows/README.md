# Netflix Data Cleaning Project

## Overview
This project focuses on cleaning and preparing the Netflix dataset (`dataset.csv`) for analysis. The dataset contains information about movies and TV shows, including titles, cast, director, country, release year, rating, duration, genres, and descriptions.

## Features
- Handle missing values in key columns (`director`, `cast`, `country`, `rating`, `duration`)
- Convert `date_added` to datetime and derive `year_added`
- Extract numeric values from `duration` and split into `duration_min` (movies) and `num_seasons` (TV shows)
- Clean and standardize text columns
- Split `listed_in` into a list of genres
- Add additional features like `num_cast`, `unknown_director`, and `unknown_country`

## Getting Started

### 1. Clone the repository
```bash
git clone <your-repo-url>
cd project-name
