---
layout: post
title: "Fox Enrichment Proposal II"
date: 2019-02-21
author: Sofia von Hauske Valtierra
---

## Preybot
02/21/2019

Based on the feedback, I have decided to move forward with my second enrichment proposal. My proposal is a preybot that mimics the behavior of a fox's arboreal prey, which consists of birds and tree squirrels. These animals have high visual acuity, and they flee upwards, which makes it really hard for foxes to catch them. They have a specific technique for hunting this type of prey: They see one on the ground, they crouch until their belly is touching the ground, and remain completely still with its ears alert. They start stalking the prey, they get closet and go into a trot, then into a gallop, and then finally they charge, trying to bite the animal. The most crucial part of this hunting technique is minimizing visual cues.

I want to build a device that hangs from the top mesh of the fox's habitat. Using a motor and fishing wire, the device can move food up and down. The idea is to lower food to the ground, catching the foxes eye by making it seem attainable. At the bottom of the wire, right above the food, a motion sensor will be "standing guard," if it senses the fox, it sends a signal to the Arduino and the motor gets activated, reeling the food back up. The fox has to apply his arboreal prey hunting technique to be able to get past the sensor and bite the food.

**Things to consider:**

- Size of the spool: Apart from taking into consideration the speed and amount of torque that I need in the motor, the size of the spool also plays a significant role when it comes to the speed of the reeling. The wider the spool, the faster the food can move up and down. 

- Type of sensor: Infrared sensors work better with light, but foxes do not only hunt during the day. An ultrasonic sensor makes more sense because it would make the preybot functional at all times. 

- Hanging Structure: Different zoos and rescue habitats have different meshes to contain the foxes, so creating a hook might limit the number of places it can be used. I want to create two small arms that you can slide onto square wooden dowels or metal extrusions so that the machine can hang from any mesh.

- Wire vs. Fixed Structure: Because of how this is designed, this device will behave like a pendulum, so the sensor won't always be looking to the same direction, but I think it will help create more of a challenge. In *Feeding enrichment in an opportunistic carnivore: The red fox*, they found that unpredictability in the presentation of food has a stimulating effect on the foxes’ behavior, so the unpredictability of the direction of the sensor should be a good thing. Also, in terms of mimicking nature, it makes sense not to have the sensor fixed because the prey's eyes are never fixed either. 

- Food Container: I had initially thought of hanging a tray that would contain the food, but because of the way in which these animals are hunted, I do not believe this is the right direction. I think the food should hang more freely, without being contained in something that is not edible, that way then the foxes charge and try to bite it, it happens more naturally than them trying to get it off the tray. I am thinking of a hook, something soft in case the fox bites into it, but sturdy enough to hang food from it.

![untitled](https://user-images.githubusercontent.com/43420227/53209747-7827f180-3609-11e9-9007-046051caa2e0.JPG)

[Go to main page.](https://svonhauske.github.io/Design-in-Safaris-19/)
