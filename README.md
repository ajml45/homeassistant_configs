## Light Control Info
Main light control dynamically controls all of the lights in the house via <a href="https://github.com/fredck/lightener">Lightener</a>.  Each room of the house has it's own light via Lightner that controls all of the lights in that room.  The main light control is made of up each of those room lights.

Light scripting: 
- 45 min before dusk the lights in the majority of the rooms transition to 45% (as long as they are currently off) over a 5 minute period.  This uses the built in Home Assistant service calls, <a href="https://everythingsmarthome.co.uk/creating-wake-up-sunrise-lights-with-home-assistant/">more details here.</a>
- Beginning at 6:30pm for the majority of rooms (some are later for example the Solarium doesnt start until 830pm), the lights gradually fade from their current brightness down to dim levels (generally 15-0% based on the room.)  This is done via <a href="https://community.home-assistant.io/t/ashley-s-light-fader-2-0-fade-lights-and-or-color-temperature-with-your-choice-of-easing-curves-including-ease-in-ease-out-and-ease-in-out/584077">Ashley's fader script."
- The code for this is set-up in Lightener for the lights and the scripts.yaml file for the logic.  

## Tablet Dashboard
<img src="https://github.com/ajml45/ha-configs/assets/122765092/d5c67be4-170e-499f-aa8c-a1a27f3dd94d" width="500"> </br>
Home Page, dashboard uses sidecard card for the side menu.  

<img src="https://github.com/ajml45/ha-configs/assets/122765092/e1b6f14f-532f-419e-8109-56ed3253760b" width="500"> </br>
Music/Sonos Card

<img src="https://github.com/ajml45/ha-configs/assets/122765092/2b68434e-b689-4078-93c4-4188f4f3c691" width="500"> </br>
 Main room controls. Room cards have conditional icons that display when active. Tapping a room card opens a pop-up via <a href="https://github.com/Clooos/Bubble-Card">Bubble Card</a> with all of the room controls (examples below.) Double tapping opens the main light contol for that room. Holding a room card shuts off all lights in that room.

<img src="https://github.com/ajml45/ha-configs/assets/122765092/ea3eb9be-a493-4e72-b9ca-f26e8d7c868c" width="500"> </br>
Camera card for Arlo, needs work... Have to add reolink doorbell.

<img src="https://github.com/ajml45/ha-configs/assets/122765092/534f61a0-7b92-40ef-bac6-faf6d87a8441" width="500"> </br>
Mail card from Mail and Packages, acts as a pop-up via Bubble Card.

<img src="https://github.com/ajml45/ha-configs/assets/122765092/ee1cc789-181e-45f0-8679-b91482676fe8" width="500"> </br>
Weather info

<img src="https://github.com/ajml45/ha-configs/assets/122765092/703993a1-9555-497d-a915-1a9fe030c5ea" width="500"> </br>
To-Do Lists

<img src="https://github.com/ajml45/ha-configs/assets/122765092/9da5cdb8-da6e-4e89-a396-56f0b8037c25" width="500"> </br>
Room Pop-Up Example: Great Room

<img src="https://github.com/ajml45/ha-configs/assets/122765092/7a4305f1-3135-4903-8b0a-281e03d48b11" width="500"> </br>
Room Pop-Up Example: Solarium

<img src="https://github.com/ajml45/ha-configs/assets/122765092/d22be89d-6d6f-49ca-8ec4-56a7a2c0dc30" width="500"> </br>
Room Pop-Up Example: Mudroom

<img src="https://github.com/ajml45/ha-configs/assets/122765092/19dec992-46a0-4c31-b74a-d2ed1cd28f5a" width="500"> </br>
Settings etc


## Mobile Dashboard
Uses bubble card heavily - for the home page room controls as well as the individual room pop-up cards and bottom navigation.  The room buttons on the home page are a light slider that toggle the lights for that room.  Clicking the icon brings up the room pop-up with the individual controls.  Double clicking the icon brings up the main room light and holding the icon shuts all of the lights off in that room.

<img src="https://github.com/ajml45/ha-configs/assets/122765092/eea6fea4-d917-4b66-a4a1-58cbdf339392" width="300" alt="Home Page">
<img src="https://github.com/ajml45/ha-configs/assets/122765092/4e3d47a7-b60a-4690-b86e-d69e5a591921" width="300" alt="Solarium">
<img src="https://github.com/ajml45/ha-configs/assets/122765092/5defc921-ba57-4fe8-a2a7-3f590aee4dd1" width="300" alt="Basement">
<img src="https://github.com/ajml45/ha-configs/assets/122765092/5fc31eaf-639d-4e6e-8e37-e92a4d505b96" width="300" alt="Sonos">
<img src="https://github.com/ajml45/ha-configs/assets/122765092/0d490660-94c8-464b-acca-631ccd021619" width="300" alt="Calendar">
<img src="https://github.com/ajml45/ha-configs/assets/122765092/ceb21037-a235-4212-83b2-5dd18f167808" width="300" alt="Weather">
<img src="https://github.com/ajml45/ha-configs/assets/122765092/29055f91-ec93-4bd4-a129-ae3b0938323f" width="300" alt="Family">
<img src="https://github.com/ajml45/ha-configs/assets/122765092/9629c7a2-b483-440d-b955-856520c3f97b" width="300" alt="IT">


## HACS Integrations:
- <a href="https://github.com/fredck/lightener">Lightener (used heavily for main light and room lights)</a>
- Mail and Packages (mail)
- iCloud3 Device Tracker (waze distances)
- SmartThinQ LGE Sensors (washer/dryer)
- Frigate (camera playback)
- Alexa Media Player (alexa integration)
- WebRTC Camera (camera playback)
- HACS
- Arlo Camera Support (cameras)
- Govee (light brand integration)
- Rollease Acmeda Autom Pulse Hub v2 (shade integration)


## HACS Frontend
- <a href="https://github.com/Clooos/Bubble-Card">Bubble Card (used heavily, for menus and pop-ups)</a>
- slider-entity-row
- Hourly Weather Card
- Stack In Card
- Sonos Card
- Clock Weather Card
- Lovelace Hass Aarlo
- mini-graph-card
- Big Slider Card
- Vacuum Card
- card-mod
- Horizon Card
- Mushroom
- layout-card
- Weather Radar Card
- Frigate Card
- Slider Button Card
- Atomic Calendar Revive
- fold-entity-row
- vertical stack in card
- Custom Brand Icons
- button-card
- Mail and Packages Custom Card
- Sidebar Card (Tablet side bar)
- Battery Entity Row
- apexcharts-card


## Integrations
<img src="https://github.com/ajml45/ha-configs/assets/122765092/6cf310fa-3852-495f-92de-29734f0242e9" width="800">

## Add-Ons
<img src="https://github.com/ajml45/ha-configs/assets/122765092/b012dab9-04e9-4d82-9781-0fc4406a34d0" width="800">
