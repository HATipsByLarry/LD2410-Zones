# LD2410-Zones
How to set zones in Home Assistant with the LD2410 Series of mmWave Sensors

I often have people ask me how to set the zones up for the LD2410 series of mmWave presence sensors. Here are the steps i came up with to do that.

Step 1: Measure the distance from the sensor to where you want zone 1 to end. Also do the same for zone 2 and zone 3.

Step 2: In Home Assistant go to the sensors configuration page and scroll down until you find the configurations you see below.

![ld2410c zones distance](https://github.com/HATipsByLarry/LD2410-Zones/assets/49766850/eabc0fe5-1bcf-41be-8ef1-5da76bb94bcb)

Step 3: In the Radar End Zone 1 box type in the measurement you made for zone 1. This is in centimeters so if you measured in inches convert the measure first.

Step 4: Repeat step 3 for zone 2 and zone 3.

Step 5: Adjust the Radar max Move and Radar max Still distances to match the end of zone 3 or where ever you want the detection to end. Keep in mind that this measurement is in meters so again convert your measurements to meters. The max is 8 meters.

Step 6: repeat steps 1 through 5 for your other sensors.

Your automations can trigger based on what zone the person is in

![automation zones](https://github.com/HATipsByLarry/LD2410-Zones/assets/49766850/06d82486-14e8-41c8-b874-3062a86c064c)

Thus if a light fixture is in zone 1 for example you can trigger the light to come on when someone is in that zone then trigger it to go off when they leave that zone.

![automation zones 2](https://github.com/HATipsByLarry/LD2410-Zones/assets/49766850/d2acf62f-b562-41b7-804a-d5e300043433)

Code For the LD2410C with zones https://github.com/HATipsByLarry/LD2410-Zones/blob/main/LD2410%20Code.yaml

If anyone has questions about this then please ask them on my youtube channel here: https://www.youtube.com/watch?v=YNEQxj-JnEs

Also on my discord channel here: https://discord.com/invite/9EkA5rFyCE

Found This Useful and want to say thanks
___ ☕ Buy Me A Coffee! ☕ __ 
https://www.buymeacoffee.com/hatipsbylarry
