Question 1.how to integrate css file in html file? Options: a) using <javascript> tag
b) using <link> tag
Question 2. How do you make a new paragraph in HTML?
b) using <p> tag
Question 3. Div tag is a inline-block element? 
b) false (The <div> tag is a block-level element)
Question 4. Span is an inline-block element?
b) false (The <span> tag is an inline element)
Question 5. What is the output of following code?(1 mark)
function ValueOfC(){
Var y = 10;
Var c = y ** y console.log(c);
Return c; }
ValueOfC() // —-->
Answer:function ValueOfC(){
    var y = 10;
    var c = y ** y;
    console.log(c);
    return c;
}
ValueOfC();
Q6. Consider this array : const people = [
{ id: 1, name: 'John', age: 30 }, { id: 2, name: 'Jane', age: 25 }, { id: 3, name: 'Bob', age: 40 },
]; (apply all operations on this array)
only use map and filter functions to get the output array.
Answer:
A) Output array: ['John', 'Jane', 'Bob']
code:const names = people.map(person => person.name);
console.log(names);
// Output: ['John', 'Jane', 'Bob']
B) Output array: [{ "id":1,"name":"John","age":30,"salary":50000}, {"id": 2,"name": "Jane","age": 25,"salary": 50000}, {"id": 3,"name": "Bob","age": 40,"salary": 50000}]
code:const withSalaries = people.map(person => ({ ...person, salary: 50000 }));
console.log(withSalaries);
// Output: [{ "id":1,"name":"John","age":30,"salary":50000}, {"id": 2,"name": "Jane","age": 25,"salary": 50000}, {"id": 3,"name": "Bob","age": 40,"salary": 50000}]
C) Create an array of objects for people who are above 30 years old, and you only need their names and ages (no id property). Output array: [{"name": "Bob","age": 40}]
code:const above30 = people.filter(person => person.age > 30).map(person => ({ name: person.name, age: person.age }));
console.log(above30);
// Output: [{"name": "Bob","age": 40}]
Q7: write a function main and pass two functions as parameter to it cb1 and cb2. main(cb1, cb2, x, y) Define cb1 in such a way that will add two numbers Define cb2 in such a way that will give you the difference of two numbers.
X and y are two numbers ex- x=11, y =4.
code:function add(x, y) {
    return x + y;
}

function subtract(x, y) {
    return x - y;
}

function main(cb1, cb2, x, y) {
    console.log("Sum:", cb1(x, y));
    console.log("Difference:", cb2(x, y));
}

const x = 11;
const y = 4;
main(add, subtract, x, y);
Q8 : given an array
var users = [
{firstName : "Susan", lastName: "Steward"},
{firstName : "Daniel", lastName: "Longbottom"},
{firstName : "Jacob", lastName: "Black"}
];
outputarray = ["Susan Steward", "Daniel Longbottom", "Jacob Black"]
to get the output array from users array which array method will give you correct result?
c) map function
code:const outputArray = users.map(user => `${user.firstName} ${user.lastName}`);
console.log(outputArray);
// Output: ["Susan Steward", "Daniel Longbottom", "Jacob Black"]
Q10: what will be the value of arr? var arr = [1,2,3,4,5].filter(func)
function func(v){ return false;
code:var arr = [1, 2, 3, 4, 5].filter(func);
function func(v) {
    return false;
}
console.log(arr);
answer: [C]
Q11: what is the key difference between these two properties?Choose appropriate option.
 Display : none and visibility:hidden
 Answer:B) display: none removes the element from the DOM while visibility: hidden just hides the element.
Q12: what will be the output of following code? var a = 1;
var b = 0;
while (a <= 3)
{
a++;
b += a * 2;
console.log(b); }
Answer:code...var a = 1;
var b = 0;
while (a <= 3) {
    a++;
    b += a * 2;
    console.log(b);
}
Correct option isA) 4 10 18
explanation:When a = 1, the loop starts, a is incremented to 2, and b += 2 * 2 results in b = 4. This is logged.
When a = 2, a is incremented to 3, and b += 3 * 2 results in b = 10. This is logged.
When a = 3, a is incremented to 4, and b += 4 * 2 results in b = 18. This is logged.
The loop ends since a is now greater than 3.

Q13: at the end of both operations what will be the value of arr? (2 marks)
 Var arr= [1,2,3,4]
 arr.unshift(100)
 arr.shift()
 Answer:A) [1, 2, 3, 4]
 code:var arr = [1, 2, 3, 4];
arr.unshift(100);
arr.shift();

explanation:arr.unshift(100) adds 100 to the beginning of the array, resulting in [100, 1, 2, 3, 4].
arr.shift() removes the first element of the array (100), resulting in [1, 2, 3, 4].

