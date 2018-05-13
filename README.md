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
We initially experimented with various pulley-based mechanical systems of retracting and lengthening our plastic vines. Between the limited range of the servos and the lack of precision of the DC motors, this proved to be too difficult for the time period. Our alternative was to simulate movement by sequentially lighting up or turning off the LEDs. Since we already had to infrastructure in place to do this, it was easy to implement vie growth in software instead of adding more hardware.

### Power Distribution

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
