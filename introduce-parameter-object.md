# Introduce Parameter Object
## Imagine if we have a fucntion
function getOrders(<br>
  startDate: Date,<br>
  endDate: Date<br>
) {}<br>
### It has two parameters, but these parameters describe a single thing: the time interval from X to Y.
### Instead of passing two variables, we can create a single object and pass it as an argument.
## Why ?
### Let's imagine we have many functions

getOrders(startDate, endDate);<br>
getRevenue(startDate, endDate);<br>
getUsers(startDate, endDate);<br>
getInvoices(startDate, endDate);<br>

### Instead of passing each argument separately, we simply pass an object 
#### Now the code makes sense:
#### “Get orders for this period.”
#### Rather than:
#### “Get orders by passing a specific start date and a specific end date separately.”
#### And this is Fowler’s key idea. The object here isn’t there just for the sake of having an object. It’s there because several values actually represent a single concept.

getOrders(dateRange);<br>
getRevenue(dateRange);<br>
getUsers(dateRange);<br>
getInvoices(dateRange);<br>

## example

<img width="650" height="490" alt="image" src="https://github.com/user-attachments/assets/8bcba711-95f3-45cd-a617-49f7b1442e44" />
