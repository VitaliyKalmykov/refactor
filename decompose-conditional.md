# Decompose Conditional

## Break down a complex if statement into functions with descriptive names

### Imagine we have this code

if (!aDate.isBefore(plan.summerStart) && !aDate.isAfter(plan.summerEnd)) <br>
  charge = quantity * plan.summerRate; <br>
else <br>
  charge = quantity * plan.regularRate + plan.regularServiceCharge; <br>

### The code is unreadable; we won't be able to figure out what's going on here in a second.

### While, this code is much more clear

if (summer())<br>
  charge = summerCharge();<br>
else<br>
  charge = regularCharge();<br>
  
## Example 

<img width="726" height="711" alt="image" src="https://github.com/user-attachments/assets/d3f50710-fe98-43f6-8cdf-61aaec99cb4a" />

