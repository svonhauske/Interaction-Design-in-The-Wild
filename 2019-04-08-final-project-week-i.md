---
layout: post
title: "Final Project: Week I"
date: 2019-04-08
author: Sofia von Hauske Valtierra
---


## Final

I started out by choosing my 1st proposal; the preybot that imitated a flying bird or a running squirrel, so the first thing I wanted to solve was how to hang kibble from it. I did some research on edible materials that could encapsulate the kibble and that the fox could eat as well, instead of trying to create some sort of container. After looking at several possibilities, I decided to try gelatine. 

This is how it turned out:

![IMG_3559](https://user-images.githubusercontent.com/43420227/55801329-d3238400-5aa3-11e9-8bf5-df4dddc22532.jpeg)

![IMG_7099](https://user-images.githubusercontent.com/43420227/55801330-d3238400-5aa3-11e9-819a-4e87df1e3d2b.jpeg)


After this, I wanted to tackle my second most significant challenge; finding a strong enough motor. I did some research, found a couple of different options, but with each one, new problem arrised. Due to time constraints and the fact that I do not have that much experience with motors, I decided to move on from my 1st proposal, and start working on my 3rd proposal. 

### 3rd Proposal:

My third proposal is inspired by the way in which foxes hunt insects. Foxes are able to detect very low frequencies, which is how they are able to detect insects. When the insect is hiding, foxes will use their muzzle to poke around, or they do something called foot stamping. The foot stomping causes insects to try to flee, and then the fox is able to locate them  better by the sound of rustling or movement. This is the behavior that I want to generate with my prototype. 

This is the drawing that I started out with:

![Idea3](https://user-images.githubusercontent.com/43420227/55293858-fe81e100-53c8-11e9-9a48-7ead562cd174.jpg)

The idea is that this box can be placed anywhere in their zoo habitats, hidden from sight. A very low frequency is played to catch the foxes attention, and then it has to approach it and try to pinpoint its exact location by either poking around with their muzzle or foot stamping. If they do it close enough to where the box is, the motion sensor will detect it and launch a treat slightly above the ground, just like an insect flying away, so the fox can catch it and eat it. Two things add variability to this prototype, the fact that it is movable, so it doesn't always have to be in the same spot, but also the buzzing could be activated through Bluetooth, so it does not have to occur at the same time every time. 

Parts:

- Launching mechanism
- Low Frequency Sound
- Treat/Kibble Container
- Motion Sensors

I started out by building the buzzing,the launching mechanism, and the motion detection. Right now ther buzzer gets activated through a button, but for my next iteration, it will be through a phone using bluetooth. The launching mechanism gets activated when the motion sensor is approached and it catapults something into the air. 

[![](http://img.youtube.com/vi/OQnEQBiAwJ0/0.jpg)](http://www.youtube.com/watch?v=OQnEQBiAwJ0 "Week I")

Next Steps:

- Create a container similar to a gumball machine so it doesn't have to be reloaded everytime, it does it automatically.
- Build an automated door for the container, so the kibble or treat only comes out when the buzzer gets activated.
- Connect arduino to phone through bluetooth.
- Test out speaker insted of buzzer. 
- Build external container. 
