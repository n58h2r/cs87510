java c
ENGE 1215
Fall 2024
D3. MATLAB Challenge #3
(Individual – 5 points)
Due by Thursday, October 10, 2024
Purpose
In this MATLAB challenge, you will be introduced to output methods for informing users/consumers like plots and data analysis. This assignment also encompasses learning MATLAB’s basic input and output of data files. This challenge will help you learn how to create outputs with various formats in the command window, to save data, and to import data and use it. You will also need to analyze the data you see to give an informed opinion on the situation. This challenge is divided into two problems. For each problem, write formatted text, % comments, and code within the provided .mlx template.   Work for each problem should be part of a section that you could run individually, or altogether with the rest of the code as described in class.
Reminders
A few reminders as you prepare your solution:1) Start with the provided mlx template and replace the name and date place holders at the top of the mlx file with your own information.2) You will need to add comments (these can be text mode in the mlx and/or % comments within the code) to explain major sections of the code.3) It is also good practice to use clear and clc as the first executable commands.  Use the semicolon (;) to suppress echoes of value assignment statements.4) Input prompts should be designed so that the user understands what they need to enter.5) Output should include text to describe what values are being output as well as the values themselves.6) Unless otherwise stated, you may use any output method you prefer (disp or fprintf).   Your output text and values may show on a single line or multiple lines.7) Any images should have legible text.8) Remember that MATLAB does not allow any special characters in the file name except the underscore.9) Use the variable naming conventions described in lecture.10) Remember to use the appropriate file naming conventions.
Problem 1 (of 2): Dry Erase Markers
As the new boss of an office supplies company in Pennsylvania, one of your jobs is to keep track of the number of dry erase markers in your inventory. Typically, your company manages to sell 250 dry erase markers in one week. Initially, you have 5000 dry erase markers in your warehouse. Based on manufacturing and shipping constraints, your current dry erase marker supplier periodically ships a certain number of dry erase markers every 4 weeks. Use MATLAB to figure out how many dry erase markers you will be left with by the end of the year (52 weeks).
Your program should:1. Create a variable called ‘initialInventory’ that stores the number of dry erase markers initially in the warehouse.2. Create a variable called ‘sellRate’ that stores the number of dry erase markers sold each week.3. Create a time vector containing the week number (1 to 52).  This vector should be stored in a variable called ‘weekNumber’.4. Read the StationerySupplier1.csv file (you can download a copy from the D3 link) that contains a running sum (cumulative sum) of the dry erase markers that the supplier has sent you so far. Store the cumulative dry erase markers you receive as a vector in a variable called ‘cumulSupply’.5. Calculate the number of dry erase markers in the inventory every week using the following formula: inventory = initialInventory - sellRate*weekNumber + cumulSupply6. Combine the vectors into a single two-column matrix. Column 1 should contain the week number and column two should contain the number of dry erase markers in the inventory (the vector inventory).7. Create a .csv file containing the two-column matrix and name it as follows “LastnameFirstname_Inventory.csv”8. Display a message that contains the number of dry erase markers left in your inventory at the end of the year.
Create a sample run.  The first five rows of your csv file from your resulting run may look similar to this:
Week number
Number of dry erase markers in inventory
1
5731
2
5481
3
5231
4
4981
5
5455
Problem 2 (of 2): Carbon Footprint
You are tasked with analyzing the carbon footprint of a fleet of vehicles. The fleet manager has provided you with data on the number of miles driven by various vehicles of a certain size in t代 写​ENGE 1215 D3. MATLAB Challenge #3 Fall 2024Matlab
代做程序编程语言he fleet and the corresponding amount of carbon dioxide (CO2) emissions recorded. Your task is to use this data to better understand the relationship between miles driven and CO2 emissions, and to predict the potential emissions for a new trip length.
Write a MATLAB program to do the following:1. Use readmatrix to load the FleetEmissionData.csv file (you can download a copy from the D3 link), which contains two columns:· Column 1: Miles driven by each vehicle during the week· Column 2: CO2 emissions (in kg) corresponding to the miles driven.2. Create a scatter plot of CO2 emissions (Y-axis) vs miles driven (X-axis). Remember to include appropriate axis labels (with units) and a descriptive title.3. Use polyfit to determine the coefficients of a linear relationship between miles driven and CO2 emissions. You can assume the relationship is linear, so fit a first-degree polynomial (line). Add this line to your scatter plot to represent the estimated relationship (remember to use “hold on” to do an overlay).4. Use fprintf to display the equation of the best fit line.  Format the slope (m) with 2 decimal places and the intercept (k) with 0 decimal places.  Hint, to format a number with 0 decimal places, you can use %.0f. Remember to also explain the variables as part of the equation.5. Calculate the estimated CO2 emissions for a trip of 500 miles by using the formula for the best fit line.   Use disp or fprintf to output the value.  The predicted emissions for a 500-mile trip should be about 257 kg.
Based on the scatter plot that you created in step 2, answer the following question in the space provided in the mlx template:
There are several vehicles that have driven approximately 400 miles, but the CO2 emissions have a relatively large variation (ranging from about 100kg to about 280kg, see Figure 1.  What are two factors that could have contributed to such a large variation in the amount of CO2 emissions?Figure 1. Part of the graph highlighting variation in CO2 emissions for vehicles that that have been driven for about 400 milesDeliverables
Please submit the following three files to Canvas:· .mlx file for Problems 1 and 2 combined· A template for your .mlx   file is provided in the D3 link on Canvas.· Make sure the name and the date at the top of the .mlx file are updated with your information.· Use the file naming convention D3_yourPID.mlx· .csv file for Problem 1 above· Use the file naming convention LastnameFirstname_Inventory.csv· A single .pdf file of your .mlx fileo Make sure you run your .mlx with the sample run input values before making your PDF.  Use Live Editor>Export>Export to PDF menu option in MATLAB to make your PDF.   Graders need to be able to see the code and the sample output values/ figures in your PDF.  Use the file naming convention D3_yourPID_optional descriptor.pdf
If your computer is giving your problems with converting the MATLAB plot to your PDF, here are a few possible things to try to;
1. See if someone from SWAT (swat.eng.vt.edu) can help you with your graphics problem
2. Use the "print" option and choose PDF annotator if you have that installed (PDF annotator comes with your engineering bundle)
3. See if you can do a screen capture of the graph and insert that image into your mlx and then try exporting
4. Do a screen capture of your graph, then open your pdf in PDF annotator, add a new page to your pdf and paste the screen capture of your graph into it.
5. Copy and paste images of your mlx file into a document or PDF annotator and save as a PDF.
If you do #3, 4 or 5 successfully, please add a comment to the D3 link that lets the grader know that you had to do a workaround due to your graphics problem.
Rubric
Your work will be evaluated based on· Program functionality· Correctness of solutions· Good programming practices - especially with respect to commenting and variable naming· Readability and inclusion of requested elements
You can see the point breakdown in the table below.DescriptionPercentage
Instructions Followed~10
P1 Dry Erase Markers~30
P2 Carbon Footprint (code)~40
P2 Carbon Footprint (analysis)~5
Coding Practice: Thorough Commenting~10
Coding Practice: Variable Naming~5



         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
