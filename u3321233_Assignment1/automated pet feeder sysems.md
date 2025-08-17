
Step1: Understand and Define the Problem (Analyse)

My Automated Pet Feeder System is to make the user fed their pet easy when they busy, when they been away and save time and low-cost.
1 The feature 
Software: programing language 
Hardware: Microcontroller
Alert system
Container and to store food amount
2. Input and output needed
	Real-time clock, food level sensor, and weight sensor.
	Motor 
	Alert signal
3. Assumption
Dry food for (Dispense food)
For the memory will delete automatically after 30 days

Step2: Organize and Describe the Data

Input
1.	Real-time clock
2.	Food level sensor
3.	Weight sensor under bowl or container 

Expected output
1.	rotate motor 
2.	Alert LED or any voice/sound 
Every 30 minutes check time


Variable	Type 	 Sample values	Operational parameters
Real-time clock	Input	8am and 6pm	Check every 30 minutes
Food level sensor	Input	5 cm(full) 20 cm (low)	When alert exceed 12 cm
Weight sensor under bowl	Input 	0-100g	Average 500g
Rotate motor	output	1 – 8 seconds	Runtime 5 seconds
Send alert system	output	NO/OFF	120 seconds for per alert
Data table

Step4 Implement the Solution (word coding)

There are 5 variable 
1.	Real-time clock
2.	Food level sensor
3.	Weight sensor
4.	Motor
5.	Alert system

1 on the system 
Check the feeding time
If correct time at 8am and 6pm 
Check the food level greater than 20 cm the alert system send “no food”
If the food level less than 5 cm the alert system send “full” continue to next step

2 Dispense food
Wait and check the weight bowl change or unchanged 
Read the bowl weight 
If the bowl weight change send alert “pet has eaten”
If not send alert “food not eaten”
Wait before next check 10 minutes




Step5 Test and Refine he Solution (Debug and Verify)

1 pet eats as expected 
Input: When the feed time correct at 8am and 6pm. The system provide motor rotate to dispense food into bowl. The weight sensor shows signal after pet eats 10 minutes
Output: no error alert 
2. Pet does not eat 
Input: the feeding time correct, and food dispensed the sensor unchanged after 10 minutes 
Output: the alert sent “food not eaten”
3. Food bin is empty
Input: the feeding time correct, sensor show container empty. And the motor rotate but no food.
Output: Alert sent “no food “
All the steps are output matched.
The food could be dispense directly by any if needed



