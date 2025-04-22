# Wave Integration Guide

## Setting Up Wave

The following steps will instruct on setting up the Hanwha Wave application by adding the camera, setting up alerts, bookmarking, and licensing Wave. If you wish to configure the system to an external Wave Server, Skip to the second part of the guide.

### Add Device to Wave

1. Go to [this link](https://hanwhavisionamerica.com/wisenet-wave-vms/) to download and install the Wave client that's compatible with your operating system.
2. Open the application, if a dialog box appears asking to trust "Ubuntu", select I trust this server.
3. On the Dialog box on the next page, select "Setup New System".
4. Add a friendly name for the server in the text field, then select the ![](https://t9011036865.p.clickup-attachments.com/t9011036865/0c9ec987-027f-48c0-a2cf-b977c99b699a/Screenshot%202024-01-24%20at%203.57.41%20PM.png) button.
5. Setup an administrator password, then click ![](https://t9011036865.p.clickup-attachments.com/t9011036865/f6aaf644-5d4f-4fd3-b76a-6520f42d591a/Screenshot%202024-01-24%20at%203.57.41%20PM.png) again.
6. Click "Continue" on the subsequent dialog box that pops up.
7. The Next page you'll see is the blank Wave GUI. On the left side you'll see the name you gave the server in [step 4](https://app.clickup.com/9011036865/docs/8chk0p1-2791/8chk0p1-2131?block=block-6cda325a-01d7-4fbd-91e3-8a6cd7f820ef). Right click the server, then select "Add Device" on the dropdown menu.
8. Type in the IP address, username, and password of the camera you wish to add in order to add it to the system, followed by the ![](https://t9011036865.p.clickup-attachments.com/t9011036865/d14bc3c1-6183-48e7-b153-ccf774578247/image.png) button.
9. Add the device, then add the following:

`Address:` [`rtsp://ip.of.dev.ice/stream`](rtsp://ip.of.dev.ice/stream)

Port: 8554

Login: admin

Password: Visionaery123!

Make sure that the port number and path/endpoint match what was set while setting up the output stream from the Flare application in [earlier steps](https://app.clickup.com/9011036865/docs/8chk0p1-2791/8chk0p1-2131?block=5c5f99e6-cdb9-48e2-9284-cf56d180283e). Then click ![](https://t9011036865.p.clickup-attachments.com/t9011036865/e894c6ba-f889-40a7-826a-3e88f2c5e3b7/image.png).

* * *

### Add Event Rules in Wave

1. If you double click on the device from the Tree on the left side, you should be able to then view their live feeds.
2. Right click on one of the cameras, then select "Camera Rules" from the dropdown.
3. In the window that pops up, select the![](https://t9011036865.p.clickup-attachments.com/t9011036865/e0e17f47-b332-4121-8c4b-b8a9bedbe923/image.png) button in the top right.
4. Add to the following fields:
    1. When = Generic Event
    2. Source contains = Alarm
    3. Do = "Show On Alarm Layout"
    4. Enable ![](https://t9011036865.p.clickup-attachments.com/t9011036865/36717bc7-93a4-4690-9d33-250d8651d240/image.png)
    5. Disable ![](https://t9011036865.p.clickup-attachments.com/t9011036865/07914161-b88e-4fba-8b7a-1257589f647f/image.png)
5. We'll then select the "Add" Button again, then add the following to the new rule:
    1. When = Generic Event
    2. Source = Bookmark
    3. Do = Bookmark
    4. Enable ![](https://t9011036865.p.clickup-attachments.com/t9011036865/72a66381-9cc0-4b4d-af6b-c5ceebb74d97/image.png)
6. We'll then select the "Add" Button again, then add the following to the new rule:
    1. When = Generic Event
    2. Source = Overlay
    3. Do = Show text overlay
    4. Enable ![](https://t9011036865.p.clickup-attachments.com/t9011036865/4c9ec6fb-3f53-4a7e-85e5-5819f82be1d5/image.png)
    5. Set ![](https://t9011036865.p.clickup-attachments.com/t9011036865/57372c93-3fdd-4877-9655-6aba5b445f1f/image.png)
7. We'll then select the "Add" Button again, then add the following to the new rule:
    1. When = Generic Event
    2. Source = Notify
    3. Do = Show Desktop Notification
8. This completes the setup of the Wave application. Leave Wave open on your machine and return to the Dashboard Landing Page from [previous steps](https://app.clickup.com/9011036865/docs/8chk0p1-2791/8chk0p1-2131?block=block-b97788d4-1c35-4766-9130-c113261107ca)

  

![](https://t9011036865.p.clickup-attachments.com/t9011036865/1b41bf23-4b48-40f2-800d-64e078daf999/Screenshot%202024-01-24%20at%203.49.47%20PM.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/a187df9a-bb72-4e6c-b1cf-7824afbd2929/Screenshot%202024-01-24%20at%203.51.12%20PM.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/67ba1be2-a3c7-4b4f-8703-ec0826da6bb5/Screenshot%202024-01-24%20at%203.56.00%20PM.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/71b82a20-b9e0-41ec-9e24-a72460dc7b25/image.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/5ac28c1e-1a7f-424c-8d53-288c37ee9637/Screenshot%202024-01-24%20at%205.22.34%20PM.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/67287aca-2357-4d58-bd02-11c6b567ac58/Untitled.jpg)

* * *

![](https://t9011036865.p.clickup-attachments.com/t9011036865/da2ec69c-d2f2-47d3-970d-fc91aec9a79b/image.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/0e1c8e80-ef8d-44cc-b5bc-1ddbf230ac69/image.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/d0e31e1a-2acc-450a-9dbf-8f58f8ad7c88/image.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/d91607f3-28f0-4743-9b5d-1c500e04aac5/image.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/097da38b-25bf-49bb-bb7e-9f86c2107f65/image.png)

![](https://t9011036865.p.clickup-attachments.com/t9011036865/5c9f3740-02d5-4b1d-b31e-c8cefe597f59/image.png)

  

  

  

  

* * *

### To Setup events to an external Wave Server

1. From the landing page, select the ![](https://t9011036865.p.clickup-attachments.com/t9011036865/ab08d1ad-8233-4d2f-b201-3a7e57326c23/Screenshot%202025-03-14%20at%201.02.07%20PM.png) button on the top left, then select the VMS tab.

  

![](https://t9011036865.p.clickup-attachments.com/t9011036865/aeb633b3-9832-48ee-abad-55213f05eb05/Screenshot%202025-03-14%20at%201.04.24%20PM.png)

1. to direct alerts to and external server:
    1. Switch "Local on Device" to the off position ![](https://t9011036865.p.clickup-attachments.com/t9011036865/0619daa7-f7ea-41c3-932e-c2b3bd6901ec/Screenshot%202025-03-14%20at%201.05.33%20PM.png).
    2. Type the ip address of the external wave server in the ip field.
    3. Type in the user credentials of the server.
    4. Type in the camera vms ID in the last field. To acquire the Camera VMS ID:
        1. open the Wave application.
        2. Right click the Camera (not the analytics feed).
        3. Select "Camera Settings" From the Dropdown.
        4. In the resultant window, select "More Info".![](https://t9011036865.p.clickup-attachments.com/t9011036865/1365e189-02c2-4b59-b8f4-dddd26177f78/image.png)
        5. Select the![](https://t9011036865.p.clickup-attachments.com/t9011036865/d7c96c8c-dc87-4c32-a6a3-f8f7d67ab547/image.png) button to the right of where it says "Camera ID". ![](https://t9011036865.p.clickup-attachments.com/t9011036865/787a94e2-0439-40e4-b082-c405d7c29a4e/image.png)
        6. Return to the browser and paste the ID into the "Camera VMS ID" Field.
    5. Click "Save Settings"