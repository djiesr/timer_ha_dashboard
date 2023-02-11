# Create à Timer on your dashboard
Copy the timer_entity.yaml file with your other package file.

If you didn't configure packages file before, follow these steps:

1. Add these lines in your configuration.yaml. If you already have a line "homeassistant:", just copy the "packages" line.

> homeassistant: <BR>
> &nbsp;&nbsp;packages: !include_dir_named packages/

2. Create the "packages" folder in your "config" folder in Home Assistant.
3. Download or copy the timer_entity.yaml file in your "HA"/config/packages/ folder.
4. Reboot HA

# Set the package for your entity
For this package, you must replace "switch.cuisine" with the ID of the device you want to control.
Example: "switch.cuisine" can become "switch.car_charger"

To modify the names and aliases, you can replace "Prise cuisine" and "prise_cuisine" with what you want, but if you modify them, you must change them all, unless you know exactly what you're doing.
Example for the alias: "Prise cuisine Auto Off" can become "Car charger Auto Off"
Example for the name: "timer.prise_cuisine_minuteur" can become "timer.car_charger_timer"

You can set the minimum and maximum time for the timer with:
>    min: 10 # Set the minimum time for the slider <br>
>    max: 600 # Set the maximum time for the slider

Note that you can add aliases in Home assistant without changing those in this package.

In the script for notifications, you can add your mobile and Alexa. For Google, you can add a temporary text-to-speech to work around the SDK problems.

# Add the dashboard

To add the dashboard copy the content of the dashboard yaml file in a empty ("manual") card. There no other option to see the live countdown.

# Dashboard 

For the dashboard.yaml, just copy the content of the file in a empty card. It's can be hard to set the time with the tiny default slider.

![image](https://user-images.githubusercontent.com/31359825/218279715-9d760285-e79a-4b25-8a46-cf1224ab9b91.png)
![image](https://user-images.githubusercontent.com/31359825/218279761-6bc61093-8318-4b82-9f45-b01a5761827a.png)

# Dashboard extra

For the Dashboard extra, you need to install 2 extra feature from Hacs/Interface.
- slider-entity-row: https://github.com/thomasloven/lovelace-slider-entity-row
- Mushroom : https://github.com/piitaya/lovelace-mushroom

After instill these 2  extra, you can paste the "dashboard_extra.yaml" content in a empty card of your dashboard for this result.

![image](https://user-images.githubusercontent.com/31359825/218279735-50206f8b-a52d-4f25-aa52-6dfcb27b269b.png)
![image](https://user-images.githubusercontent.com/31359825/218279774-6e0be5d7-dcc3-45cc-850c-6968e9632077.png)
