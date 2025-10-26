# Metro Schedule Optimization on Istanbul M2 Line using Genetic Algorithms

This project presents a simulation-based optimization model to minimize passenger waiting times on Istanbul's M2 metro line using genetic algorithms. Real-world data was sourced from the Istanbul Metropolitan Municipality (İBB), and the model simulates daily passenger traffic to improve scheduling.

---

## Project Overview

- **Objective**: Minimize the average passenger waiting time by optimizing daily train departure times.
- **Method**: Genetic Algorithm (GA) tailored to metro scheduling with real constraints.
- **Data Source**: Istanbul Metropolitan Municipality Open Data Portal  
- **Focus Line**: M2 Metro Line (Yenikapı → Hacıosman)  
- **Average Waiting Time Improved**: From 3.65 min ⟶ 3.23 min (⬇ ~11.5%)

---

## Files

- `PRE-OPTIMIZATION.ipynb`: Preprocessing and demand analysis of İBB data  
- `OPTIMIZATION.ipynb`: Full implementation of GA and simulation  
- `Report.pdf`: Final project report, includes methodology, figures, and results

---

## Technical Details

###  Genetic Algorithm Design
- **Individuals**: 196 departure times (06:00–23:59)
- **Fitness**: Mean waiting time of all passengers
- **Constraints**:
  - Max 15 minutes between consecutive departures
  - Total trips = 196 (fixed, no extra trains)
  - Capacity ≤ 950 passengers/train
- **Hyperparameters**:
  - Population: 30
  - Generations: 40
  - Mutation rate: 0.15

###  Results
- **Baseline average waiting time**: 3.65 min  
- **Optimized average waiting time**: 3.23 min  
- **Improvement**: ~11.5%  
- Significantly better performance during evening rush hours  
- Lower variance and more balanced distribution of waiting times

---

## Data Sources

- [İBB Open Data Portal](https://data.ibb.gov.tr)  
- Metro Istanbul Timetable, Passenger Boarding Data, Vehicle Specs

---

## Authors

- **Berker Eriş** – Artificial Intelligence and Data Engineering, ITU  
- **Enes Yemenli** – Artificial Intelligence and Data Engineering, ITU  

> Contact: berkereris1@gmail.com
> Contact: yemenli22@itu.edu.tr


---



