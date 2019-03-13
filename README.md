# Design in Safaris 
### by Sofia von Hauske Valtierra
---
1. [Designing for Humans](https://svonhauske.github.io/Design-in-Safaris-19/2019-01-28-designing-for-humans)

1. [Ethograms](https://svonhauske.github.io/Design-in-Safaris-19/2019-02-03-ethograms)

1. [Empathy Machine](https://svonhauske.github.io/Design-in-Safaris-19/2019-02-10-empathy-machine)

1. [Fox Enrichment Proposal I](#fox-enrichment-proposal-i)

1. [Fox Enrichment Proposal II](#fox-enrichment-proposal-ii)

1. [Fox Enrichment Prototype](#fox-enrichment-prototype)

1. [Central Park Zoo](#zoo-visit)

1. [Boris & Horton Cafe](#pet-store-visit)

1. [Group Enrichment Proposal](#group-enrichment-proposal)

1. [Hyena Enrichment Prototype]
--- 

## Enrichment Proposal II
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

[Go to top.](#design-in-safaris)

--- 

## Fox Enrichment Prototype
02/26/2019

This machine is a preybot that tries to mimic the fleeing upward behavior of a fox's arboreal prey. These type of prey consists of birds and tree squirrels, which have high visual acuity. The idea with this machine is to encourage hunting behaviors in foxes. The device lowers food to the ground, making it seem attractive, like a bird or squirrel that is on the ground in a vulnerable position. The machine has a motion sensor that can detect when the fox is getting close, just like a bird can detect it with their eyes. When hunting this type of prey, foxes stalk their prey in a deeply crouched posture and then try to catch the animal in a dashing run. The fox needs to practice this technique to be able to avoid the motion sensor, and it has to be fast enough to catch the food before that happens. If the motion sensor senses the fox, it'll automatically pull the food up, like a bird fleeing upwards. 

![img_1484](https://user-images.githubusercontent.com/43420227/53420046-07862980-39a9-11e9-80ad-2e301a555372.jpg)

[![](http://img.youtube.com/vi/WYKcjypKHa4/0.jpg)](http://www.youtube.com/watch?v=WYKcjypKHa4 "Bodystorming")

[Bodystorming Video](https://vimeo.com/319504079)

[Go to top.](#design-in-safaris)

--- 

## Pet Store Visit
## Boris & Horton Cafe
03/04/2019

Boris & Horton opened its doors for the first time in the summer of 2018. The idea was to have a place where you could have great coffee, eat, have wine and beer, hang out, but most importantly, bring your dog inside. For this to happen, the space had to be formally divided into two distinct spaces: a café side, with food and drink sales, and a dog side, featuring tables and dog-centric store. There is an outdoor window where you can order your drink or food and then walk into the dog side. 

![bh_colorlogo_transparent_800x800_5b98fe56-24d9-4d12-88fd-9885685d293f_280x 2x](https://user-images.githubusercontent.com/43420227/53781624-8d3d3400-3ed7-11e9-9be3-23225172f05c.png)

![mg_3326_2_1200x](https://user-images.githubusercontent.com/43420227/53781668-b6f65b00-3ed7-11e9-96a8-deaf583a6628.jpg)

![boris_and_horton_cover](https://user-images.githubusercontent.com/43420227/53781625-8dd5ca80-3ed7-11e9-96fe-16c7dea1ce28.jpg)

### Observations:

From the very beginning, this "puppy cafe" was completely anthropocentric. Even one of the owners, Logan Mikhly says: “We’re a dog-friendly cafe, but not a dog cafe.” He also added: “We’re a solution for people who have dogs or are interested in coming to an adoption event." The cafe opened up so people could go out and get coffee, wine or beer, without feeling bad about leaving their dogs alone in their homes. 

When you walk in, you see one of the few dog-centric objects in the cafe, the entrance doors. The cafe has two doors; as soon as you approach the first one, you can see a sign that reminds you to make sure only one door is open time because there are unleashed dogs that could run out into the streets if both doors are open at the same time. Once inside, there is a pet store, with items that the dogs cannot interact with, but that is also completely anthropomorphized like toys that look like champagne bottles or sushi. They have different types of treats, some of them promise to freshen up your dog's breath, which is something I do not believe dogs care about. They have coats and jackets that although seem “stylish” do not seem very functional when it comes to keeping a dog warm, and within this same idea, they also sell bandanas for dogs. 

![img_2887](https://user-images.githubusercontent.com/43420227/53782336-d80c7b00-3eda-11e9-93a4-a2f10961f7ba.jpg)

![img_5843](https://user-images.githubusercontent.com/43420227/53782338-d80c7b00-3eda-11e9-96bc-ae18d06a90c3.jpg)

![img_5235](https://user-images.githubusercontent.com/43420227/53782335-d80c7b00-3eda-11e9-9f06-289ee6fe7da1.jpg)

Past the store, there are a lot of tables and chairs for people to sit down and drink their coffee or work. Dogs are allowed to jump on the seats and rest there, but the seats are completely designed for humans. There are not dog-friendly resting areas or items. In between the tables, there is a photo booth where people take pictures with their dogs, and there are two trunks next to it full of dog costumes for people to dress up their dogs. I have never seen a dog excited about getting one of these on. Next, to the trunks, they also have a kissing booth that can be set up in front of the camera, so the “pooch” is behind it. 

![img_5325](https://user-images.githubusercontent.com/43420227/53782341-d80c7b00-3eda-11e9-84e2-49b06eb37d16.jpg)

![img_9024](https://user-images.githubusercontent.com/43420227/53782342-d8a51180-3eda-11e9-9015-c13367bbe86a.jpg)

Behind the photo booth, there is a big sign with the rules of the place, which make a lot of sense, but at the same time, they limit certain behaviors that are natural in dogs. We saw a couple of dogs playing around, sometimes it seemed like it was getting a little too rough and people would get their dogs to split them up, but they ended up doing it again. It is hard to know when they are being playful and when they are being aggressive. 

![img_5846](https://user-images.githubusercontent.com/43420227/53782337-d80c7b00-3eda-11e9-81fa-762718e6accb.jpg)

Overall it is a nice place, people seem to enjoy having their pets around and being able to play with other people’s dogs, but it doesn’t seem that great for dogs. Something very interesting is that several people sat on the floor to interact with the dogs, which I think is very dog-centric. 


### Redesign:

### Add resting areas for dogs

![resting](https://user-images.githubusercontent.com/43420227/53811358-365f4b00-3f27-11e9-9421-2cd429b1cbd9.jpg)

### Add pet relief area

![petrelief](https://user-images.githubusercontent.com/43420227/53810412-debfe000-3f24-11e9-92cc-31259b10b974.jpg)

### Educate people about play behavior

![posters](https://user-images.githubusercontent.com/43420227/53811699-f5b40180-3f27-11e9-9007-50339c482fed.jpg)

[Go to top.](#design-in-safaris)

---

## Zoo Visit
## Central Park Zoo
03/04/2019

During my visit to the Central Park Zoo, I decided to observe lemurs, because there were no foxes I could observe. The type of lemurs they have is Ruffed Lemurs, and they can be found in the [Tropic Zone: The Rainforest Exhibit](https://centralparkzoo.com/exhibits/tropic-zone-the-rainforest). 


![blackandwhiteruffedlemur_za_4722-b](https://user-images.githubusercontent.com/43420227/53779365-d4bec280-3ecd-11e9-90ab-d3d0615150eb.jpg)

![black-and-white ruffed lemur image4 - alex cearns](https://user-images.githubusercontent.com/43420227/53779367-d5575900-3ecd-11e9-813e-50b25beb9af5.jpg)

### Ethogram

I had a hard time trying to observe these lemurs because they are incredibly fast and they move all over the place. I went from trying to do my ethogram right there to try to record them, but that wasn't completely successful either. I kept losing the lemur I had chosen to follow because they either jumped behind a tree and I no longer was sure I was following the same one when it came from behind it, or sometimes I couldn't move around because people were watching the lemurs. I have several short clips of different lemurs, but I did successfully follow the same one for 12 minutes and 35 seconds. For this round of ethograms, I decided to do instantaneous sampling with my time interval being 30 seconds. 

![lemur - sheet1](https://user-images.githubusercontent.com/43420227/53781282-33883a00-3ed6-11e9-8988-ff7a6c7a190b.jpg)

I was not a fan of the instantaneous sampling because I observed so many interesting behaviors that I wanted to put down, but they would happen in between my intervals. I think even though continuous is hard to do, it is my favorite technique so far.

### Homonculus

While I was obeserving the lemurs, the part of the body that I saw them use the most to interact with the world was their hands. They used them to hold their food, to hang from branches, to hold on to branches, and to scratch themselves. They also use their feet to do a lot of things, but not as much as their hands. The third thing I saw them use the most was their mouth and nose. Their tail mostly just hung, sometimtes they would grab it and groom it, but I did not observe the tail being used for anything. 

![lemurhomunculus](https://user-images.githubusercontent.com/43420227/53808306-e2049d00-3f1f-11e9-9344-7d1a44fa8e16.jpg)

[Go to top.](#design-in-safaris)

### AEIOU

![aeiou](https://user-images.githubusercontent.com/43420227/54008651-94617d80-4135-11e9-9ad4-ec98fd4bcdd8.jpg)

### Behavioral Mapping 

![lemurs](https://user-images.githubusercontent.com/43420227/54009977-eeb10d00-413a-11e9-81ba-db16fcf95508.jpg)

--- 

## Group Enrichment Proposal
## Spotted Hyena
03/07/2019

### Brainstorming

![8431bc3b-7b78-4b14-8de0-8a9f8f4a22e3 copy](https://user-images.githubusercontent.com/43420227/54010008-11dbbc80-413b-11e9-8ecd-d24620610cb7.jpg)

![8431bc3b-7b78-4b14-8de0-8a9f8f4a22e3](https://user-images.githubusercontent.com/43420227/54010014-1607da00-413b-11e9-85bc-1ba56a8a45e5.png)

**Resources:**

* [Cooperative Pulling Paradigm - Meredith Crawford](https://langint.pri.kyoto-u.ac.jp/ai/en/publication/SatoshiHirata/Hirata_and_Fuwa_2007_Primates.html)

* [Behavioral Development In The Spotted Hyena](https://www.researchgate.net/publication/230660902_Behavioral_Development_in_the_Spotted_Hyena)

* [Problem Solving and Social Learning in Spotted Hyena](https://krex.k-state.edu/dspace/bitstream/handle/2097/18258/LindsayKubina2014.pdf?sequence=1)

* [Play Behavior In Spotter Hyenas](http://msuhyenas.blogspot.com/2017/10/play-behavior-in-spotted-hyenas.html)

* [Learning How To Keep a Hyena Happy](https://www.berkeley.edu/news/berkeleyan/1998/0408/hyena.html)

* [Animal Enrichment - Spotted Hyenas](http://www.animalenrichment.org/spotted-heynas)

### Proposal

**Environment Location:**

Meant for spotted hyenas in captivity, zoo environments or rehabilitation centers.
   
**Form:**

We want to build a box that contains a smaller box inside where the food is housed. Each side of the outer box has horizontal slits, and the inner box has ropes are attached to each side that slide through these slits. The bottom of the outer container slides in and out, allowing for different bottoms to be used, each one with a different hole pattern.

**Targeted Animal Behavior/Action:**

The device targets hyenas hunting and collaboration behavior. Hyenas are known for taking down large prey like wildebeest and buffalo by hunting in groups and using their powerful jaw to bite down and hold onto the animal until it falls. The device encourages hyenas to engage their physical and problem-solving capabilities. It requires them to pull the different ropes to move around the box until it passes over a hole and releases food. Hyenas have to work together to succeed and acquire treats/food faster and more efficiently.

**Things To Consider:**

Although this device is meant to create cooperation among hyena clans, based on previous research we found that it is not uncommon that zoos only have one solitary hyena. Although the device can function as feeding enrichment for one individual, it cannot encourage cooperation if there aren’t at least two participants involved.

![untitled 123](https://user-images.githubusercontent.com/43420227/54005685-66297100-4128-11e9-90bb-3c353341a7d4.jpg)

![untitled 124](https://user-images.githubusercontent.com/43420227/54005684-66297100-4128-11e9-89f1-4dd5eccbe45d.jpg)

![untitled 125](https://user-images.githubusercontent.com/43420227/54005683-66297100-4128-11e9-83c0-8c8a855498f2.jpg)

![hyena 127](https://user-images.githubusercontent.com/43420227/54006335-df29c800-412a-11e9-9b68-3ba4c998e281.jpg)

![box](https://user-images.githubusercontent.com/43420227/54007228-bacfea80-412e-11e9-9e08-9eb33da21366.jpg)

[Go to top.](#design-in-safaris) 

--- 



[Go to top.](#design-in-safaris) 

--- 

