Test 1
-----

###We need a Type called 'Car' wich will have the following specs:###
1. has model, color, year properties
2. has speed, maxSpeed properties
3. has drive, stop functions
4. has accelerate function that accepts number and increase the speed of the car by this number
5. if the car is stopped the accelerate function will not work and log error message.
6. if the car speed is more than the maxSpeed, it will log out an error message.
7. car speed will never go more than the maxSpeed
8. has function 'toString' that will log the model number, color, and year, ex "BMW 2013 Black".

###Test Output###

```javascript
var c = new Car();

c.model = 'Mercides';
c.color = 'Red';
c.year = 2012;
c.maxSpeed = 240;

c.accelerate(10); // should log error message
console.log(c.speed) // should log 0

c.drive();
c.accelerate(50);
console.log(c.speed) // should log 50

c.accelerate(250); // should log error message
console.log(c.speed) // should log 240

c.stop();
c.accelerate(10); // should log error message

c.toString(); // should log 'Mercides 2012 Red'

 ```
