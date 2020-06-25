# Ball_Sorting_Machine
## Team Members: Ayesha Khatun, Jing Yang Kuo, Sushil Jagmohan, Yousouf Amologbe

Our Team has worked on the 'Ball Sorting Machine Project' as a part of the MAE (Mechanical & Aerospace Engineering) Lab - I course.  As a team leads, I have organized team meetings, created different project plans, actively encouraged the team members to work on the design for better performance as well as dedicated myself in the design revision process. The overall experience gained from this Mechanical Team project gave me invaluable insights into basic mechanical system designing phases and engineering team management process.

#### Abstract
This project was aimed at designing an automated system using the fundamental theories and techniques we learned in this course. This system used an Arduino to evenly distribute 30 steel balls into three bins mounted on a ball screw. Our design involved several design components such as a color sensor, an Arduino, breadboard, and a servo motor. In general, our system partially completes the goal that is required but has some inconsistencies in certain areas.

#### Introduction
Three different materials and ball specifications are introduced. The birch, steel, and acetal resin need to be deposited into 3 separate bins. Steel and birch have the same diameter of ⅜”. The acetal resin ball is slightly smaller at 5/16”. 10 balls of each type are placed into the funnel randomly, which then directly attaches to the sorting machine to be deposited in particular compartments of collecting bin. Our goal is to design and build a system with a budget of 75$ and to sort the balls in a timely manner with precision.

Our first design began with the use of a TCS34725 color sensor which then was replaced using TCS3200 for better performance. Also, other significant change decisions had been made throughout time like time interval for each operation, restricting light passing during sensor operation, structural changes, etc. 

![System_design](/images/system_design.JPG)             ![CAD](/images/CAD_drawing.JPG) 

There were many setbacks that our project had to deal with such as lack of sufficient time, proper equipment, and an unreliable light-sensitive sensor. The only major change throughout the development was the use of a different sensor. The system is still viable but requires major tweaks to the electrical side which can result in a complete change to the design to help the sensor read the balls more consistently and efficiently. Overall our system completes the goal that is required but lacks fault detection on the electrical side of the project.

#### Design Process
The detailed report of our three design ideass, decesion process to choose a final design from the conceptual designs, system operation, instrument selection, test procedure instructions for the color sensor calibration, machine setup etc. and the detailed results of our sorting machine performance along with the arduino code developed for the operation, can be found here:

our designed sorting machine is built with a class project budget of around $40, where the detailed bill of materials is as below:

![BOM](/images/Bill_of_material.JPG) 

#### Discussion: 
##### Performance of our system:
Following is link to one of the test runs in our sorting system which visually demonstrate the mechanism and perfromance of the system:

video: 

The performance of our system is mostly based on reading from the RGB color sensor. The purpose of this system is to sort 30 balls with 3 different materials, which are wood, steel, and plastic. At the beginning of the project, the team thinks that this should be easy because those samples have distinguished color, but end up it is actually pretty difficult to obtain accurate data. First and foremost, the RGB color sensor is pretty sensitive with the light and disturbance around the operating environment, for example, we obtain a different kind of reading by scanning the same ball, this has actually become the major problems that caused our performance can only maintain with a 75% precision rate. As shown in Fig, the reading for steel ball and plastic are only have 2 readings for both, there are 5 readings for the wooden samples. The main reason why there is so many set of data ie because the light reflectability of steel ball and transparency of the plastic ball also affecting the result of the readings, but the reading for these 2 samples are acceptable. For the wood samples, they do not have a uniform color on the ball, and there are black dots around them which make the readings of the wooden one very inconsistent.


##### Design Improvements & Operartion Modifications

Several improvements were done since starting of working in our project. Since with any system working in real life, there is always room for improvements and modifications to make it more efficient, we would definitely be able to do more of improvements given more time and resources.

We took the reliability of the design to be the first priority over the speed of the system for a better engineering approach. The cost of the design had been constrained to not to be over $75 for the model.

1.Improved Reliability 
We allotted enough time for the sensor to scan each ball to collect the RGB data for the proper signal to the second servo motor to drop in the correct bin. In the beginning, we kept to around 1 second and then changed it to 1 and a half seconds in the final design. Though it might appear this tradeoff has been slowed down the system, but in reality, it was not the case. The system had a time of operation fall in a convenient range of 3 seconds for each ball sorting cycle. Also, there were structural approaches for a better design.  For more resistance to the vibration we added a base platform to the design and to limit the sensor to have into enough but not too much lighting, we blocked the whole background with a piece of cardboard. Initially, there was more distance between the color sensor and the platform where the balls drop. Later we added more layers in between to decrease the distance which helped the sensor to collect more distinguished and reliable data. The platform where the balls drop to be scanned by the color sensor was made black so that the color of background does not affect the color data of experimental objects – the balls. The final structural approach was to change the pipe from the funnel to slide down the balls to be made of clear plastic material instead of made up with paper. Though we were offered to use the pipes for this purpose provided from, we were not able to collect until the stock lasted. But the plastic pipe worked out just fine and better than the paper channel.

