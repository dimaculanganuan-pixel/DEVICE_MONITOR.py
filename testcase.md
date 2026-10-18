# Test Cases: Simulated Device Monitoring and Alert System

Name: Villanueva, Uan Timothy D.  
Student Number: 2500746  
Section: 1CPE-B  
Date Tested: October 18, 2026  

## Test Cases

I made these test cases to check if my program works correctly. I tested valid and invalid inputs to see if the program displays the correct results and handles mistakes properly.

| Test Case | Input or Action | Expected Result | Why I Expected This Output | Actual Result | Pass/Fail |
|---|---|---|---|---|---|
| TC01 | Select option 1 to view readings. | The program displays 28, 31, 35, 37, and 29. | These are the initial readings given in the project instructions. | The program displayed all five readings. | Pass |
| TC02 | Select option 2 and enter 33, then select option 1. | The program accepts 33 and adds it to the readings. | The value is a whole number between 0 and 100. | The program accepted 33 and added it as the sixth reading. | Pass |
| TC03 | Select option 2 and enter abc. | The program rejects the input and displays an error message. | Letters cannot be used because the program requires a whole number. | The program rejected the input and displayed an error message. | Pass |
| TC04 | Select option 2 and enter -5. | The program rejects the input. | The allowed reading range is from 0 to 100. | The program rejected the negative value. | Pass |
| TC05 | Select option 2 and enter 120. | The program rejects the input. | The value is greater than the maximum allowed reading of 100. | The program rejected the value. | Pass |
| TC06 | Add the reading 30, then select option 3. | The reading 30 is classified as WARNING. | Readings from 30 to 35 belong to the WARNING category. | The program classified 30 as WARNING. | Pass |
| TC07 | Restart the program and classify the initial readings. | 28 and 29 are NORMAL, 31 and 35 are WARNING, and 37 is CRITICAL. | NORMAL is below 30, WARNING is from 30 to 35, and CRITICAL is above 35. | The program classified all readings correctly. | Pass |
| TC08 | Restart the program and select option 4. | Count: 5, Total: 160, Average: 32.00, Minimum: 28, Maximum: 37, NORMAL: 2, WARNING: 2, CRITICAL: 1, Overall Status: ATTENTION REQUIRED. | The total is 160 and the average is 32.00. The minimum is 28 and the maximum is 37. Since one reading is CRITICAL, the overall status is ATTENTION REQUIRED. | The program displayed the correct summary and overall status. | Pass |
| TC09 | Enter 9 at the menu. | The program displays an invalid choice message and shows the menu again. | The menu only has options 1 to 5. | The program rejected the choice and displayed the menu again. | Pass |
| TC10 | Select option 5. | The program displays an exit message and stops running. | Option 5 is the Exit option. | The program displayed an exit message and ended. | Pass |

## Bugs Found and Fixed

During testing, I did not find any bugs in the ten test cases. The program displayed the expected results for valid readings, rejected invalid readings, classified temperatures correctly, generated the correct summary, and exited when I selected option 5.

## Testing Notes

1. I ran each test case and compared the actual result with the expected result.
2. I restarted the program before TC07 and TC08 to use only the five initial readings.
3. I marked each test as Pass because the results matched the expected results.
4. I tested TC02 and TC06 separately so that the added readings would not affect TC07 and TC08.
