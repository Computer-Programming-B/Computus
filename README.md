Computus
========
This assignment is similar to the previous temperature conversion assignment. You are to write a program that traverses a list of years and displays the date of Easter for each of those years. Easter Sunday is the first Sunday after the first full moon of Spring. The calculation of the date of Easter is called Computus in Latin.  One algorithm for Computus was invented by mathematician Carl Friedrich Gauss in the early 1800s and is shown below. All divisions are integer divisions. 
1. Let y be the year.
2. Divide y by 19 and call the remainder a. Ignore the quotient. 
3. Divide y by 100 to get a quotient b and a remainder c. 
4. Divide b by 4 to get a quotient d and a remainder e. 
5. Divide 8 * b + 13 by 25 to get a quotient g. Ignore the remainder. 
6. Divide 19 * a + b - d - g + 15 by 30 to get a remainder h. Ignore the quotient.
7. Divide c by 4 to get a quotient j and a remainder k. 
8. Divide a + 11 * h by 319 to get a quotient m. Ignore the remainder. 
9. Divide 2 * e + 2 * j - k - h + m + 32 by 7 to get a remainder r. Ignore the quotient.
10. Divide h - m + r + 90 by 25 to get a quotient n. Ignore the remainder. 
11. Divide h - m + r + n + 19 by 32 to get a remainder p. Ignore the quotient.
12. The month that Easter falls on is n and the date is p. For example, if n is 4 and p is 15, Easter falls on 4/15 or April 15th of that year.

Suggested Steps to complete this assignment
1. Start a new program in Processing. 
2. Create a list of years with code like years = [2010,2011,2012,2013,2014,2015,2016,2017,2018,2019,2020]
3. Now create a for each loop that traverses the list and one by one stores each year in a variable y.
4. Now add code inside the for each loop to implement Gauss' Computus algorithm. You should use 13 variables: a, b, c, d, e, g, h, j, k, m, r, n, p
5. Check your calculations. For 2010 a, b, c, d, e, g, h, j, k, m, r, n, p should be 15, 20, 10, 5, 0, 6, 9, 2, 2, 0, 4, 4, 4
6. Add print() statements inside the for each loop to display n, p and y in month, day and year form. Your output should look similar to this:   
![screenshot of output](computus.png)
7. Submit the .pyde file via the school loop drop box.
