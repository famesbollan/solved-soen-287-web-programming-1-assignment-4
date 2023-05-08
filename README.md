Download Link: https://assignmentchef.com/product/solved-soen-287-web-programming-1-assignment-4
<br>
<h1>Exercise 1</h1>




The following set of short questions will focus on getting you familiar with how to write

PHP functions as well as how to make use of the pre-existing PHP functions.  All your PHP functions must be declared in the document body section and each functions name must be as specified below. To demonstrate the functionality of each method, you must make function calls in the document body. Include a heading (h1 … h6) that indicates the function is being tested before the function demonstration.  The use of Global Variables is forbidden!




<ol>

 <li>Function:<strong> findSummation </strong></li>

</ol>

<strong>Parameter(s): A positive integer number (default value is =1) </strong>

Given the input positive number (N), find the summation of all positive integer numbers from 1 to N (1+2+3+….+N) and return this summation. If the input parameter is not a number, or if it is not a positive number return false.




<ol>

 <li>Function:<strong> uppercaseFirstandLast </strong></li>

</ol>

<strong>Parameter(s): String </strong>

For each word in the input string, capitalize (uppercase) both the first letter and the last letter and return the modified string.

<ol>

 <li>Function<strong>: findAverage_and_Median </strong><strong><em>Parameter</em></strong><strong>: An array of numbers. </strong></li>

</ol>

Calculate the average and median of the numbers and return both values.







<ol>

 <li>Function:<strong> find4Digits</strong></li>

</ol>

<em>Parameter</em>: A string of numbers separated by spaces.

<em>Return t</em>he first four-digit number in the string; false if none.




<h1>Exercise 2</h1>




Create a php page (name it numOfVisits.php) that uses cookies to record and track the number of times a webpage has been visited. If the visitor is looking at the webpage for the first time, it should display the following message: <em>Welcome to my webpage! It is your first time that you are here. </em>If the page has been visited more than once, display: <em>Hello, this is the ## time that you are visiting my webpage </em>(where ## shows the number of visits). In this case you should also display a message that shows the day of the week, date, time and the time zone on your server that the page was visited last time in the following format (as an example):

<strong><em>Last time you visited my webpage on: Sun  Mar 20  17:16:18  EST  2017 </em></strong>(EST= Eastern Standard Time Zone)




<h1>Exercise 3</h1>

Write an HTML document to provide a form that collects names and telephone numbers. The phone numbers must be in the format ddd-ddddddd. Write a PHP script that checks the submitted telephone number to be sure that it conforms to the required format and then returns a response indicating whether the number was correct.




<h1>Exercise 4: Project</h1>

As you know, the last exercise of each assignment is continued from assignment to assignment and will have the goal of building a website by the end of this course. (Note: since this assignment introduces PHP into the project, it is likely that some of your web pages will have to have their extensions changed from .html to .php).




<strong>Nancy’s Apartment Search Website </strong>

Running Problem – Version 3

This version requires HTML, CSS, JS and PHP.

1) Create a template for your entire site such that you define the header and footer once and include them in each page of the site. This should be done using PHP. The following is just as a reminder of what the header and footer should contain.

2)

<ul>

 <li><strong>Header</strong>: It should include the name of your service and a logo/picture.</li>

</ul>

Clicking on the logo/picture should take you back to the home page. It

should also display the current date and time. The Time should automatically refresh every second.




<ul>

 <li><strong>Footer</strong>: This should appear at the bottom of all your pages. Give it a distinct background color and include links to a <strong>Privacy/Disclaimer Statement</strong> which can either appear in the content area of the site or in an alert or confirm box. It should display a message promising users that their information will not be sold or misused, and protects the website builder from any incorrect information.</li>

</ul>




<ul>

 <li>You will manage 2 text files which will reside on the server.

  <ul>

   <li>A <em>login file</em> which will contain username and passwords. This file will be consulted when a user is logging in. Each field should be separated by colon (:) and each user info is in one line.</li>

  </ul></li>

</ul>

For example if I have a file with 3 accounts, the file will look like so:

user1:pass1 user2:pass2 user3:pass3

<ul>

 <li>An <em>available apartment information file</em> that will store the information about address, type, amenities, pet info. Design your own format and field name for search.</li>

</ul>




<ul>

 <li><u>Functionality of your site</u>: Add the following functions to your site:

  <ul>

   <li><strong>Search</strong>: enter some search criteria and submit the query to a server site PHP program. This PHP program can search in the available apartment information file and find the matching apartments. Please notice that you can have none or multiple matchings.</li>

  </ul></li>

</ul>




<ul>

 <li><strong>Login/Create New Account: </strong>

  <ul>

   <li>Add a login button at the top-right corner of the search page.</li>

  </ul></li>

</ul>




<ul>

 <li>When a user clicks on this button, a login page loads into the content area with text fields for a username and one for a password as well as a login button. Below the login button, you can show a description of the allowed formats for usernames and passwords. A username can contain letters (both upper and lower case) and digits only. A password must be at least 4 characters long (characters are to be letters and digits only), have at least one letter and at least one digit. Before sending this information to the server make sure that the entered username and password satisfy the format criteria just listed.</li>

</ul>




<ul>

 <li>A user can input a username and a password on the login page. If the username and the password is a match verified by a PHP program against the log in file, redirect the user to the search page with “welcome, username” at the top-right corner (besides the login button).</li>

</ul>

If the username exists and the password is not a match verified by a

PHP program against the log in file, stay on the login page and show

“invalid login” before the login button and allow the user to re-enter inputs. If the username does not exist, write this new pair to the login file following the format specified in bullet 2 a) and return a new page to confirm that the account was successfully created and display a button to redirect the user to the search page.




 <strong>Connect the search page and the account login</strong>: if the user has logged in, show the full search results – types, street address, price. If the user does not login, the search results include only the area information, not the street address and a button “login to show the address” besides each result item. User can click the button to login. You do not need to cache the search results. After the login, the search starts again.


