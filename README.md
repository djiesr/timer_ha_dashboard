# Create à Timer on your dashboard
Copy the timer_entity.yaml file with your other package file.

If you didn't configure packages file before, follow these steps:

Add these lines in your configuration.yaml. If you already have a line "homeassistant:", just copy the "packages" line.
homeassistant:
  packages: !include_dir_named packages/

Create the "packages" folder in your "config" folder in Home Assistant.
Download or copy the hq_open_data.yaml file in your "HA"/config/packages/ folder.
Reboot HA

# Set the package for your entity

# Add the dashboard

To add the dashboard copy the content of the dashboard yaml file in a empty ("manual") card. There no other option to see the live countdown.

# Dashboard 

For the dashboard.yaml, just copy the content of the file in a empty card. it's can be hard to set the time with the tiny default slider.

![image](https://user-images.githubusercontent.com/31359825/218279715-9d760285-e79a-4b25-8a46-cf1224ab9b91.png)
![image](https://user-images.githubusercontent.com/31359825/218279761-6bc61093-8318-4b82-9f45-b01a5761827a.png)

# Dashboard extra

For the Dashboard extra, you need to install 2 extra feature from Hacs/Interface.
- slider-entity-row: https://github.com/thomasloven/lovelace-slider-entity-row
- Mushroom : https://github.com/piitaya/lovelace-mushroom

After instill these 2  extra, you can paste the "dashboard_extra.yaml" content in a empty card of your dashboard for this result.

![image](https://user-images.githubusercontent.com/31359825/218279735-50206f8b-a52d-4f25-aa52-6dfcb27b269b.png)
![image](https://user-images.githubusercontent.com/31359825/218279774-6e0be5d7-dcc3-45cc-850c-6968e9632077.png)
