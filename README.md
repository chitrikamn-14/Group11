**EMBEDDED LAB PROJECT**



PROBLEM STATEMENT:
   	
To create a system that tracks room occupancy using an LED ring that indicates the room's status. When someone enters the room red LED glows and when leaves a 15-minute timer starts to allow for cleaning. Once the timer finishes, a green light signals that the room is clean and ready to use again.


SOLUTION:

·  Switches as Input:
* SW1 (PF4): Acts as the "Enter" button. When pressed, it indicates that someone has entered the room.
* SW2 (PF0): Acts as the "Exit" button. When pressed, it indicates the room is now vacant and starts a 15-minute cleaning countdown.
* 
·  LED Ring Behavior:
* Occupied (Red): SW1 press lights the LED ring in red.
* Vacant & Cleaning (Blue): SW2 press initiates a 15-minute countdown, turning the LED ring blue.
* Available (Green): After the timer expires, the LED ring turns green to show the room is ready.
* 
·  Reset Condition:
* If SW1 is pressed while the countdown is active, the room status resets to "Occupied" (red) and stops the cleaning timer.


BLOCK DIAGRAM:

Tiva C Series
Micro              -------------------->      LED Ring
Controller


FLOW CHART:

![image](https://github.com/user-attachments/assets/4b520bb9-4ceb-40c6-a8a7-478eaca296bc)
