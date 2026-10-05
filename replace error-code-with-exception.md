## Replace Error Code with Exception
### Example

<img width="721" height="597" alt="image" src="https://github.com/user-attachments/assets/8aa81ab1-13c3-4d78-8c41-54f5c9a7f17e" />

### Purpose of this method is separate normal return values from errors. Instead of returning special error codes like -23, the method throws an exception, which  makes errors clearer and allows them to be handled separately using try/catch.
