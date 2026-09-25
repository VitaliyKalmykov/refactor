# Extract Function

## If there is a separate block of code within a function that performs a clear, self-contained task, you can extract it into a separate function and give that task a name.

## As we can see below, logic is mixed. 

function printOwing(invoice) { <br>
  printBanner();<br>

  let outstanding = calculateOutstanding();<br>

  // print details<br>
  console.log(`name: ${invoice.customer}`);<br>
  console.log(`amount: ${outstanding}`);<br>
}<br>

## How to refactor this correctly

function printOwing(invoice) { <br>
  printBanner();<br>

  let outstanding = calculateOutstanding();<br>

  printDetails(outstanding);<br>
}<br>

function printDetails(outstanding) {<br>
  console.log(`name: ${invoice.customer}`);<br>
  console.log(`amount: ${outstanding}`);<br>
}<br>

## Example

<img width="760" height="892" alt="image" src="https://github.com/user-attachments/assets/3088ec0e-20be-4ebc-8fd3-83baf65e92a6" />

