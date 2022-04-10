JavaScript Example for ARRAY

```JavaScript
var countries = ["USA",]
undefined
var countries = ["USA","Germany","China"]
undefined
countries[0]
'USA'
var mixed = [true,20,"mixed"]
undefined
mixed
(3) [true, 20, 'mixed']
// String is immutable
undefined
animal = "dog"
'dog'
animal[1]
'o'
// Try to change it
undefined
animal[1] = "i"
'i'
// Check if changed
undefined
animal[1]
'o'
animal
'dog'
// Array is mutable
undefined
countries[0] = 'India'
'India'
countries
(3) ['India', 'Germany', 'China']
```
Here also the pop() and push() works and also the length() method calls.

```JavaScript
for (var i=0;i<countries.length;i++) {
    console.log(countries[i])
}
VM1138:2 India
VM1138:2 Germany
VM1138:2 China
undefined
// The other way
undefined
for (country of countries){
    console.log(country)
}
VM1372:2 India
VM1372:2 Germany
VM1372:2 China
undefined
// Alerting the user with the content
undefined
for (country of countries){
    alert(country)
}
undefined
// Another way to do it
undefined
countries.forEach(alert)
undefined
```
