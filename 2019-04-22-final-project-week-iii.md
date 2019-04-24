---
layout: post
title: "Final Project: Week II"
date: 2019-04-16
author: Sofia von Hauske Valtierra
---

## Changes from last week

![Final 152](https://user-images.githubusercontent.com/43420227/56206626-cdd1b680-601a-11e9-9b09-c81e54bd5bdc.jpg)

I initially thought about making this out of wood, plywood specifically. Plywood is durable and has cross-graining, which reduces the tendency of wood to split, it reduces expansion and shrinkage, and it makes the strength of the panel consistent across all directions. Instead of wood, since this will be out in the open, I decided to go with plastic for the actual prototype, because it will make it more durable when subjected to bad weather.

![Final 151](https://user-images.githubusercontent.com/43420227/56206625-cdd1b680-601a-11e9-86d4-02cb9f2d73b8.jpg)

They whole device was a lot bigger than I wanted, mostly becuase of the dispensing mechanism I came up with: 

![Final 153](https://user-images.githubusercontent.com/43420227/56206627-cdd1b680-601a-11e9-8589-e2a2f4780562.jpg)

The mechanism had to change completely for me to be able to shrink the whole thing. I decided to use a servo actuator that gives linear motion through rack and pinion movement.

![b4a17783f01681ccc25858dcd89c555b_preview_featured](https://user-images.githubusercontent.com/43420227/56629985-94eaa080-661d-11e9-97a5-badc6de64a81.jpg)

These are the dimensions I started out with:

![Catapulta](https://user-images.githubusercontent.com/43420227/56206621-cdd1b680-601a-11e9-904a-80c2d79b86b4.jpg)

This first ideation required:

- Arduino
- 2 Servo motors
- 4 PIR Sensors
- 1 MP3 Shield
- 1 speaker

As I was testing out my electronic components, I discovered that having one PIR sensor on top of the device was enough and that having 4, one on each side was unnecessary. 


## This week

### Dimensions

### Renderings

### Prototype Pictures

![IMG_0474](https://user-images.githubusercontent.com/43420227/56629892-2d345580-661d-11e9-8023-923411da2ce8.jpeg)

![IMG_2194](https://user-images.githubusercontent.com/43420227/56629893-2d345580-661d-11e9-8606-b254be8868ff.jpeg)

![IMG_9380](https://user-images.githubusercontent.com/43420227/56629894-2d345580-661d-11e9-8cd1-03f483b63b46.jpeg)

### Interaction

My interaction flow stayed the same. 

![Catapulta2](https://user-images.githubusercontent.com/43420227/56206622-cdd1b680-601a-11e9-9b81-50d35ce1d7ec.jpg)

**Zookeper:** Activates the low-frequency sound through bluetooth.

**Fox:** Hears sound and tries to pin-point its location.

**Device:** Waits for movement.

**Fox:** Approaches device with either muzzle or by stamping close by.

**Device:** Detects movement, dispenses treat and launches it into the air like a flying insect.

**Fox:** Catches treat.

### Video

[![](http://img.youtube.com/vi/k6kEeGP1h3k/0.jpg)](http://www.youtube.com/watch?v=k6kEeGP1h3k "Enrichment")

### Next Steps

- I made a small measurement mistake while making the dispensing system, that needs to be redone so it works smoothly. 

- The motion sensor needs to be tuned, because it is very sensitive.

- The catapult arm needs to become longer so it launches it better, it is too short right now. 



