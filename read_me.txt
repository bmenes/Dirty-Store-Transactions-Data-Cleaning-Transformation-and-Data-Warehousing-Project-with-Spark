## Question  

- Use this dataset: ` https://github.com/erkansirin78/datasets/raw/master/dirty_store_transactions.csv ` 
do the following tasks:
- If you have not learned yet how to write dataframe to storage/db please skip question 2 and 3.

### 1. 
Clean data
#### 1.1. Schema
```text
root
 |-- STORE_ID: string (nullable = true)
 |-- STORE_LOCATION: string (nullable = true)
 |-- PRODUCT_CATEGORY: string (nullable = true)
 |-- PRODUCT_ID: integer (nullable = true)
 |-- MRP: float (nullable = true)
 |-- CP: float (nullable = true)
 |-- DISCOUNT: float (nullable = true)
 |-- SP: float (nullable = true)
 |-- Date_Casted: date (nullable = true)
```
#### 1.2. String columns should not include special characters.

#### 1.3. Currencies should not include special characters.

Example output
```text
YR7220,New York,Electronics,12254943,31,20.77,1.86,29.14,2019-11-26
```

### 2. 
Write clean data to object storage (minio) format should be orc.

### 3. 
Write clean data to Postgresql as a table.