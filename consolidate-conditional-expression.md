# Consolidate Conditional Expression

## The point is to combine several conditions that mean the same thing from a business perspective.

### imagine we have this code

if (employee.seniority < 2) return 0; <br>

if (employee.monthsDisabled > 12) return 0; <br>

if (employee.isPartTime) return 0; <br>

### At first glance, these are three different `if` statements. But they all produce the same result:

return 0;

### So we can just group it 

function isNotEligibleForDisability() { <br>
  return ( <br>
    employee.seniority < 2 || <br>
    employee.monthsDisabled > 12 || <br>
    employee.isPartTime <br>
  ); <br>
} <br>

## Example

<img width="654" height="801" alt="image" src="https://github.com/user-attachments/assets/51649e46-4b65-4c24-aade-329f330ff86c" />


