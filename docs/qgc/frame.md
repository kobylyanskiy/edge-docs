### Vehicle Setup

You can select your vehicle type using QGroundControl.
After starting QGC go to the `Vehicle Setups` menu <img src="../../img/qgc/vehicle_setup_menu.png" style="width:30px; vertical-align: middle">  and there choose `Vehicle` tab

<div style="text-align: center;"><img src="../../img/qgc/vehicle_setup_button.png" style="width: 150px;"></div><br>

In the `Vehicle Setup` Settings you can set one of the following vehicle types:

* ArduPlane
* ArduCopter
* ArduCopter-heli
* ArduRover
* ArduSub

<div style="text-align: center;"><img src="../../img/qgc/vehicle_selector.png" style="width: 800px;"></div><br>

After choosing the required type of vehicle click on `Apply and Restart` button. A confirmation window will appear

<div style="text-align: center;"><img src="../../img/qgc/apply_restart_button.png" style="width: 300px;"></div><br>

After pressing `Apply` button Edge will restart with the selected ArduPilot binary. QGC will
disconnect from the autopilot after some time.

!!! note
    QGC should reconnect to Edge if you have enabled AutoConnect for UDP

### Airframe setup

!!! note
    Airframe Setup is only available on ArduCopter vehicles

Go to `Airframe` tab

<div style="text-align: center;"><img src="../../img/qgc/airframe_setup.png" style="width: 700px;"></div><br>

There you may choose Frame Class (Quad, Hexa, Octa, etc) and Frame Type (Plus, X, H, etc) of your copter.
