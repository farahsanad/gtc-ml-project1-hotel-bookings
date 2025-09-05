# Hotel Booking Cancellations – Data Cleaning & Preparation

This project is a Jupyter Notebook (`Project1.ipynb`) that walks through **data preprocessing** and **feature preparation** for predicting hotel booking cancellations.  
It is based on the [Hotel Booking Demand Dataset](https://www.sciencedirect.com/science/article/pii/S2352340918315191).

---

## 📌 Project Overview
The notebook demonstrates:
- Cleaning and handling missing values
- Managing high-cardinality features (e.g., `country`) using:
  - Frequency encoding  
  - Grouping rare labels into `"Other"`
- Avoiding **data leakage** by dropping `reservation_status` and `reservation_status_date`
- Selecting meaningful features for prediction
- Splitting the dataset into **train** and **test** sets (80/20)

---

## ⚙️ Features Used
From the full dataset, the following columns are selected as predictors:

- `is_repeated_guest`  
- `previous_cancellations`  
- `previous_bookings_not_canceled`  
- `reserved_room_type`  
- `assigned_room_type`  
- `booking_changes`  
- `deposit_type`  
- `days_in_waiting_list`  
- `customer_type`  
- `stays_in_week_nights`

**Target column**:  
- `is_canceled` (1 = canceled, 0 = not canceled)

---

## 🛠️ Tech Stack
- Python 3.x  
- Pandas  
- NumPy  
- scikit-learn  

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/your-repo-name.git
   cd your-repo-name
