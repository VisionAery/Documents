# VisionAery_LLD_ACAP (Liquid Leak Detection - Puddle)

Date Updated: March 12 2025

<br>

# Camera Requirements: 
* Axis Hardware Platform: ARTPEC-8 SoCs only
* Axis Firmware: Axis OS 11 Only 

<br>
<br>

# Setup:

1. On the Axis Camera with ARTPEC-8 SOC go to the "Apps" Tab <br>
![Image of App page on Camera Web UI](/setup_images/app_page.png "App Page")

1. Make sure both ""Allow unassigned apps" and "Allow root-privileged app" are enabled <br>
![Image of enabled radio buttons](/setup_images/enable_unassigned_and_root_apps.png)

1. Press "Add App" button and drag in or select .eap App file to install app. <br>
![Image of Install App Page](/setup_images/add_app.png)

1. Wait for app installation to complete (It usually takes a bit, >2min) <br>


1. Once the install is complete, enable the LLD App <br>
![](/setup_images/LLD_App_Enabled.png)

1. Wait for the app to fully stary, then press the yellow "Open" button to open the Web UI for the LLD App <br>
![](/setup_images/Open_Button.png)

1. LLD Axis ACAP Web UI <br>
![](/setup_images/LLD_ACAP_Web_UI.png)

<br>

# Licensing:

## For app licensing, please send "Device BLOB" to  [support@visionaery.com](mailto:support@visionaery.com)
### The Device BLOP can be found on the LLD ACAP App web UI unfer the "License" Tab
![](/setup_images/App_License_Page.png)


<br>

# Events/Alarms and Telemetry Data


| Type: | Data Description |
| ----------- | ----------- |
|Events/Alarms:| Message sent when detection meets or exceeds the user set thesholds for each event 
|Telemetry:| Message sent at user specified time interval

## Events/Alarms
| Event | Description |
| ----------- | ----------- |
| puddle_detected | Sent when puddle area is above set threshold |

## There are 3 pathways in which the LLD ACAP App can send out events or telemetry data 
1. Device Event on Axis Camera using its VMS Integration
1. MQTT using Axis Cameras MQTT Connection to Broker
1. MQTT directly from the LLD to Broker 

## LLD MQTT Topics:
| Event Pathway | Event/Telemetry | Default MQTT Topic |
| ----------- | ----------- | ----------- |
| From Axis MQTT | Event | axis/MAC_ID/event/tns:axis/CameraApplicationPlatform/LiquidLeakMonitor/Puddle_Detected |
| From Axis MQTT | Telemetry | axis/MAC_ID/event/tns:axis/CameraApplicationPlatform/LiquidLeakMonitor/Telemetry |
|  |  |  |
| From App MQTT | Event | leak-detector/alarms/puddle_detected |
| From App MQTT | Telemetry | leak-detector/status |

<br>
<br>

# Release Notes:

## Pre-Release v1.0.3

* Bug fixes:
  * Bounding Box alignment bug fixed
  * Fixed integration with Axis VMS
  * Fixed display of augmented video stream in NxWitness VMS

## Pre-Release v1.0.2

* Bug fixes

## Pre-Release v1.0.1

* Change port of webserver

## Pre-Release v1.0.0

* First release

<br>
<br>

# Known issues

* Model not as accurate as it needs to be. Issue with running on Axis DLPU and Image re-size layer.

