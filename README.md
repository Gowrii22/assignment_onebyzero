
# OnebyZero Data Engineer Assignment

## Description
This is an in-memory REST API app to load, merge and expose transaction and product data using Flask.

##  Folder Structure
- `app.py`: Main application
- `transactions/`: Contains streaming transaction CSVs
- `reference/`: Contains product reference data
- `sample_data/`: Extra sample CSVs
- `requirements.txt`: Python dependencies
- `README.md`: Instructions

## How to Run

1. Install requirements:
   ```
   pip install -r requirements.txt
   ```

2. Run the app:
   ```
   python app.py
   ```

3. Visit the APIs:
   - Get Transaction:
     `http://localhost:8080/assignment/transaction/1`
   - Summary by Product:
     `http://localhost:8080/assignment/transactionSummaryByProducts/10000`
   - Summary by City:
     `http://localhost:8080/assignment/transactionSummaryByManufacturingCity/10000`

## Live Updates
The app watches `transactions/` folder and auto-loads new CSV files every 10 seconds.

## Author
Gowri Priya R
