Modern traffic control systems make extensive use of embedded systems to ensure the effective 
management of traffic flow. Once good example of this the control of traffic light systems. Traffic 
light systems are essential for the safe management of road traffic junctions, preventing collisions 
where traffic flow meets from multiple directions. But as well as ensuring safety, modern systems 
aim to maximise traffic flow throughout the day. This can be achieved by using different flow 
patterns at different times of the day (e.g. for peak and off-peak periods) to ensure flow is prioritised 
for busier roads, and by using sensors to manage flow (e.g. sensors that determine whether a vehicle 
is approaching a red light and turning that light green if there is no other traffic around).


This means that modern traffic light controller embedded systems are more complex than simply 
timers. They make use of active decision making, driven by sensor data under program control from
micro-controllers.

In the United Kingdom, the traffic light sequence for a standard 3 light (red, amber, green) traffic 
light is as follows:

• Red: compulsory STOP.

• Amber and Red together: get ready to GO. You may GO if the road is clear.

• Green: GO.

• Amber: get ready to STOP. You may proceed if you are already over the wait line provided 
your exit is clear.

• And back to Red.

The standard 3 light system can also be augmented by filter lights. For example, a light that permits 
a left turn to be made on a red signal. Other lights can also include options to allow cyclists to 
proceed before motor vehicles, pedestrians to make crossing requests, and override options for 
emergency vehicles (typically turning all lights red)


Requirements


You need to develop a model of the traffic light system that you are building. It should consist of 3-4 
sets of traffic lights that work together to operate a traffic junction. Here are some example images 
to give you some inspiration:
![image](https://github.com/user-attachments/assets/6972f5dd-0609-427c-944b-d0d5284bcb38)![image](https://github.com/user-attachments/assets/908a2996-496a-4329-a104-8c3557901306)

Figure 1: Example of a 3 way and a 4 way traffic light controlled junction.

Your model should incorporate the following functional requirements:
• Allow for timed control of the flow of traffic between a series of connected roads.

• The timed element should be variable so that each phase of continuous GO or STOP for each 
pathway can be varied from 20 seconds to 2 minutes by means of a potentiometer.

• You can add additional light elements e.g. filters if you think it would help manage traffic 
flow efficiently and safely.

• One of the road pathways should be designated as more important than the others (a 
designated busy route). The flow of traffic along this pathway should be prioritised at peak 
flow times. The setting of peak flow mode should be determined by a switch input to the 
system. Under peak flow conditions, the designated busy route should provide for two times 
the green period than other non-busy routes.

• There should be an option for all lights to be switched safely to red when there is an 
emergency. An emergency should be determined by a switch input to the system. When the 
emergency is over, the system should return to normal mode, starting with the designated 
busy route.

• During hours of darkness, the system should prioritise the designated busy route. The state 
of darkness can be determined using a light sensor. Under these conditions, you could also 
incorporate light sensors so that a vehicle approaching the traffic junction from a less busy 
route can automatically switch the traffic light to green for that driver if there is no traffic on 
the busy route.

You can also add any other requirements that you think would add value to the operation of the 
traffic light system in terms of managing traffic flow safely and efficiently.

You should consider the number and types of inputs and outputs this traffic light system will need to 
do its job, and ensure that the Arduino has sufficient connectivity for what you want to achieve.
