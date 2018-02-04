# Car-Heater-Package V 1.0.1
Control your car engine heater with Home Assistant

## Description
Designed for and tested with Home Assistant hassio version 0.62.1

 #### Functions:
- 2 sliders to control leaving time
- Shows current time
- Manuel switch to start/stop heater
- switch to activte function
- switch to control if it should be active all week or just weekdays

Its created as a [Home Assistant package](https://home-assistant.io/docs/configuration/packages/) and uses yr as temp sensor but its recomended to use a local temp sensor for batter accuracy.


In the example im using 3 different starting times
- 120 min when colder then -10 degres celsius
- 60 min when colder then +1 degres celsius
- 30 min when colder then +5 degres celsius

You can edit the times and temp values to better fit your conditions and heater.

Please note that the automation that checks time/temp is started at 02:00 and you need to change that if you are leaving before 04:00 (this is because they check status every 5th min so dont want them on all day)


## Screenshot from HASS GUI
![gui_screenshot](https://github.com/Gnaget2/Car-Heater-Package/blob/master/Images/GUI_Screenshot.jpg)

## Installation
- If your installtion dont allready support the use of [packages](https://home-assistant.io/docs/configuration/packages/) please activete it.
- Place Heater.yaml in your package folder
- Edit Heater.yaml to use the sensor of your choice (or leave it as is to use the YR sensor)
- Edit Heater.yaml to use the corect switch that controls your heater (switch.motorvarmaren in the example)
