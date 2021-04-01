# Technical Assignment
Assignment to test fundamental javascript knowledge for Prism Force. This can be written as a `nodejs` executable or a js file invoked through a browser.


### Problem statement
Write a `.js` file which will take a json object containing the revenue and expense data of a company, and output its balance sheet month wise. The revenue and expense may be fixed or variable amounts payable in installments.

The program should output the answer/ balance sheet to the console. The balance for any month is the sum of all revenue for the month - sum of all expense for the month (`revenue.amount - expense.amount`). Each entry has amount, timestamp and period. `period` represents recurring revenue in months including the entry date. If an entry in March has a period of 2, it means that amount will be for March and April. In some cases, the amount will increase month on month based on an `rate`. Assume the increments are compounded rates.

Sort the balancesheet in ascending order by timestamp.
Generate input JSON(s) of your own, attach them with the solution and verify the output.


#### Assumptions
- Amount will always be a valid positive number
- `startDate` will always be a valid ISO timestamp where the year and month may change. The day and time will remain constant
- Revenue and expense can be of different length. No guarentee which is longer
- Take `rate` as a decimal
- Variable `period` will always be a valid integer


#### Scenarios
- Date entries may be missing for revenue or expense, assume the amount is 0
- Think of additional cases, if any not covered here. Mention and solve for them


### Example
Two sample input files with their corresponding expected outputs have been provided for testing.


For `1-input.json`.

Expense for May is 20 with a period of 2 so it logs in expense of 20 for May and June. Similarly the entry for Jan results in revene for 3 periods - Jan, Feb and March. Jan, Feb and March are missing in expense so their amount is taken as 0.


### Bonus points
- Follow `es6` syntax strictly
- Read the json object from a file
- Optimize the solution for lowest time complexity
- Focus on writing modular reusable functions


### Sample data
2 set of files have been included where input is sample input data and output is the expected values.
