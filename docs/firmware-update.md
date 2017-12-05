## Grab the latest image

Download the latest available image

* [v1.1](https://files.emlid.com/edge/firmware/2017-11-14-edge-emlid-v1.1.img.xz)

## Connect Edge to your PC

To connect Edge to your computer use USB-cable and PC port on Edge. 

<div style="text-align: center;"><img src="../img/firmware-update/pc_to_edge.png" style="width: 550px;"></div><br>

## Flash your Edge

The instructions depend on your OS

### Windows

* Download [Etcher](https://etcher.io/) (v1.2.0 or later)
* Extract the downloaded file
* Run

Click `Select image` and choose the archive file with image

<div style="text-align: center;"><img src="../img/firmware-update/etcher_windows_select_image.png" style="width: 550px;"></div><br>

Click `Select drive` and wait while Etcher initializes your Edge

<div style="text-align: center;"><img src="../img/firmware-update/etcher_windows_select_drive.png" style="width: 550px;"></div><br>

Waiting...

<div style="text-align: center;"><img src="../img/firmware-update/etcher_windows_cm_initialization.png" style="width: 550px;"></div><br>

Finally, there!

<div style="text-align: center;"><img src="../img/firmware-update/etcher_windows_cm_initialization_done.png" style="width: 550px;"></div><br>


Click `Flash`. 

!!! tip
    The process will take a few minutes. Please, be patient!


<div style="text-align: center;"><img src="../img/firmware-update/etcher_windows_flash.png" style="width: 550px;"></div><br>


### Linux

Open QGroundControl, choose `Setup` <img src="../img/firmware-update/qground_setup_ico.png" style="width:30px; vertical-align: middle"> menu and go to `Firmware` tab

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_start.png" style="width: 800px;"></div><br>

Plug in your device (If you did not do it before) and wait until QGroundControl automatically detects it.

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_edge_available.png" style="width: 800px;"></div><br>

Next, click on the `Connect` button to start initialization your device.

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_edge_connected.png" style="width: 800px;"></div><br>

QGroundControl will ask you for administrative privileges.

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_auth.png" style="width: 800px;"></div><br>


Wait several seconds while QGrounControl initializes your device.

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_init_start.png" style="width: 800px;"></div><br>

After initialization completes, you'll see this dialog:

* (1) You can enable or disable checksum computation 
* (2) You should choose file with Edge firmware

!!! tip
	If you enable checksum computation, QGroundControl will check correctness of flashing.

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_prefs_menu.png" style="width: 800px;"></div><br>

Next, you should select Edge firmware image

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_select_image.png" style="width: 800px;"></div><br>

After file is selected, press `Ok` at the top right corner of the dialog window and firmware update will start.
You can cancel the update process by pressing `Cancel` button.

!!! tip
	If you enable checksum, you should wait while QGroundControl computes it from your image and from image which is written to the device. The progress of computation will be shown on the progress bar.

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_flasher_running.png" style="width: 800px;"></div><br>

When firmware update complete, you can unplug your device.

<div style="text-align: center;"><img src="../img/firmware-update/qgc_upgrader_linux_end.png" style="width: 800px;"></div><br>
