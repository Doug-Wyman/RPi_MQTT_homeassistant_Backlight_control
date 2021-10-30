<!DOCTYPE html>

<html lang="en" data-color-mode="auto" data-light-theme="dark" data-dark-theme="dark" xmlns="http://www.w3.org/1999/xhtml">
<head>
    <meta charset="utf-8" />
    <title>RPi remote Backlight</title>
</head>
<body style="word-wrap: break-word; color: white; background-color: black;">
    <h1>MQTT Raspberry Pi Backlight remote control</h1>
    <p>Remote Control for Touch screen backlight on Raspberry Pi for control by <a href="https://www.home-assistant.io/" rel="nofollow">Home Assistant</a></p>
    </br></p>
    <h1>Installation</h1>
    <p>
        1)  On the Raspberry Pi copy the MqttScr.py and RpiMqtt.conf files to a convenient folder.
        The folder used in testing was /var/www/html. </br>
        If this location is changed, that change needs to be reflected in the mqttscrD file.</br></br>
        2)  For the start and restart to work properly python3 needs to be linked to pyscr.</br>
        Enter the command "sudo ln /usr/bin/python3 /usr/bin/pyscr" </br>
        This allows the program to be stopped and started without affecting other python3 programs.</br></br>
        3)  To enable startup at boot and restart of the app, copy mqttscrD to the /etc/init.d folder.
        </br>Then activate it by typing in "sudo update-rc.d mqttscrD defaults" </br>
        This installs mqttscrD as a service.</br></br>
    </p>
    <h1>Homeassistant</h1>
    <p>
        The backlight control will look like a light to Homeassistant</br>
        It can be added to the lights.yaml file with the entry in lights.yaml.</br>
        It can also be added to configuration.yaml as a light.
    </p>
    <h1>Notes:</h1>
    <p>Suggestions branches or anything to improve this is welcome.</p>
</body>
</html>
