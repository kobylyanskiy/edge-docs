### Intro

This quickstart tutorial will guide you through the initial setup of Edge drone controller and its accessories.
In the end you’ll get a configured Edge drone controller that streams video from a camera to your laptop.
After that you can proceed to the hardware installation guide and install your Edge in a frame.

!!! tip
    If you encounter any issues performing these steps, we are happy to help you out on our [**community forum**](http://community.emlid.com/).

## Connect Edge GNSS module

Edge GNSS module is a positioning device interfaced via CAN bus. It includes a GPS/GLONASS/BeiDou/Galileo receiver, a high-precision barometer, and two 3-axis compasses.
The module has 2 ports internally connected to the same CAN bus.

To connect Edge GNSS module to Edge use a JST-GH-4P-to-JST-GH-4P cable.

* Connect one end of the cable to any of the CAN ports on Edge GNSS module
* Connect another end of the cable to any of the CAN ports of Edge drone controller


<div style="text-align: left;"><img src="../img/quickstart/edge_to_gnss_top_view.png" style="width: 500px;"></div><br>

You can connect the wire to any of the two CAN ports on Edge

## Connect video camera

Camera should be connected to HDMI-IN port on Edge.
In case you are connecting an action camera then most likely it will have Micro-HDMI connector as well.
In that case you would need Micro-HDMI to Micro-HDMI cable to connect the camera to Edge.

<div style="text-align: center;"><img src="../img/quickstart/camera_to_edge.png" style="width: 550px;"></div><br>

!!! danger
    Turn off the camera’s internal WiFi, otherwise it may interfere with RC equipment or Wi-Fi modules

!!! warning
    Turn on the camera after Edge has booted (led-status.md reference)

!!! warning
    Turn the camera on after Edge is [booted](led-status.md)

!!! warning
    Turn off the camera’s WiFi

!!! tip
    Resolution and frame per second value of the input stream may vary. Maximum supported video format is 1080p 30fps

## Connect Wi-Fi modules

Edge kit comes with two identical long-range Wi-Fi modules in separate boxes.
Use one to connect to Edge drone controller and another one to connect to a computer.

### Connect Wi-Fi module to Edge

<div style="text-align: center;"><img src="../img/quickstart/edge_to_wifi_top_view.png" style="width: 550px;"></div><br>

To connect Wi-Fi module to Edge use a Micro-USB to JSH-GH-4P cable.

* Plug JST-GH-4P connector into Edge port labeled USB2
* Plug Micro-USB connector into Micro-USB port of the Wi-Fi module

### Connect Wi-Fi module to a computer

We need to connect your laptop to your Wi-Fi module. In order to do that you need to perform two simple steps

<div style="text-align: center;"><img src="../img/quickstart/wifi_to_laptop.png" style="width: 550px;"></div><br>

Use Alfa’s Micro-USB-3.0 to USB-3.0 cable from the Wi-Fi module box

* Connect Micro-USB-3.0 one end of the cable to the Wi-Fi module
* Connect the other end to the USB port of your laptop/desktop computer

## Software installation

### Wi-Fi module driver

Now we need to install the driver for your Wi-Fi module. The instructions depend on your OS.

#### Windows

Note: To update drivers you need network connection.
*   Connect Wi-Fi module to laptop.
*   Start device manager:
    * Open the "Run" dialog box by pressing and holding the Windows key, then press the R key ("Run")
    * Type devmgmt.msc

<div style="text-align: center;"><img src="../img/quickstart/devmgmt.png" style="width: 550px;"></div><br>

* Expand Network Adapters category
* Right click on “Realtek 8812AU Wireless LAN 802.11ac USB NIC” and select Update Driver Software
* Select Search automatically for updated driver software

<div style="text-align: center;"><img src="../img/quickstart/windows_drivers_search.png" style="width: 550px;"></div><br>

Windows will find the newest version of driver and install it.

<div style="text-align: center;"><img src="../img/quickstart/device_manager.png" style="width: 550px;"></div><br>
