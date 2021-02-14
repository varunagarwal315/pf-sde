# Technical Assignment
Assignment to test json manipulation skills for Prism Force.

### Requirements
Write a javascript program which will import a json file and calculate the balance sheet for an organization, sorted by month in ascending order. Follow `es6` syntax wherever applicable.
Revenue and expenses may have multiple entries per month, may have missing data for which you can assume the `amount` is `0`. Their timestamps may not overlap. Eg. Revenue may be for Feb and March, while expenses has data for Jan, March and April.

- Create a new json array where `amount` is `revenue.amount - expense.amount`
- Split the code into multiple functions to ensure reusability
- Write unit test using any test framework such as `jest` or `chai` for each of the functions written

### Sample data
2 set of files have been included where input is sample input data and output is the expected values.
