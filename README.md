Download Link: https://assignmentchef.com/product/solved-kit101-assignment1
<br>
You have a meal to eat. But should you consume it? Obviously if it’s solely chocolate or alcohol then the answer is probably ‘yes’. Obviously if it’s some kind of green vegetable or green meat (or in fact anything green) then the answer is most definitely ‘no’!

If you can eat it, should you? Well, not if it’s too hot or too cold — and not if there’s too much of it!  Everything in moderation after all (except green food).

You are to write a Java application program named AssigOne216.java which provides the user with advice as to whether their meal is edible or inedible and why. If it’s edible then the amount of food left over (if any) should be shown. The details (specifications) of this task are given below. Note that the correctness marks you receive for your program will depend on how well it matches this specification. If you decide to implement something that is more elaborate than specified, you should understand that:

<ul>

 <li>There will be no marks awarded for the elaborations you have designed and penalties may be applied for confusing/extraneous code.</li>

 <li>Your program MUST STILL meet the basic specifications given below.</li>

</ul>

The program is to determine whether the meal is edible or inedible and why. The user will be asked three initial questions:

<ul>

 <li>The description of the meal to be consumed (which may be a multi-word answer which contains spaces).</li>

 <li>The volume of the meal in millilitres (a whole number).</li>

 <li>Whether or not the meal is at the ambient room temperature (of 22.0 degrees Celsius). If the meal is not at room-temperature then the user should be asked for the temperature (as a floating point number).</li>

</ul>




The user may opt not to provide any information about meals at all.




NOTE: Part of the assessment of your program may be done automatically, so it is important that you follow the specification exactly, for example the questions must be asked in the order given and the method the user is given to indicate that they want to enquire about.

<h2>Algorithm</h2>

<ul>

 <li>Firstly, the program should ask the user whether they would like to consume the food they have.</li>

 <li>If the user does wish to consume their food then o The user will be asked to enter a description of the meal they have.</li>

</ul>

(Their entry may contain spaces and upper- and lower-case letters.) o The user will be asked to enter the volume of their food in millilitres (as a whole number).

<ul>

 <li>The user will be asked to enter whether or not their meal is at roomtemperature (using a true or false value).</li>

 <li>If the user indicates that their meal is not at room temperature then

  <ul>

   <li>They will be asked to enter the current temperature of their meal (a floating-point number value which may be positive, negative, or zero).</li>

  </ul></li>

 <li>The program will then work out whether the meal is edible or not and what, if any food remains after the first 1500 ml is consumed… Starting with the assumption that the meal is edible, if there is insufficient food to eat (i.e. 0 ml or less) then

  <ul>

   <li>the meal is inedible because there is not enough of it o Otherwise</li>

   <li>If the meal is too hot (65 degrees or hotter) or too cold (–5 degrees or colder) then</li>

  </ul></li>

 <li>The meal is inedible because of its temperature</li>

 <li>Otherwise</li>

 <li>If the meal is either “chocolate” or “alcohol” then o The meal is edible because it’s a favourite food</li>

 <li>Otherwise</li>

</ul>

o If the description of the meal starts with “green” then

<ul>

 <li>The meal is inedible because it is green o Otherwise</li>

 <li>The meal is edible but for no special reason</li>

</ul>

o If the meal is edible

<ul>

 <li>The amount of food which remains after the maximum of 1500 ml is consumed is calculated.</li>

 <li>The description of the meal, its volume, and its temperature should then be displayed to the user</li>

 <li>The state (edible) of the meal should then be given together with the reason (see sample output).</li>

 <li>The volume remaining should also be displayed (again, see sample output). o Otherwise</li>

 <li>The description of the meal, its volume, and its temperature should then be displayed to the user</li>

 <li>The state (inedible) of the meal should then be given together with the reason (see sample output).</li>

 <li>After the meal’s contents has been considered the user will be asked if they wish to consider another meal. To analyse another the user must enter a line beginning with ‘y’ or ‘Y’ (for yes). The program should repeat until they enter a response commencing with a letter other than ‘y’ or ‘Y’.</li>

 <li>The user will be shown a message saying how many meals were analysed.</li>

</ul>




Three example executions are shown below:




Would you like to eat the food you have? <strong><em>n</em></strong>




0 meals were attempted.










Would you like to eat the food you have? <strong><em>y</em></strong>




Please describe the food you have: green beans

What is the volume of the food you have (in millilitres)? <strong><em>200</em></strong>

True/False — Is the food at room temperature? <strong><em>false</em></strong>

What temperature is the food (in Celsius)? <strong><em>50</em></strong>




Your 200 ml meal of green beans, currently at 50.0 degrees Celsius is inedible because food contains something green — yecccchhh!




Would you like to eat more of the food you have? <strong><em>Yes</em></strong>




Please describe the food you have: <strong><em>chocolate</em></strong>

What is the volume of the food you have (in millilitres)? <strong><em>30</em></strong>

True/False — Is the food at room temperature? <strong><em>true</em></strong>




Your 30 ml meal of chocolate, currently at 22.0 degrees Celsius is edible because food is either chocolate or alcohol!

There will be 0 millilitres of food remaining after you’ve eaten




Would you like to eat more of the food you have? <strong><em>yep</em></strong>




Please describe the food you have: <strong><em>alcohol</em></strong>

What is the volume of the food you have (in millilitres)? <strong><em>2000</em></strong>

True/False — Is the food at room temperature? <strong><em>false</em></strong>

