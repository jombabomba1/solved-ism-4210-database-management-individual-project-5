Download Link: https://assignmentchef.com/product/solved-ism-4210-database-management-individual-project-5
<br>
<h2>INSTRUCTIONS</h2>

Please read the description and the requirements of Deliverable #5 carefully before responding. If you have any questions or clarifications, feel free to contact me via email (<u><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="fa9b9e938e93978f91929f88909f9fba">[email protected]</a> ufl.edu</u>), during my office hours, or by appointment <strong> </strong>

All submissions should be <u>individual work</u> only. Do not discuss your answers with your class mates or group members. Plagiarism will not be tolerated.

<strong><u>Due Date:</u></strong>  Before class Apr 14, 2016 on Canvas.

No late submissions will be accepted. If you have trouble submitting assignments to the e-learning system, please contact me <u>before</u> the submission deadline.

<strong><u>Page Limit:</u></strong>  There is no fixed page limit for this deliverable.

<strong><u>Format: </u></strong>  You will submit 7 SQL statements and the results of running the queries in the attached database. Copy and paste all the statements and the diagram into a Word document that you can save and submit as a PDF. Please note the number of the problem statement clearly above each query. See page 3 of this document for an example of how to present the statements.  The name of your file should be <strong>&lt;LastName&gt;_&lt;FirstName&gt;_IP5.pdf. </strong>Submissions that do not follow the formatting guidelines will not be graded.




<h2>DELIVERABLE #5 – MULTIPLE TABLE QUERIES</h2>

For this deliverable, you will be writing queries to use the data in the TheHipp database.




<strong>STEP 1:</strong> Download the SQL script (TheHipp.sql) file attached to assigment IP#4. Run the scripts into MySQL as follows:

<ul>

 <li>Open the SQL script file using CTRL+SHIFT+O.</li>

 <li>Run the entire script using CTRL+SHIFT+Enter.</li>

</ul>




<strong>STEP 2:</strong>  For each of the problem statements listed in below, please do the following:

<ol>

 <li>Write the SQL query that will achieve the desired result</li>

 <li>Run the query in the MySQL database.</li>

 <li>Copy and paste the results of the query below each SQL statement using the format on page 3 of this assignment. If you results have more than 10 rows only copy the <strong><u>first 10 rows</u></strong>.</li>

</ol>




Each query must satisfy the following criteria:

<ol>

 <li>They must not include any extra/unnecessary tables.</li>

 <li>The results must not include any extraneous columns.</li>

 <li>All column headings should be meaningful names. Please do not have columns with headings that contain expressions or aggregate functions.</li>

 <li>They must not use views unless specified in the instructions.</li>

</ol>

<strong> </strong>

<strong> </strong>

Department of Information Systems &amp;

Warrington College of Business Administration, University of Florida

<h1>Individual Project #5</h1>

<strong> </strong>

<h2>PROBLEM STATEMENTS</h2>




<ol>

 <li>List the names of the customers in the database who have not bought a single ticket. You must submit two queries: (A) Write this query using a sub-query</li>

</ol>

(B) Write this query using a join

The output section of MySQL Workbench shows you the Duration for each query. Which query took longer to execute?




<ol start="2">

 <li>List the venue name, capacity, total revenue and the number of tickets sold for each venue. Write an efficient query that uses the minimum number of tables required.</li>

</ol>




<ol start="3">

 <li>List the name, revenue (total price paid for all the tickets), the promotion cost, the screen cost and the total profit (revenue – promotion cost – screening cost) for the 5 most profitable movies.</li>

</ol>




<ol start="4">

 <li>List the name, description and Venue ID for each event. In addition, if the event is a movie, list the genre. If the event is a play – list the name of the author. Your table should only have 4 columns. The fourth column should be called ‘Genre/Author’. The results will have the same number of rows as the EventTable.</li>

</ol>




<ol start="5">

 <li>Create a View called TicketDetails that includes all the columns from the Ticket and the Event table for each ticket.</li>

</ol>




<ul>

 <li>Use the TicketDetails view in a query that returns the following information for each event: EventCode, event name, the number of shows, the screen cost, the total screening cost (number of shows * screening cost), promotion cost, production cost, total cost (total screen cost + promotion cost + production cost), the expected revenue (use the BaseTicketPrice), the actual revenue, the total discounts given (expected revenue – actual revenue) and the profit (all costs – actual revenue)</li>

</ul>




<ul>

 <li>Use the Customer table and the TicketDetails to list the HippCode, name and email of each customer, along with number of tickets they have bought for theater (plays) and the number of tickets they have bought for movies. Sort your results in the descending order of the total number of tickets. Your results may look like the following but should have 199 rows.</li>

</ul>

<table width="580">

 <tbody>

  <tr>

   <td width="74"><strong>HippCode </strong></td>

   <td width="75"><strong>LastName </strong></td>

   <td width="77"><strong>FirstName </strong></td>

   <td width="154"><strong>Email </strong></td>

   <td width="104"><strong>TheaterTickets </strong></td>

   <td width="95"><strong>MovieTickets </strong></td>

  </tr>

  <tr>

   <td width="74">29249</td>

   <td width="75">Yang</td>

   <td width="77">Shengda</td>

   <td width="154"><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="86f5eee3ffc6ffe7eee9e9a8e5e9eb">[email protected]</a></td>

   <td width="104">41</td>

   <td width="95">4</td>

  </tr>

  <tr>

   <td width="74">91179</td>

   <td width="75">Burnell</td>

   <td width="77">Dana</td>

   <td width="154"><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="f99d98979b8c8b979c9595b99e94989095d79a9694">[email protected]</a></td>

   <td width="104">37</td>

   <td width="95">4</td>

  </tr>

  <tr>

   <td width="74">19670</td>

   <td width="75">Hill</td>

   <td width="77">Annie</td>

   <td width="154"><a href="/cdn-cgi/l/email-protection" class="__cf_email__" data-cfemail="accdc2c2c5c9c4c5c0ecc3d9d8c0c3c3c782cfc3c1">[email protected]</a></td>

   <td width="104">36</td>

   <td width="95">4</td>

  </tr>

 </tbody>

</table>

Department of Information Systems &amp;

Warrington College of Business Administration, University of Florida

<h1>Individual Project #5 Template</h1>

For each query, you must present your results using the following template.




<table width="667">

 <tbody>

  <tr>

   <td width="667"><strong>SELECT statement</strong></td>

  </tr>

  <tr>

   <td width="667">SELECT * FROM Customer; </td>

  </tr>

 </tbody>

</table>


