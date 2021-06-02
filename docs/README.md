---
layout: home
permalink: index.html
repository-name: ee14-3yp-Smart-Waste-Disposal-Monitoring-System
title: Smart Waste-Disposal Monitoring System
---

# Smart Waste-Disposal Monitoring System

---

## Team
-  E/14/122, Ahmedh J.R., [e14122@eng.pdn.ac.lk](mailto:e14122@eng.pdn.ac.lk)
-  E/14/213, Ariyarathna K.G.D. N., [e14213@eng.pdn.ac.lk](mailto:e14213@eng.pdn.ac.lk)
-  E/14/144, Jaseel M.I. A., [e14144@eng.pdn.ac.lk](mailto:e14144@eng.pdn.ac.lk)

## Table of Contents
1. [Introduction](#introduction)
2. [Solution Architecture](#solution-architecture )
3. [Hardware & Software Designs](#hardware-and-software-designs)
4. [Links](#links)

---

## Introduction
![image](https://user-images.githubusercontent.com/73756777/120498755-1b693300-c3dd-11eb-842c-81c30473cbb3.png)


Waste management is one of the primary problem that the world faces irrespective of the case of developed or developing country. The key issue in the waste management is that the garbage bin at public places gets overflowed well in advance before the commencement of the next cleaning process. Sometime the garbage collector truck not sufficient for collecting all the garbage. These in turn leads to various hazards such as bad odor & ugliness to that place which may be the root cause for spread of various diseases. Another issue is in the waste management is having more trucks and human resources than needed. To avoid all such hazardous scenario and maintain public cleanliness and health this work is mounted on a smart garbage system.

We are living in an age where tasks and systems are fusing together with the power of IOT to have a more efficient system of working and to execute jobs quickly! With all the power at our finger tips this is what we have come up with.

 
![image](https://user-images.githubusercontent.com/73756777/120498791-215f1400-c3dd-11eb-8894-27fcc98baf87.png)



The traditional way of manually monitoring the wastes in waste bins is a cumbersome process and utilizes more human effort, time and cost which can easily be avoided with our present technologies. The main theme of the work is to develop a smart intelligent garbage alert system for a proper garbage management. What our system does is it gives a real time indicator of the garbage level in a trashcan at any given time using weight and volume (solar) sensors. Using that data and as the bins are containing GSM module we can give an alert signal to the municipal web server then optimize waste collection efficient routes, sufficient number of trucks and labors. It allows trash collectors to plan their daily/weekly pick up schedule.


## Solution Architecture
CO321 Embedded Systems:

Garbage monitoring system detect the level of waste in the garbage bin and identify whether garbage bin is full or not by sensors. Location of the garbage bin will identify using GPS. After municipal send the truck to collect wastes from particular bin, a light indicator in bins switch on to inform the people that garbage collector trucks are on their way. Another light indicator in bins is used to inform the worker that the status of garbage bins.

CO324 Network and Web Application Design:

Send the data/message from garbage bins to municipal council to take relevant action. A summary report will send from municipal council to centralized server in main department within a period (per week/ per month).

CO325 Computer and Network Security

The data are sent by the controller in the garbage bin to the server. Database and network system is protected as it sent as encrypted data. Therefore third party couldn’t access and change the data.

## Hardware and Software Designs
The basic Model works like so...

We will first have to enter the height of the dustbin. This will help us to generate the percentage of trash in the trashcan. We then have two criterias which needs to be satisfied to show that the particular bin needs to be emptied :

1.The amount of trash - let's say if a bin is half full we don't really need to empty it. Our thresh, or maximum amount that we permit of trash, is 75% of the bin.

2.If supposing a particular trashcan fills up 20% and then for a week doesn't change, it comes into our second criteria, time. With time even the little amount will start rotting leading to a smelly surrounding. To avoid that our tolerance level is 3 days, so if a trashcan is less than 75% but it is two days old it then will also need to be emptied.

COMPONENTS IN OUR SYSTEM

An ultrasonic sensor will be placed on the interior side of the lid, the one facing the solid waste. As trash increases, the distance between the ultrasonic and the trash decreases.

An weight sensor will be placed on the bottom of the bin. Weight sensor detect the weight of the trash.

This live data will be sent (distance & weight) to our microcontroller.

Our micro- controller then processes the data and through the help of GSM/GPRS module sends it to an app (to MC).

What the app does it visually represents the amount of trash in the bin with a small animation.

This process will indicate all the bins which require attention, leading the user to take the most effective route.



## Links

- <a href = "https://github.com/cepdnaclk/e14-3yp-Smart-Waste-Disposal-Monitoring-System" target = "_blank"> Project Repository </a>
- <a href = "https://cepdnaclk.github.io/e14-3yp-Smart-Waste-Disposal-Monitoring-System/" target = "_blank">Project Page</a>
- <a href = "http://www.ce.pdn.ac.lk/" target = "_blank">Department of Computer Engineering</a>
- <a href = "https://eng.pdn.ac.lk/" target = "_blank">University of Peradeniya</a>



[//]: # (Please refer this to learn more about Markdown syntax)
[//]: # (https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet)
