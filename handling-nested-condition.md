# Replace Nested Conditional with Guard Clauses

### Imagine we have something like that

function getPayAmount() { <br>
  let result;<br>
  if (isDead)<br>
    result = deadAmount();<br>
  else {<br>
    if (isSeparated)<br>
      result = separatedAmount();<br>
    else {<br>
      if (isRetired)<br>
        result = retiredAmount();<br>
      else<br>
        result = normalPayAmount();<br>
    }<br>
  }<br>
  return result;<br>
}<br>

### It's unreadable and looks really bad.

### At the same time, this function is fix this behaviour

function getPayAmount() {<br>
  if (isDead) return deadAmount();<br>
  if (isSeparated) return separatedAmount();<br>
  if (isRetired) return retiredAmount();<br>
  return normalPayAmount();<br>
}<br>

### Code became more readable and clear

### Example

https://refactoring.com/catalog/replaceNestedConditionalWithGuardClauses.html
