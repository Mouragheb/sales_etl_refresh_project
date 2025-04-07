# Sales ETL Refresh Project

This project is a complete Extract-Transform-Load (ETL) pipeline that reads raw sales data from a CSV file, transforms it, and loads it into a PostgreSQL database. It is designed for deployment both locally and on an AWS EC2 instance.

---

## Project Structure
sales_etl_refresh_project/
├── data_lake/
│   └── raw/
│       └── sales_data.csv
├── .env
├── requirements.txt
├── sales_etl.py
└── README.md

---

## Features

- Extracts sales data from a CSV file
- Cleans and transforms product and region fields
- Loads the data into a PostgreSQL table named `sales`
- Compatible with both local and cloud (EC2) environments

---

## Technologies Used

- Python 3
- Pandas
- psycopg2-binary
- python-dotenv
- PostgreSQL
- Git & GitHub
- AWS EC2

---

## How to Run (Locally or on EC2)

1. **Clone the repository**
   ```bash
   git clone git@github.com:Mouragheb/sales_etl_refresh_project.git
   cd sales_etl_refresh_project
2.	Create a virtual environment
   python3 -m venv venv
   source venv/bin/activate
3.	Install dependencies
   pip install -r requirements.txt
4.	Set up .env file
   DB_NAME=salesdb
   DB_USER=mousragheb
   DB_PASSWORD=12345678
   DB_HOST=localhost
   DB_PORT=5432 
5.	Run the pipeline
   python3 sales_etl.py
6. Example Output  
   Extracting from: data_lake/raw/sales_data.csv
   Inserted 3 rows into 'sales' table.   


## Project Screenshots

1. ETL Script & Terminal Output

Shows the main sales_etl.py pipeline and successful ETL run.

2. Table Schema in PostgreSQL

Describes the structure of the sales table.

3. Data in Sales Table (SELECT)

Displays a sample query result from the sales table.

4. Row Count in Sales Table

Verifies data insertion using row count.

5. Sales by Region (Grouped Query)

Shows a query grouping total sales by region.

## Author
Moustafa Ragheb
GitHub: @Mouragheb     

## License
This project is licensed under the MIT License.

---

### Next Step:
Replace your current content with this, save the file, and let me know. Then we’ll commit and push it to GitHub!
