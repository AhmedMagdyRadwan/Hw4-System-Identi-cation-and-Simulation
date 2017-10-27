# Hw4- System Identication and Simulation

Ev3 Line Following  Robot using  PID controller

Description of the project: 

  The project is to create a Lego Mindstorms EV3 line following robot that has the ability to follow any path using color sensor 
  (light sensor), the robot is controlled using PID program which is created on LEGO MINDSTORMS EV3 Home Edition software.
  and the PID paameters are tuned using different methodes like zeglar 
  
  
  
Description of the work process:

1) first i started by building the robot using the supplied manual book with the tools/parts box as a refrence.
    -The robot has two front wheels, each connected to a large motor.
    -One swivel wheel in the back.
    -one color sensor.
    -motors were connected to B and C  ports on the robot and color sensor to port 3.
    
 2) I used the LEGO MINDSTORMS EV3 Home Edition software to create the code which i transfered it to the robot using  Bluetooth support which is included in the brick.
 
 3) after assembling the robot and connected it to my laptop through bluetooth, first started to calibrate the color sensor as it also works as a Light sensor, so by choosing the mode for Measuring the reflected light mode started to store in two variables the white and black colors.

 4) depending on the below concepts started to tune the values of Ki,Kp,Kd :
        - The proportional value is approximately proportional to the robot’s position with respect to the line.
        - The integral value records the history of the robot’s motion: it is a sum of all of the values of the proportional term that were recorded since the robot started running.
        - The derivative is the rate of change of the proportional value.
        
 5) so started by giving values to Kp while keeping  the othe factors of the controller Ki,Kd equal zero.using the following equation:
 
"how much to turn = Kp * ( midpoint - Light Sensor Reading )"

6) for the Ki, while working inside a loop "integral = integral + error", the main goal is decrease the error by makingth integral part to be zero and that can be achieved by applying another negative error, So the robot will move from one side to the other of the midpoint in order to cancel the error and be exactly on the midpoint.

7) 

 