What temperature is the food (in Celsius)? <strong><em>0</em></strong>




Your 2000 ml meal of alcohol, currently at 0.0 degrees Celsius is edible because food is either chocolate or alcohol!

There will be 500 millilitres of food remaining after you’ve eaten




Would you like to eat more of the food you have? <strong><em>no</em></strong>




3 meals were attempted.













Would you like to eat the food you have? <strong><em>YES</em></strong>




Please describe the food you have: beef steak

What is the volume of the food you have (in millilitres)? <strong><em>350</em></strong>

True/False — Is the food at room temperature? <strong><em>false</em></strong>

What temperature is the food (in Celsius)? <strong><em>-10.5</em></strong>




Your 350 ml meal of beef steak, currently at -10.5 degrees Celsius is inedible because food must be between -5.0 and 65.0 degrees to be consumed!




Would you like to eat more of the food you have? <strong><em>y</em></strong>




Please describe the food you have: <strong><em>water</em></strong>

What is the volume of the food you have (in millilitres)? <strong><em>100</em></strong>

True/False — Is the food at room temperature? <strong><em>false</em></strong>

What temperature is the food (in Celsius)? <strong><em>100</em></strong>




Your 100 ml meal of water, currently at 100.0 degrees Celsius

is inedible because food must be between -5.0 and 65.0 degrees to be consumed!




Would you like to eat more of the food you have? <strong><em>y</em></strong>




Please describe the food you have: <strong><em>biscuit</em></strong>

What is the volume of the food you have (in millilitres)? <strong><em>5</em></strong>

True/False — Is the food at room temperature? <strong><em>true</em></strong>




Your 5 ml meal of biscuit, currently at 22.0 degrees Celsius is edible because of nothing special.

There will be 0 millilitres of food remaining after you’ve eaten




Would you like to eat more of the food you have? <strong><em>n</em></strong>




3 meals were attempted.




<h2>Planning</h2>

This program (like all programs) should be developed in stages, with each stage fully implemented and tested before the next stage is attempted. Here are some suggestions that should help with your planning and development of the program.




Write a program in a file with the correct name — put very simple code in it, for example just display a message such as “program starts”.

<ol>

 <li>Work out the types of variables that will be needed to hold the necessary information and write their declarations. Some of the things that will be needed are:

  <ul>

   <li>a String entered by the user (for the description of the meal)</li>

   <li>an int entered by the user (for the volume of the meal)</li>

   <li>a boolean entered by the user (for whether the meal is at roomtemperature)</li>

   <li>a double entered by the user (for the temperature of the meal)</li>

   <li>a String for the description of why the meal is edible or inedible</li>

   <li>a boolean to remember whether it is edible or inedible</li>

   <li>an int for the volume of excess food</li>

   <li>the char entered by the user to indicate they wish to enter more meal details</li>

   <li>the count of the number of meal analyses undertaken (an int)</li>

   <li>a Scanner object</li>

  </ul></li>

 <li>Work out what ‘constant’ values will be needed to be stored in the program; these can be implemented as final Some of these could be:

  <ul>

   <li>the current room-temperature</li>

   <li>the minimum and maximum temperatures for edible food</li>

   <li>the minimum and maximum volumes that may be consumed</li>

   <li>the favourite foods and the colour of the inedible food</li>

   <li>the letters that allow the repetition of the program</li>

  </ul></li>

 <li>Work out how to use the Scanner class provided for this unit to read in values of different types entered by the user. <em>NB you will need to mix calls of </em></li>

</ol>

<em>nextLine(), </em><em>nextDouble(), </em><em>nextInt(), and </em><em>nextBoolean(). To do this effectively follow the latter three with calls to </em><em>nextLine().</em>

<ol start="4">

 <li>At this stage you should be able to write a program that will do all the things that are needed to work out the result for a single meal.</li>

 <li>To allow the user to see more you will need another loop. Think about what the loop will need and which loop (for, do, while) will be most appropriate:

  <ul>

   <li>initialisation</li>

   <li>test (should this be before or after?)</li>

   <li>body</li>

   <li>update</li>

  </ul></li>

</ol>




<h2>Program Style</h2>

The program you write for this assignment must be in a single file called AssigOne216.java.




Your program should follow the following coding conventions:

<ul>

 <li>final variable identifiers should be used as much as possible, should be written all in upper case and should be declared before all other variables</li>

 <li>variable identifiers should start with a lower case letter and all variables should be declared at the top of the main() method (but after any constants)  every if and if-else statement should have a block of code (i.e. collections of lines surrounded by { and }) for both the if part and the else part (if used)</li>

 <li>every loop should have a block of code for its body</li>

 <li>the keyword continue should not be used</li>

 <li>the keyword break should only be used as part of a switch statement</li>

 <li>opening and closing braces of a block should be aligned</li>

 <li>all code within a block should be aligned and indented 1 tab stop (or 4 spaces) from the braces marking this block</li>

 <li>commenting:

  <ul>

   <li>There should be a block of header comment which includes at least

    <ul>

     <li>file name</li>

     <li>student name</li>

     <li>student identity number</li>

     <li>a statement of the purpose of the program</li>

     <li>date o Each variable declaration should be commented</li>

    </ul></li>

   <li>There should be a comment identifying groups of statements that do various parts of the task</li>

   <li>Comments should describe the strategy of the code and should not simply translate the Java into English, e.g.</li>

  </ul></li>

</ul>

count = count + 1; // increment the count of the number of meals analysed and not:

count = count + 1; // add 1 to the count variable