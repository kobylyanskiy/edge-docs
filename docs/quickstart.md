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

## Connect Wi-Fi

You need to connect the USB wireless adapter to Edge to port labeled as USB2

<div style="text-align: center;"><img src="../img/quickstart/edge_to_wifi_top_view.png" style="width: 350px;"></div><br>

And connect another end to the USB port of your laptop using original Alfa’s cable

<div style="text-align: center;"><img src="../img/quickstart/wifi_to_laptop.png" style="width: 350px;"></div><br>

## Software installation

### Wi-Fi driver

You need to install the appropriate driver for the Wi-Fi USB adapter for your OS.

#### Linux

*  Make sure you have the required build packages

    ```
            sudo apt-get install linux-headers-generic build-essential git
    ```

* Download the source code

    ```
    git clone https://github.com/emlid/8812au.git
    ```

* Compile the driver

```
$ cd 8812au
$ make -j$(nproc) && sudo make install
$ sudo modprobe 8812au

```


#### Windows
* Connect Wi-Fi module to laptop.
* Start device manager:

    ```
    Open the "Run" dialog box by pressing and holding the Windows key, then press the R key ("Run").
    Type devmgmt.msc
    ```

* Expand Network Adapters category
* Right click on “Realtek 8812AU Wireless LAN 802.11ac USB NIC” and select Update Driver.
* Select Search automatically for updated driver software.
*     Windows will find the newest version of driver and install it.

#### Mac Os X

Coming soon

### QGroundControl

#### Windows

[Download]() and double click the executable to launch the installer.

#### Linux

* [Download]()
* Launch

```
    chmod +x ./QGroundControl.AppImage
    ./QgroundControl.AppImage
```
#### Mac Os X

Coming soon

### Power from a battery

* Now you can power your Edge up using Power Module (PM). Connect 6-pin JST-GH wire to any power port on Edge (PWR1 or PWR2)

<div style="text-align: center;"><img src="../img/quickstart/pm_to_edge.png" style="width: 350px;"></div><br>


* And after connect battery to your PM

<div style="text-align: center;"><img src="../img/quickstart/batt_to_pm.png" style="width: 350px;"></div><br>


### Connect to QGroundControl

### Enjoy videostream
