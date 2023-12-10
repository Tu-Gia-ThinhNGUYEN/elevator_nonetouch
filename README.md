# 1. Overview

This is my project for Programmable Logic Controller (PLC) subject. With an idea is a user can be follow the realtime status of the cabin in elevator, make plan and select floor without touch elevator button. The project includes hardware sub-system controlled by PLC iQ-F series of Mitsubishi Electric. One IoT system using ESP8266 to show update QR code from server and SCADA system, one web app and one mobile app for user.

In this project, the hardware sub-system is four floors elevator model which controlled by PLC Mitsubishi iQ-F FX5U. It definitely has SCADA system which was developed on Windows Form App, this part of system is not only using for control and supervise hardware model but also using for back-end server for webserver and mobile app. One web app using hosting of Firebase and one mobile app was developed on Unity3D (cause for app is able to be cross platform app).

![results](/images/Slide3.PNG)

# 2. Results

The SCADA system is developed in Windows Form App with C#. This system is used for supervise and control elevator model. In addition, this system also aquisition data from under layer, store data to the local storage and cloud (Firebase), this system also plays role of back-end for webserver read data from realtime database then handle requirement of user from webserver to PLC and update respond of PLC to realtime database.

The webserver is using hosting of Firebase. All requirement of user will be updated to realtime databse, which will be handled by SCADA system, then responds and updates all status for user. So webserver is able to be online over internet through this method.

Link of webserver is here: https://elevatornonetouch.web.app/

Preview of website:

![results](/images/Slide9.PNG)
