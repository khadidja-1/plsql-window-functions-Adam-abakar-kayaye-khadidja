# PL/SQL Window Functions

This project demonstrates the use of window functions in PL/SQL for advanced data analysis and reporting.

## Features

- Examples of common window functions: `ROW_NUMBER()`, `RANK()`, `DENSE_RANK()`, `LEAD()`, `LAG()`, etc.
- Sample schemas and queries for learning and experimentation.
- Well-documented code for easy understanding.

## Getting Started

1. Clone the repository.
2. Set up your Oracle database environment.
3. Run the provided SQL scripts to create sample tables and data.
4. Explore the window function examples in the `/examples` directory.

## Requirements

- Oracle Database (tested on 12c and above)
- SQL*Plus or any compatible PL/SQL client

## Usage

```sql
-- Example: Using ROW_NUMBER() window function
SELECT
    employee_id,
    department_id,
    salary,
    ROW_NUMBER() OVER (PARTITION BY department_id ORDER BY salary DESC) AS rank
FROM
    employees;
```

## Contributing

Contributions are welcome! Please open issues or submit pull requests for improvements.

## License

This project is licensed under the MIT License.

## Authors

- Khadidja Adam Abakar Kayaye
