# Technical Assignment
Assignment to test json manipulation skills for Prism Force.

### Explanation
Write a `.js` file which will take a json object containing the revenue and expense data of a company, and output its balance sheet month wise. 

Write a javascript program which will calculate the balance sheet for an organization and output the answer to the console. The balance for any month is the sum of all revenue for the month - sum of all expense for the month (`revenue.amount - expense.amount`)

Two sample input files with their corresponding expected outputs have been provided for testing.

Look at `1-input.json` for the month of March. The `expense` is 30 while the revenue has 2 entries - amount of 60 and 10. The total balance for March is `60 + 10 - 30` which is `40` - visible in `1-output.json`.
Revenue and expenses may have multiple entries per month, may have missing data for which you can assume the `amount` is `0`. Their timestamps may not overlap. Eg. Revenue may be for Feb and March, while expenses has data for Jan, March and April - refer to `2-input.json` for further examples


You may assume
- Amount will always be a valid positive number
- startDate will always be a valid ISO timestamp where the year and month may change. The day and time will remain constant


### Bonus points
- Follow `es6` syntax strictly
- Read the json object from a file
- Sort the balancesheet in ascending order by timestamp
- Think of any fringe cases and solve for them - think from a product perspective as well
- Optimize the solution for lowest time complexity
- Focus on writing modular reusable functions


### Sample data
2 set of files have been included where input is sample input data and output is the expected values.
