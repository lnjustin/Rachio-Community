# Rachio-Community
Community version of Rachio App/Drivers for Hubitat

Rachio Community builds off of the native Rachio integration. On top of the native features, this community version adds:
* Dashboard. See your watering schedule and skips, in conjunction with Rachio weather information, on your smart home dashboard. Substantially similar to what you see on the Home tab of the mobile app, except Rachio Community enhances it to include different icons for different types of skips. Highly configurable.
* Next Run and Last Run data exposed for automation & display. Automate based on when your next run will occur and/or when your last run occurred.
* Rain Sensor State exposed. Use your irrigation system's rain sensor for automation and/or see its status on your smart home dashboard.
* Next event data exposed. See information about your system's next event, e.g., scheduled run or skip.
* Monthly watering summary exposed. See the same monthly watering summary as on the Home tab of the mobile app.

Filled Icon Pack
![image](https://user-images.githubusercontent.com/12822477/118013431-1ce49580-b320-11eb-824d-a81a2a92e31d.png)

Outline Icon Pack
![image](https://user-images.githubusercontent.com/12822477/118013465-266dfd80-b320-11eb-9fe6-bc0c002f0dec.png)

## Icon Key:
![image](https://user-images.githubusercontent.com/12822477/118013482-2b32b180-b320-11eb-8849-fd853cc4dea2.png) Watering

![image](https://user-images.githubusercontent.com/12822477/118013502-2f5ecf00-b320-11eb-9d02-e8545fddd681.png) Rain Skip due to predicted rain

![image](https://user-images.githubusercontent.com/12822477/118013513-32f25600-b320-11eb-81ea-1dd865a4b10c.png) Soil saturated skip

![image](https://user-images.githubusercontent.com/12822477/118013550-3a196400-b320-11eb-8e1a-de0b26ed85d6.png) Wind skip

![image](https://user-images.githubusercontent.com/12822477/118013559-3c7bbe00-b320-11eb-8db4-598ad790d59c.png) Freeze skip

![image](https://user-images.githubusercontent.com/12822477/118013569-3f76ae80-b320-11eb-9bd8-eb367fd005ae.png) Rain Sensor skip
(Tentative skip if rain sensor remains triggered)

![image](https://user-images.githubusercontent.com/12822477/118013586-42719f00-b320-11eb-8ccc-91466a841cc3.png) Manual Skip

**Dashboard Output Format**
The Dashboard outputs an SVG image to a local endpoint as well as a cloud endpoint, so you can embed the resulting image into any image tile of any dashboard, e.g., Sharptools dashboard, Smartly, etc. Note that you would want to embed the image into a dashboard image tile with a dark background if you select a white color scheme, and embed the image into a dashboard image tile with a light background if you select a black color scheme.

**Dashboard Configuration**
The dashboard is highly configurable with regard to:
* Number of days on dashboard
* Hide/Show precipitation percentage, precipitation amount, high/low temp
* Select from predefined color schemes or customize every color
* Expand or Collapse vertical or horizontal spacing
* scale up or down in size

**Uses undocumented Rachio API**
Note that Rachio Community relies on an undocumented API to extend the native Rachio functionality. Rachio has stated in its community forum that, although use of the undocumented API is allowed, there is no guarantee about its availability, meaning it could change without notice at any time. Accordingly, the expanded functionality in Rachio Community cannot be guaranteed. This especially since *this community version of the app and drivers has been developed by the Hubitat community, without any affiliation or cooperation with Rachio.*

**Supported Controllers**
Rachio controllers 1, 2, 3, and 3e are supported.


**Hubitat Package Manager Install Instructions**
1. Uninstall the Rachio native app
2. Install Rachio Community Package via Hubitat Package Manager
6. Follow the install instructions in the Rachio Community app

**Manual Install Instructions**
1. Uninstall the Rachio native app
2. Install the Rachio Zone driver
3. Install the Rachio Controller driver
4. Install the Rachio Community app
5. Enable Oath
6. Follow the install instructions in the Rachio Community app

