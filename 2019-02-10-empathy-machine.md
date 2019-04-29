---
layout: post
title: "Empathy Machine"
date: 2019-02-10
author: Sofia von Hauske Valtierra
---

## First Attempt: Researching Animals

First I started by researching animals; I started looking into interesting behaviors that they had, or exciting ways in which they sensed things. One of the things that I found really interesting and that I went a little more deeply into was Firefly communication. Fireflies have different flying and lighting patterns that lets them communicate with their species and attract females. I had a couple of ideas of physical and digital games that had to do with this, but I wasn't really convinced. Starting out with research was not really getting me to where I wanted.

![firefly](https://user-images.githubusercontent.com/43420227/52544532-6039ad80-2d7f-11e9-9998-c70df796e1ec.jpg)
- [Science Friday](https://www.sciencefriday.com/educational-resources/talk-like-a-firefly/)
- [NPS](https://www.nps.gov/grsm/learn/nature/firefly-flash-patterns.htm)

 So I decided to start by thinking about empathy. 

## Thinking About Empathy

The first thing that came to my mind when I thought of empathy was something that happened back home in Mexico while I was visiting last year. I have two dogs back home, and I always travel with my dog from here; they are all rescues, so they already a little bit afraid of things. There is a church a couple of blocks away that celebrates several saints throughout the year, and they throw this big block party that goes on until 6 AM. There are fireworks all night long, and my dogs get really scared. They start shaking like crazy, they hide under the furniture and they won't come out, and there is nothing we can do about it. This time, my mom decided to call the church. It was about 2 AM when this happened. She managed to get in contact with the priest; he was in charge of the celebration. She explained why she was calling and politely asked him to stop lighting up fireworks, to which the priest responded: "Animals are replaceable." and hung up the phone. 

This is a picture of the Church:
![3350843466_80204db618_b](https://user-images.githubusercontent.com/43420227/52544673-1d2c0a00-2d80-11e9-86c1-15d243a5237b.jpg)

From here I decided to do more research on hearing, and the effect that loud noises and noise pollution, in general, has on wildlife. 


## Hearing in Animals

As I started searching for more information on this, I kept coming across things like this:
![news](https://user-images.githubusercontent.com/43420227/52544882-9f68fe00-2d81-11e9-8205-5e219b9a1b24.jpg)

News reports are mostly about marine life and the effect of noise pollution on them, but they aren't the only ones getting affected.

## Noise Pollution

What is noise pollution? A noise is an unwanted or inappropriate sound. Noise pollution is noise that interferes with normal activities, and disrupts or diminishes our quality of life. [PBS News Hour](https://www.pbs.org/newshour/nation/noise-pollution-humans-wreaking-havoc-u-s-wildlife)

**Noise Pollution Effects:**

* **Flying Species:**
  - Changes the distribution of birds, affecting trees and plants.
  - Some bird species have demonstrated adjustments to their vocal behaviour in an attempt to adapt. 
  - Some birds species have begun to sing at night.
  
* **Land Species:**
  - Female frogs have more difficulty locating the male's signal.
  - Reduces in the size of an area in which predators can hear their prey, and the ability of animals to avoid predators.
  - High-intensity sound induces fear, sometimes forcing species to abandon their habitat.
  - It can alter their established behaviours like vigilance, foraging, resting and their social interactions.

* **Marine Species:**
  - Damage a cetacean’s hearing and interfere with their sonar navigation system, leaving them stranded.
  - Physical trauma like bleeding around the ears, brain and other tissues, and air bubbles in their organs. ("The Bends")
  - Some species have started avoiding areas that were previously breeding or feeding grounds.
  - Different species have suffered behavioural changes when communicating.
  - Cephalopods suffer damage to their statocyst, the organ responsible for their maintaining balance in the water.

- [NPS](https://www.nps.gov/subjects/sound/effects_wildlife.htm)
- [Everything Connects](http://www.everythingconnects.org/noise-pollution.html)
- [IFL Science](https://www.iflscience.com/environment/how-noise-pollution-changing-animal-behaviour/)
- [Australian Academy of Science](https://www.science.org.au/curious/earth-environment/noise-pollution-and-environment)

## Animal Pinnae

What is Pinnae? Pinnae are the external part of the ears in humans and other mammals. I decided to focus on the pinnae because I think it is something we often overlook or take for granted when we are thinking about hearing.

Some animals can swivel or rotate their pinnae in order to pinpoint where sounds are coming from. For predators, it is helpful while hunting, to find their prey, and for the animals being hunted, it helps them avoid predators.  

**Examples:**
* Foxes: Foxes can rotate pinnae up to 150 degrees.
* Canines
* Felines: Cats can rotate pinnae up to 180 degrees.
* Equines: Horses can rotate pinnae up to 180 degrees.
* Porcines
* Ungulates
* Rodents

[Signia](https://www.signiausa.com/blog/fun-facts-hearing-animal-insect-edition/)

![animals](https://user-images.githubusercontent.com/43420227/52544539-66c82500-2d7f-11e9-8a3a-cbe71294bc40.jpg)

## How can I design something that let's humans experience an animal's ability to rotate their pinna and focus on a sound?

**First Step: Interior Mechanism**

I started out by building out the mechanism I would need. I was going to use a servo motor to make the pinna rotate and since I wanted to somehow tie it back to muscle control, I decided to use a flex sensor. Bending the sensor with your finger would control the degrees of rotation of the servo.

This is what my circuit looks like:

<img width="794" alt="screen shot 2019-02-11 at 10 38 04 pm" src="https://user-images.githubusercontent.com/43420227/52610149-e6242a00-2e4d-11e9-9b9f-3170496d15e3.png">

<img width="788" alt="screen shot 2019-02-11 at 10 38 43 pm" src="https://user-images.githubusercontent.com/43420227/52610150-e8868400-2e4d-11e9-8438-842531810af3.png">

**Second Step: Code**

```C++
// Servo library

#include <Servo.h> 

Servo servo1;

const int flexpin = 0; 

void setup() 
{ 

  Serial.begin(9600);

  servo1.attach(7);
} 

void loop() 
{ 
  int flexposition;  
  int servoposition;   

  flexposition = analogRead(flexpin);

  servoposition = map(flexposition, 100, 300, 0, 180);
  servoposition = constrain(servoposition, 0, 180);


  servo1.write(servoposition);

  //Serial.print("sensor: ");
  //Serial.print(flexposition);
  //Serial.print("  servo: ");
  //Serial.println(servoposition);

  delay(20); 
}
```

**Third Step: Exterior**

Sketches:

![untitled_artwork 2](https://user-images.githubusercontent.com/43420227/52610671-14a30480-2e50-11e9-8f90-c3706c6ce121.jpg)

![untitled_artwork](https://user-images.githubusercontent.com/43420227/52610678-17055e80-2e50-11e9-8cab-8cba97c61849.jpg)

3D Model:

![ear1](https://user-images.githubusercontent.com/43420227/52611345-381b7e80-2e53-11e9-9f50-0bd5ce787e3e.JPG)

![ear2](https://user-images.githubusercontent.com/43420227/52611346-381b7e80-2e53-11e9-8069-de30ddbe957f.JPG)

Technical Drawings:

![ear_techd](https://user-images.githubusercontent.com/43420227/52611405-75800c00-2e53-11e9-8b79-36b108cd4285.jpg)

**Fourth Step: Testing**

<img width="1440" alt="screen shot 2019-02-11 at 11 56 25 pm" src="https://user-images.githubusercontent.com/43420227/52612712-e118a800-2e58-11e9-9c96-f67348bf6a76.png">

<img width="1440" alt="screen shot 2019-02-11 at 11 56 58 pm" src="https://user-images.githubusercontent.com/43420227/52612713-e118a800-2e58-11e9-90fc-0d0424864f61.png">

<img width="1440" alt="screen shot 2019-02-11 at 11 57 32 pm" src="https://user-images.githubusercontent.com/43420227/52612715-e118a800-2e58-11e9-8c8b-fbd90628cf78.png">


[Empathy Machine Video](https://vimeo.com/316803913)
 
[!["screen shot 2019-02-12 at 9 55 46 am" src="https://user-images.githubusercontent.com/43420227/52644314-94f75300-2eac-11e9-87b3-b52ed9e94ac9.png"](http://img.youtube.com/vi/BB0bYADjauI/0.jpg)](http://www.youtube.com/watch?v=BB0bYADjauI "Empathy Machine")

**Results:**

People found this fun and interesting. They really liked being able to control it with their finger. It did make them realize how hard it is to focus and pinpoint a sound in general, but even more when several things were happening around them.In terms of the volume, they could hear a slight change when rotating the ear towards a sound, but the motor and friction produced too much noise.

Ideally, this would be made out of nylon or with bearings to reduce friction and noise. The ear pinna is modeled after a small sized red fox ear, but maybe testing out larger sizes would make the effect greater.

[Go to main page.](https://svonhauske.github.io/Interaction-Design-in-The-Wild)
