# Developer Log
## Programming Assignment 2

### Entry 1 ###
**Date:** 2026-05-04
**Entry Type:** Edge Case 
**Task worked on:** Tested the base cases to ensure they branched when needed
**Decision:** I added a few debugging statements to better see how my code handles these edge cases
**What I tried:** I ran the function with a few r & c values, both in and out of range, to ensure the code is running properly
**Resolution:** The code is running as expected from the cases that I have tested 

---

### Entry 2
**Date:** 2026-05-04
**Entry Type:** Engineering Decision
**Task worked on:** printVisited function
**Decision:** Attempting to debug was getting difficult. I needed a way to see any possible errors
**Resolution:** I created a function to print the Visited function, allowing me to see if there was an issue

---

### Entry 3
**Date:** 2026-05-04
**Entry Type:** Bug Fix
**Task worked on:** dfs function
**Issue or decision:** The visited array was not being output as expected.  
**What I tried:** I printed the coordinates being visited to see if there was an issue with the recursive function calls
**Fix:** I forgot to change the enter values within the dfs function call in the main function after testing edge cases

---

### Entry 4
**Date:** 2026-05-04
**Entry Type:** Bug Fix
**Task worked on:** dfs function
**Issue:** The visited array would occasionally either not be printed or would be incorrect. When the array was correct, the printPath function would cause an error.
**What I tried:** I checked the code for every instance where these arrays were used to see if there was a possible mistake. 
**Fix:** The dfs function was passing the array by value rather than reference, causing issues when they were being manipulated. 

---

### Entry 5
**Date:** 2026-05-04
**Entry Type:** Engineering Decision
**Task worked on:** Creating the printPatent function
**Decision:** I needed to observe how the parent arrays were being manipulated throughout the dfs function calls 
**Resolution:** Created a function to print the array and included it after the arrays are manipulated in the dfs function. 

--- 

### Entry 6
**Date:** 2026-05-04
**Entry Type:** Edge Case
**Task worked on:** parent arrays within the dfs function
**Issue:** The function would occasionally raise an error when after the first recursive call of dfs and when printPath is called. 
**Error message:** Process finished with exit code -1073741571 (0xC00000FD)
**What I tried:** I added conditional branches before editing the parent array to ensure they did not access an out of bound memeory addess. 
**Fix:** I moved all conditional statements to be checked right before the parent arrays and the recursive call of the dfs function. 
