# Data Validation Report

## Project: SafeBank Fraud Shield

## Validation Framework
Custom validation using PySpark

## Rules Implemented

1. Account ID should not be NULL
2. Transaction amount must be > 0
3. Country should be valid
4. Timestamp should not be null

## Results

Total records processed: 5,000,000

Valid records: 4,998,500  
Invalid records: 1,500  

## Handling Strategy

Invalid records are filtered and logged separately for monitoring.

## Conclusion

Data quality checks ensure reliability of fraud detection pipeline.