# Viene

Viene is a robotic living wall that reflects the changing seasons, set to Vivaldi's _The Four Seasons_.

## Team
Victor Wang, Rebecca Abraham, Tina Ye, Dipika Khullar, Matthew Bronars

## Summary

The wall cycles through the four seasons of the year along with a soundtrack consisting of segments from Vivaldi's concertis to enhance the mood of each season. Moving vines suspended along a beam and spinning flowers powered by DC motors allow for movement as the seasons pass, simulating growth and wind. Strings of neopixels are embedded along each vine allow for changing colors and patterns according to the season that the wall is experiencing. This project aims to mimick the events of nature through programming and electronics. 


## Component Parts

* 8 plastic vines
* 6 servos
* Painted canvas backing
* 60 neopixels
* Electronic components
* Adafruit feather
* Power supply


Include what types of inputs/outputs/data it will use, and a block diagram showing how all those pieces are connected.

## Challenges

### Simulating Vine Growth
We initially experimented and mentally prototyped various pulley-based mechanical systems of retracting and lengthening our plastic vines. These included ideas such as using a timing belt that wrapped from the bottom to the top. Another idea included usinga high friction surface. Another idea was to use a system of strings. Between the limited range of the servos and the lack of precision of the DC motors, this proved to be too difficult for the limited amount of time allocated for this project. Our alternative was to simulate movement by sequentially lighting up or turning off the LEDs. Since we already had to infrastructure in place to do this, it was easy to implement vie growth in software instead of adding more hardware.

### Power Distribution
We had a lot trouble getting the power distribution for our project to work. Since our project included a large number of electronic components such as 60 neopixels which in total drew about 1.5A at peak and 8 servos which draw about .5A at peak. We initially had all of our compoenents plugged in to a single rail of the breadboard which resulted in uncontrollable servo movement. We spent a long time trying to diagnose the cause and saw that removing the power load by removing some servos from the power rail allowed the servos to be controlled again. We were extremely confused as to why this was happening as the power supply reported constant 5V voltage and nominal current. We eventually checked the voltage at the source of the breadboard power rails where we saw a large voltage drop of under 3V which explained the cause of the uncontrollable servos. Upon further diagnosis, we attempted to increase the voltage at the source power supply to try to acheive 5V at the breadboard rails by pushing almost 9V and 6A before the source wire from the power supply to the breadboard started smoking and we were forced to shut everything off. Upon further diagnosis, we found that the thin wires from the power supply and the breadboard supply rails caused a large amount of heat to build inside the wires and the resistance started to skyrocket as the wires became extremely hot which led to a voltage drop at the rails when the wires became a voltage divider. This issue was resolved after braiding multiple source wires together to distribute power evenly accross the rails by increasing the guage/insulation of the wire.

## Timeline

- Week 1: Wrote proposal
- Week 2: Purchased materials, planned out design
- Week 3: Assembled hardware
- Week 4: Tested components, wrote code
- Week 5: Showcase

## Completed Work

[Final Video](https://www.youtube.com/watch?v=HiZiRdkXOhQ)

## References and links
[Final Showcase Document](./Viene Poster.pdf)

### Resources
[Adafruit Feather Documentation](https://learn.adafruit.com/adafruit-feather-32u4-bluefruit-le/overview)  
[NeoPixel Uberguide](https://learn.adafruit.com/adafruit-neopixel-uberguide/the-magic-of-neopixels)
