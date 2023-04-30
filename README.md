Download Link: https://assignmentchef.com/product/solved-cs2400-homework-6-auto-dealership
<br>
Use arrays, files, searching arrays, manipulating array contents, characters, and strings.

You are asked to implement a car ordering system for <strong><em>Bobcats Auto Dealership</em></strong>.  This dealership is brand new and only sells one brand of cars with three different models. However, a buyer can add options if they choose.

Write a C++ program that allows the user to order a single car with different options.  All the options available will be stored in a file called “<strong>options.txt</strong>” along with their cost. You may assume that the file will not contain more than 30 options. The user should be able to select the car model, display options and prices, add options, remove options, or cancel the order. Allow the user to see all the available options and their prices. <strong>The program should always display the car model, cost, and the options ordered so far</strong>.  If the user has not selected a car model, then an error message should be displayed indicating that the order has not started yet (e.g. NO MODEL SELECTED).  A user should not be able to add more than 6 options to the car.

The base prices of the three models: <strong>E </strong>($10,000.00), <strong>L</strong> ($12,000.00), and <strong>X </strong>($18,000.00).

<strong>Implement the following menu options in separate functions: </strong>

<ol>

 <li><strong>Select a model (E, L, X) </strong></li>

</ol>

The user should enter either E, L, or X (either in lower or upper case). If the wrong character is entered, the user should be prompted repeatedly until the user enters a valid model. Update the order information after this selection.

<ol start="2">

 <li><strong>Display available options and prices </strong>List all the options 3 per line. See below.</li>

</ol>




<ol start="3">

 <li><strong>Add an option </strong></li>

</ol>

The user should enter an option such as “DVD System”, “10 Speakers”, etc. The option entered must be one of the options available. If it’s not, the user should be prompted repeatedly until the user enters a valid option or enter “<strong>cancel</strong>“. After the selection, the order information should be updated. (see sample input/output below). Duplicate options should not be allowed.

<ol start="4">

 <li><strong>Remove an option </strong></li>

</ol>

Allow the user to remove one of the option from the list of options added earlier. Update the order information. If the option name is not in the list of options, then it should be ignored.

<ol start="5">

 <li><strong>Cancel order </strong></li>

</ol>

Start over. Update the order information.

<ol start="6">

 <li><strong>Quit</strong><strong>     </strong></li>

</ol>

<strong>Hints: </strong>

<ul>

 <li>Use an array/vector to store all the options along with an integer for the number of options read.</li>

 <li>Use an array/vector to store all the options’ prices.</li>

 <li>Use an array/vector of strings for the options added along with an integer for the number of options ordered.</li>

 <li>Write a function to convert a string to lowercase for comparison.</li>

 <li>Write a function that returns true if an option is valid</li>

</ul>

<strong>Sample input/output: </strong>

NO MODEL SELECTED

<ol>

 <li>Select a model (E, L, X)</li>

 <li>Display available options and prices</li>

 <li>Add an option</li>

 <li>Remove an option</li>

 <li>Cancel order</li>

 <li>Quit</li>

</ol>

Enter choice: <strong>3</strong>

NO MODEL SELECTED

<ol>

 <li>Select a model (E, L, X)</li>

 <li>Display available options and prices</li>

 <li>Add an option</li>

 <li>Remove an option</li>

 <li>Cancel order</li>

 <li>Quit</li>

</ol>

Enter choice: <strong>2</strong>




Prices for model E, L, &amp; X: $10000.00, $12000.00, $18000.00

Available Options




<table width="0">

 <tbody>

  <tr>

   <td width="240">Leather Seats ($5000)</td>

   <td width="408">DVD System ($1000)      10 Speakers ($800)</td>

  </tr>

  <tr>

   <td width="240">Navigation System($1400)</td>

   <td width="408">CarPlay ($500)          Android Auto ($500)</td>

  </tr>

  <tr>

   <td width="240">Lane Monitoring ($2000)</td>

   <td width="408">3/36 Warranty ($800) 6/72 Warranty ($999)</td>

  </tr>

  <tr>

   <td width="240">Dual Climate ($1500)</td>

   <td width="408">Body Side Molding($225) Cargo Net ($49)</td>

  </tr>

  <tr>

   <td width="240">Cargo Organizer ($87)</td>

   <td width="408">450W Audio ($700)       Heated Seats($1000)</td>

  </tr>

 </tbody>

</table>




NO MODEL SELECTED




<ol>

 <li>Select a model (E, L, X)</li>

 <li>Display available options and prices</li>

 <li>Add an option</li>

 <li>Remove an option</li>

 <li>Cancel order</li>

 <li>Quit</li>

</ol>

Enter choice: <strong>1</strong>

Enter the model (E, L, X): <strong>l</strong>




Model: L, $12000.00, Options: None







<ol>

 <li>Select a model (E, L, X)</li>

 <li>Display available options and prices</li>

 <li>Add an option</li>

 <li>Remove an option</li>

 <li>Cancel order</li>

 <li>Quit</li>

</ol>

Enter choice: <strong>3</strong>

Enter option: <strong>450w aUdIO</strong>




Model: L, $12700.00, Options: 450W Audio




<ol>

 <li>Select a model (E, L, X)</li>

 <li>Display available options and prices</li>

 <li>Add an option</li>

 <li>Remove an option</li>

 <li>Cancel order</li>

 <li>Quit</li>

</ol>

Enter choice: <strong>3</strong>

Enter option: <strong>carplay</strong>




Model: L, $13200.00, Options: 450W Audio, CarPlay







<ol>

 <li>Select a model (E, L, X)</li>

 <li>Display available options and prices</li>

 <li>Add an option</li>

 <li>Remove an option</li>

 <li>Cancel order</li>

 <li>Quit</li>

</ol>

Enter choice: <strong>4</strong>

Enter option to remove: <strong>carplay</strong>




Model: L, $12700.00, Options: 450W Audio