# Smart_car_parking_system

WORKING PRINCIPAL 
System Initialization: When powered on, the Arduino UNO begins by initializing all connected components,including the IR sensor, servo motor, and 16x2 LCD display (with I2C module). The display shows a welcoming message or the current parking status, such as "Parking Available Slots" or "Parking Full."

Vehicle Detection: An IR sensor at the entrance detects incoming vehicles. When a car approaches, it interrupts the infrared light from the sensor. The sensor detects this interruption and sends a signal to the Arduino UNO, confirming that a vehicle is present.

Decision Making: Upon receiving the vehicle signal, the Arduino UNO checks for available parking spaces. If spaces are available, it instructs the servo motor to open the barrier gate and updates the LCD to display the remaining spots. Barrier Gate Operation: The servo motor activates to lift the gate when a vehicle is detected and parking is available. The gate remains open briefly to allow the vehicle to enter. 

Parking Slot Management: After a vehicle enters, the Arduino updates the count of available spaces. If the parking lot is full, the system will not open the gate,and the LCD will display a "Parking Full" message. Continuous Monitoring: The system continually checks the parking lot status using the IR sensor to detect any new vehicles. The servo motor is prepared to open or close the gate depending on parking availability. 

User Interaction: The 16x2 LCD provides real-time updates to users, including the number of available spaces, a "Parking Full" message when necessary, and instructions or status updates during entry. 

System Reset: The system automatically resets after each car enters, updating the display and preparing the servo motor for the next vehicle, ensuring continuous and efficient parking management.







NOTE:Took Reference from Youtube
