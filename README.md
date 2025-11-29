# New-York-City-Taxi-Trip-Data-Analysis-Project
# Software Project – Group N

**Authors:** Assima Amangeldina, Ceyla Kaya, Ziyi Dong, Sabina Nurseitova  
This project processes a NYC taxi dataset and implements multiple data analysis, sorting, and graph-based tasks using Python.


## 📂 Project Overview

This repository contains Python scripts that:

1. Load and preprocess taxi trip data  
2. Calculate descriptive statistics  
3. Compute trip speeds  
4. Count trips per pickup/dropoff zone  
5. Sort trip-related metrics using QuickSort and HeapSort  
6. Build and visualize a trip graph using NetworkX  
7. Identify connected components via DFS/BFS or NetworkX  


## 📁 File Structure

```text
read_file.py
calculate_stats.py
calculate_speed.py
count_trips.py
quick_sort.py
heap_sort.py
build_graph.py
zones.csv
dataset_small.txt
README.ipynb
```


## 🧩 Task 1 — Data Processing & Statistics

### 1. `read_file(file_path)`  
Parses `dataset_small.txt` and returns a structured list of dictionaries.

### 2. `calculate_stats(data)`  
Computes **min, max, and average** for:
- Number of passengers  
- Fare amount  
- Total amount  
- Tip amount  

### 3. `calculate_speed(data)`  
Computes trip speed in **km/h** from pickup/dropoff times and distances.

### 4. `count_trips(data, zones)`  
Counts the number of trips per pickup (or dropoff) zone using zone IDs mapped to zone names.


## 🧩 Task 2 — Sorting Algorithms

### 5. `quick_sort.py`  
- Uses a random pivot  
- Recursively partitions the data  
- Measures execution time for sorting different metrics (passengers, fare, total amount, tips, speed, time)

### 6. `heap_sort.py`  
- Builds a max-heap  
- Repeatedly extracts maximum values  
- Measures execution time on the same metrics


## 🧩 Task 3 — Graph Construction & Connected Components

### 7. `build_graph.py`  
- Uses NetworkX and Matplotlib  
- Nodes represent pickup and dropoff locations  
- Edge weights correspond to number of trips between locations (thicker edge = more trips)  
- Identifies connected components either via NetworkX built-ins or manual DFS/BFS.


## ⚙️ Requirements

Install dependencies (example):

```bash
pip install networkx matplotlib
```

Standard libraries used include:
- `csv`  
- `datetime`  


## ▶️ Running the Code

From the project directory, run:

```bash
python read_file.py
python calculate_stats.py
python calculate_speed.py
python count_trips.py
python quick_sort.py
python heap_sort.py
python build_graph.py
```


## 📝 Notes

- All data comes from `dataset_small.txt`.  
- Sorting algorithms are used to compare performance on multiple numerical features.  
- The graph visualization helps understand relationships between taxi zones.
