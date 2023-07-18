---
layout: post
title: "Empathy Machine"
date: 2019-02-10
author: Sofia von Hauske Valtierra
---

# Creating an Empathy Machine:

## First Attempt: Researching Animals

I began my journey by studying animals and their interesting behaviors and sensory abilities. One particular area that caught my attention was Firefly communication. I was fascinated by the various flying and lighting patterns these creatures use to communicate with their own species and attract mates.

I explored different possibilities for incorporating this concept into physical and digital games. However, none of the ideas I came up with felt quite right. Despite conducting extensive research, I realized that I had not yet reached the desired outcome.

![firefly](https://user-images.githubusercontent.com/43420227/52544532-6039ad80-2d7f-11e9-9998-c70df796e1ec.jpg)
- [Science Friday](https://www.sciencefriday.com/educational-resources/talk-like-a-firefly/)
- [NPS](https://www.nps.gov/grsm/learn/nature/firefly-flash-patterns.htm)

 So I decided to start by thinking about empathy. 

## Thinking About Empathy

When I think about empathy, I immediately recall something that happened back home in Mexico last year. I have two dogs, and whenever I visit, I bring one of them along. They're both rescues, so they tend to be a bit skittish.

There's this church a few blocks away that throws these massive block parties to celebrate different saints throughout the year. The parties go on all night, and fireworks are a big part of the celebration. The problem is, my dogs get really scared of the loud noises. They start shaking like crazy, hiding under furniture, and they won't budge. It's tough to see them so terrified, and we feel helpless in those situations.

During my last visit, around 2 AM, my mom took matters into her own hands. She decided to call the church and talk to the priest in charge of the celebration. She explained why she was calling and politely asked him to stop lighting up fireworks, to which the priest responded: "Animals are replaceable." and hung up the phone. 

This is a picture of the Church:
![3350843466_80204db618_b](https://user-images.githubusercontent.com/43420227/52544673-1d2c0a00-2d80-11e9-86c1-15d243a5237b.jpg)

After that incident, it sparked my curiosity to dig deeper into the subject of hearing and how loud noises, like noise pollution, affect wildlife. I wanted to learn more and get a better grasp of the broader impact these things can have.

So, I started doing some research, delving into the connection between animals and sound. I wanted to understand how those loud noises can mess with their habitats, communication, and overall happiness. It became my mission to uncover the effects of noise pollution on wildlife and really get to the bottom of it.


## Hearing in Animals

As I started searching for more information on this, I kept coming across things like this:
![news](https://user-images.githubusercontent.com/43420227/52544882-9f68fe00-2d81-11e9-8205-5e219b9a1b24.jpg)


News reports tend to focus heavily on marine life and how noise pollution impacts them, but it's essential to remember that they're not the only ones facing the consequences.

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

Here's the interesting part: some animals can actually move their pinnae. They can rotate or swivel them around to figure out where sounds are coming from. It's like having a built-in sound detector! This skill is super useful for predators when they're hunting because it helps them locate their prey accurately. And for animals that are being hunted, it's a survival tool that helps them detect and avoid potential predators.

So, pinnae may seem like just an ordinary part of our ears, but they play a vital role in helping animals hear and survive in their environments.

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

I decided to use a servo motor as the core component to achieve the pinna rotation. The servo motor would be responsible for moving the pinna-like structure. In order to make the rotation feel more interactive and connected to the user's body, I incorporated a flex sensor into the design. This sensor detects the bending motion and translates it into degrees of rotation for the servo motor.

By bending the flex sensor with your finger, you would be able to control the extent of rotation of the pinna-like structure through the servo motor. This would simulate the experience of having control over the direction and focus of the sound, similar to how animals with rotating pinnae can adjust their hearing.

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
 
[![](http://img.youtube.com/vi/BB0bYADjauI/0.jpg)](http://www.youtube.com/watch?v=BB0bYADjauI "")


[Go to main page.](https://svonhauske.github.io/Interaction-Design-in-The-Wild)
