# Encapsulate Variable

## Imagine a variable

let age = 20;

## Anyone in code may change that

age = 30; <br>
age = -100; <br>
age = 999999; <br>

## Encapsulate is about - Don't modify `age` directly. If you want to change it, call my function.

let age = 20; <br>

function getAge() { <br>
  return age;<br>
}<br>

function setAge(newAge) {<br>
  age = newAge;<br>
}<br>

## The goal is to create a single point of control over data access.

## Example

<img width="671" height="572" alt="image" src="https://github.com/user-attachments/assets/81714682-fe7e-48ff-8704-ab299fab5dd9" />