2.Faster operating speed:
The operation time in each step for sorting out balls has been adjusted without comprising the required time required for the critical steps. For example, the time slot for scanning each ball has been kept a bit longer, while the time difference between balls to drop to the platform is less.  Also after the color sensor data collection and sending the signal to the second servo motor, less time was allotted to slide the ball in the proper compartment.  So the total operating process became faster.

3.Cost decrease: 
Our total cost was which was $40.40, even lower than $75, the low-cost requirement of the project. Though initially, we planned to use lab equipment for cost minimization, for the very limited time allocated during lab our group’s lab session only has restricted us from the plan. So we provided both of the motor, which increased the cost a little, but the overall design was built using cardboard, glue, paper tape so the cost was minimized. Also, a low-cost color sensor TCS34725 was chosen instead of a previously chosen TCS3200 color sensor for the final design.

Constraints such as time and resources were the biggest hindrance in achieving a more improved and modified design. The shortcomings of the equipments used in our design can also be found in the final report. 

#### Proof-of-concept vs. Industrial application
A significant amount of rework on a larger scale would be needed for our design to be ready for industrial use. The system would require an additional type of sensor for example a weight just to ensure the pattern of balls sorted using a color sensor. As stated in the earlier section, the use of a color sensor only creates difficulty in separating wood and steel ball because of inconsistent color data. Also, from observations stated in the earlier section, the RGB color ranges for provided ball types are very closer to each other. But the weight of the provided different types of balls is very different from each other due to material properties. So, the additional weight sensor would make the design industrially reliable with great accuracy. 

The function of the color sensor also depended significantly on the lighting surrounding during the scan of the balls. So, to make it industrially applicable, it is impossible to rely on bringing the system to darker spots for the operation, therefore built-in less light passing compartment would be needed surrounding the color sensor to enable the sensor function properly. 

The system would also need a proper design of sorted balls collecting bin. Because the wood and plastic balls are very light to easily bounce off while sliding down the ladder and only having a 3-compartment bin kept in an appropriate position is the best way to collect the balls. So, properly designed built-in compartments attached along with the main system or having an attached pipe of adjustable length with the ladder can help to complete the ball transfer perfectly. Finally, if parts of the system would be welded together, it would be easier to move around, making it more industrially a better design. 

In terms of improving the quality control of our system, if given more time we could test different types of color sensors to find an optimal set up that will have better performance in reading consistent RGB values ignoring minimal changes due to lighting or vibrations. Our group would also be able to add a proper ball collecting beams after the balls are sorted according to their color. Another solution would be to make the ladder by itself more thoughtfully designed so that it ensures sliding down the balls perfectly to each collecting compartments.

Finally having a fault detection mechanism and response to the error using a third arm attached to the system to send back the faulty ball to the sensor would solve our issues of faulty operations and allow our system to be used in an industrial setting. 


#### References
[1] Estes, Aaron. MAE 334: Mechanical and Aerospace Engineering Lab I. (2019) https://ublearns.buffalo.edu/bbcswebdav/pid-4927765-dt-content-rid-22317251_1/courses/2191_16097/MAE%20334%20-%20Lab%201%20-%20Procedure%20-%20Spring%202019.pdf 

[2] Armstrong, Jason. Lab Report Guidelines. Department of Mechanical and Aerospace Engineering, 25 Jan. 2019, https://ublearns.buffalo.edu/bbcswebdav/pid-4903664-dt-content-rid-21904548_1/courses/2191_ 16097/MAtjE%20Lab%20Report%20Guidelines_V5.pdf 

[3] Hitec HS-422 servo motor. (n.d.). https://www.robotshop.com/en/hitec-hs-422-servo-motor.html 

[4] TCS34725 RGB color sensor for arduino. (n.d.). https://www.robotshop.com/en/tcs34725-rgb-color-sensor-arduino.html

[5] A. Raihanian and A. Estes, Lab 2: Instrument Calibration, University at Buffalo, 2019

[6] Estes, Aaron. MAE 334 Mechanical and Aerospace Engineering Lab 1. Lab 4 -Experimental Analysis of a Flexible Beam. Spring 2019. https://ublearns.buffalo.edu/bbcswebdav/pid-4969982-dt-content-rid-23570746_1/courses/2191_16097/MAE%20334%20-%20Lab%204%20-%20Procedure%20-%202019.pdf
