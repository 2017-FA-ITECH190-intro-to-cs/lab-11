# Introduction to Computer Science - Fall 2017

## Lab 11 - If ifs and ands were pots and pans

**Selective Execution:** This lab is an extension of Lab 10. It gives you a chance to practice using selective execution in JavaScript. That is, you will be adding statements to the functions you put in your weather library last week. Locate those files -- _weather.html_ and _weatherFunctions.js_. Copy those files into this repository before modifying them. Also, if you had any errors from last time, you should correct them before continuing.

As you may have noticed, there were times that the dew point and wind chill calculations didn't make a lot of sense. In this lab, you get to work toward fixing that.

The first step is to fix the calculateDewPoint() function in your _weatherfunctions.js_ file. The dew point calculated by that formula is only valid when the humidity is above 50%. Add an _if_ statement that verifies that the humidity is at least 50%. If it is not, the function should do two things. First, it should issue an alert that indicates that the humidity is too low to calculate the dew point. Then it should return the string literal "invalid".

Next you will fix the updateDewPoint() function in _weather.html_. After the call to calculateDewPoint(), add an _if_ statement that prevents the output div from being updated with the dewPoint is not a number. Said another way, add an _if_ statement that will do the update to the output div only when the dewPoint is a number. Not sure how to do this? Look at the NaN() function in the [diagonals demo](http://itech190.erickuha.com/conditionals/diagonals.html) or ask a classmate or the instructor.

The next step is to fix the calculateWindChill() function in your _weatherFunctions.js_ file. The wind chill calculated by that formula is only valid on temperatures less than 50 degrees Fahrenheit. Add an if statement that verifies that the temperature is at most 50 degrees. If it is not, the function should do two things. First, it should issue an alert that indicates that the temperature is too high to calculate the wind chill. Then it should return the string literal "invalid".

Another problem is that if the wind speed is 3 miles per hour or less, then the wind chill is the actual air temperature. Add an if statement that checks wether the wind speed is 3 miles per hour or less and, if it is, the function just returns the temperature.

Next, you will fix the updateWindChill() function in _weather.html_. After the call to calculateWindChill(), add an _if_ statement that prevents the output div from being updated when windChill is not a number. Said another way, add an _if_ statement that will only do the update to the output div when windChill is a number. This change will be very similar to the change you made to updateDewPoint().

Once you have completed the assignment, push your repository back to its master branch for grading.
