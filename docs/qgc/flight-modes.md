This article provides an overview of the available flight modes.

 
### Recommended Flight Modes

In general you should progress with the flight modes in the order listed below, being sure that you are comfortable 
with each before progressing to the next: 

* Stabilize
* Alt Hold
* Loiter
* RTL (Return-to-Launch)
* Auto


### Stabilize

Stabilize mode passes the pilot inputs directly to the motors, with stabilization. This mode allows you to fly your
vehicle manually, but self-levels the roll and pitch axis.

!!! tip
    If you’re learning to fly, try Alt Hold or Loiter instead of Stabilize.
    You’ll have fewer crashes if you don’t need to concentrate on too many controls at once.


### Alt Hold
    
In altitude hold mode, Copter maintains a consistent altitude while allowing roll, pitch, and yaw to be controlled
normally. The throttle is automatically controlled to maintain the current altitude. Roll, pitch and yaw operate the 
same as in Stabilize mode meaning that the pilot directly controls the roll and pitch lean angles and the heading. 
    

### Loiter
   
Loiter Mode automatically attempts to maintain the current location, heading and altitude. The pilot may fly the copter
in Loiter mode as if it were in a more manual flight mode but when the sticks are released, the vehicle will slow to a 
stop and hold position.
    
    
### RTL (Return-to-Launch)
    
RTL mode navigates Copter from its current position to hover above the home position. The copter will first rise to the 
minimum relative altitude (RTL_ALT) before returning home or maintain the current altitude if the current altitude is
higher than RTL_ALT. To learn more about RTL Mode and its parameters please navigate to [this page](http://ardupilot.org/copter/docs/rtl-mode.html).
    
### Auto

In Auto mode the copter will follow a pre-programmed mission script stored in the autopilot which is made up of
navigation commands (i.e. waypoints) and “do” commands (i.e. commands that do not affect the location of the copter
including triggering a camera shutter).

<hr>

!!! tip
    If you want to learn more about the available flight modes, please, refer to the ArduPilot docs available
    [here](http://ardupilot.org/copter/docs/flight-modes.html).