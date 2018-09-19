# XTV Football Graphics

## Prerequisites
 - Node.js (tested with version 4)
 - CasparCG Server (tested with 2.0.7)
 - CasparCG Client to load the templates (tested with 2.0.7)
 - Tested with a Blackmagic Decklink HD Extreme 3D+  for SDI Key & Fill Out

## Install Control
- Inside the graphics-control folder:
- `npm install`
- `bower install`

## Run Control
- `gulp`

## Set Up Caspar Templates
- Copy the `html-templates` folder into your CasparCG Server templates directory
- Load all the templates in Caspar using the CasparCG client on separate video layers on the correct channel and 'play' them.

# Use Control
http://localhost:3000 (or the IP of the machine you have the controls running on)

# Data Storage
- Data is stored in /graphics-control/data/db.json
- Preset-Data is stored /graphics-control/server/data/ltPresets.js

# Operation

## Control
### Team Settings
![Screenshot](/screenshots/team_settings.png?raw=true)

Set Name, Colour, Short name and players.
Settings are applied immediately to the template.

The 'Picture URI' is currently not being used by any of the templates. Future development could see it integrated into the lower thirds, or additional templates for a teamsheet with photos or similar.git p

### Player Control
![Screenshot](/screenshots/main_control.png?raw=true)

All relevant match controls to show relevant lower thirds.
'Goal' also updates the Score.

### Substitution Modal
![Screenshot](/screenshots/substitute_modal.png?raw=true)

Select an inactive player to substitute with.

### Manual and Time Control
![Screenshot](/screenshots/manual_control.png?raw=true)

Set clock, stoppage time and adjust the score.


## Look
### Main Clock and Score
![Screenshot](/screenshots/full_clock.png?raw=true)

Score and clock, including over time and stoppage time, on display.

### Yellow Card
![Screenshot](/screenshots/yellow_card.png?raw=true)

Yellow Card lower third.
By default all lower thids are displayed for 5 seconds, and are animated with animoJS animations.
