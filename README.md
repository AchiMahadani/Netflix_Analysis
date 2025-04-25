# 📊 Netflix Data Analysis with PostgreSQL & Jupyter

This project presents a detailed analysis of Netflix titles data using **PostgreSQL** and **Jupyter Notebook**, connected through **SQLAlchemy**.

## 📁 Dataset

- The dataset used in this project is a single CSV file containing information about Netflix titles including type, director, cast, country, genre, date added, and more.

## 🛠️ Tools & Technologies

- **Jupyter Notebook**: For interactive data analysis .
- **PostgreSQL**: Used as the main relational database
- **SQLAlchemy**: To connect PostgreSQL with Python for executing queries inside Jupyter

## 🔄 Preprocessing Steps

1. **Duplicate Removal**: Cleaned the dataset to remove exact and partial duplicates based on key attributes like `title`, `show_id`, etc.
2. **Table Creation**: Derived multiple tables such as `netflix_directors`, `netflix_cast`, `netflix_genres`, and `netflix_countries` based on string-split logic for multi-valued fields.
3. **Normalization**: Transformed comma-separated values in columns like `cast`, `listed_in`, `country`, and `director` into separate rows to allow accurate filtering and aggregation.

## 📌 Key Insights and SQL Queries

The following insights were derived through SQL queries:

1. **Movies vs TV Shows per Director**  
   Count of Movies and TV Shows directed by each individual who has done both.

2. **Top Country in Comedy Movies**  
   Which country has produced the highest number of comedy movies on Netflix.

3. **Top Directors per Year**  
   For each year (based on date added), the director with the highest number of movie releases.

4. **Average Duration per Genre**  
   Calculated the average duration of movies in each genre.

5. **Directors in Horror & Comedy**  
   Identified directors who have directed both horror and comedy movies.

6. **Actors in Both Action and Comedy**  
   Found actors who have worked in both 'Action' and 'Comedy' genres.



