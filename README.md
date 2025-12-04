# Analyzing Students' Mental Health

A data analysis project examining the mental health of international students using PostgreSQL.

## Overview

This project analyzes data from a 2018 survey conducted by a Japanese international university on student mental health. The study, published in 2019 and approved by several ethical and regulatory boards, found that international students face higher risks of mental health difficulties compared to the general population.

**Key Findings from the Study:**
- International students have elevated mental health risks
- Social connectedness (belonging to a social group) is predictive of depression
- Acculturative stress (stress from adapting to a new culture) is predictive of depression

## Project Objective

Using PostgreSQL, this project explores whether:
1. Similar conclusions can be drawn for international students in this dataset
2. Length of stay is a contributing factor to mental health outcomes

## Dataset

The `students.csv` dataset contains 286 student records with 50 variables including:

| Field | Description |
|-------|-------------|
| `inter_dom` | Student type (international or domestic) |
| `japanese_cate` | Japanese language proficiency |
| `english_cate` | English language proficiency |
| `academic` | Academic level (undergraduate or graduate) |
| `age` | Current age |
| `stay` | Length of stay in years |
| `todep` | Total depression score (PHQ-9 test) |
| `tosc` | Total social connectedness score (SCS test) |
| `toas` | Total acculturative stress score (ASISS test) |

## SQL Analysis Tasks

The analysis involved writing a PostgreSQL query to:

- [x] Return a table with **nine rows** and **five columns**
- [x] Create five aliased columns: `stay`, `count_int`, `average_phq`, `average_scs`, and `average_as`
- [x] Calculate average scores for:
  - Depression (`todep` - PHQ-9 test)
  - Social connectedness (`tosc` - SCS test) 
  - Acculturative stress (`toas` - ASISS test)
- [x] Round all averages to **two decimal places**
- [x] Count the number of international students (`count_int`) for each length of stay
- [x] Group results by length of stay
- [x] Sort results by length of stay in **descending order**

## Key Results

The analysis revealed patterns in mental health metrics across different lengths of stay for international students:
- Students with longer stays (8-10 years) showed lower average depression scores
- Social connectedness scores varied across different stay durations
- Acculturative stress trends were observable across the length of stay spectrum

## Files

- `notebook.ipynb` - Jupyter notebook containing the SQL query and analysis
- `students.csv` - Dataset with student mental health survey responses
- `README.md` - Project documentation

## Technologies Used

- PostgreSQL
- Jupyter Notebook
- DataCamp DataLab

## Source

This project was completed as part of DataCamp's data analysis curriculum.
