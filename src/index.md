---
layout: home
title: L-ONE&#58; starter kit for going it alone
postsHeading: Latest posts
archiveButtonText: See all posts
metaDesc: 'L-One is an ESP32-based IoT wireless node starter kit, featuring thermal imaging and blob detection.'
socialImage: ''
---


L-ONE is a hardware+firmware starter platform for the Internet of Things (IoT) / Machine-to-machine (M2M) applications, initially developed as an educational project by the Interactive Prototyping studio course at Woodbury University’s [Applied Computer Science program] (https://woodbury.edu/program/school-of-media-culture-design/applied-computer-science/)

The title of the project stands for “Level-One,” to imply that the platform aims to be a beginner hardware kit suitable for a first-level, introductory course in physical computing or electronics + software prototyping.  The characters of the name can also be rearranged to spell “LEON,” a tribute to Leon Theremin’s invention of his namesake musical instrument one hundred years ago in 1920.

Another way to read the project title is by pronouncing it as the word “alone” (/əˈlōn/). The specific context for the project happened to be the Covid-19 pandemic unfolding in the spring of 2020, necessitating a sudden transition of all class instruction online due to newly implemented stay-at-home and social distancing guidelines.  This new reality ultimately led to a re-imagination of the ongoing studio course around a brief that would support students working remotely, while trying to address the unprecedented situation in a meaningful way. 

The resulting project’s brief challenged the students to build a wearable “social distancing” device based on a programmable electronic kit coupled with a miniature infrared thermal imaging sensor.  The device would help the wearer maintain recommended social distancing guidelines by interpreting sensor data and indicate safe/unsafe distance to other people via graphical display, lights and/or sound.

In order to facilitate project development and make it possible to rapidly distribute necessary components to the students, it was conceived around an off-the-shelf hardware platform based off a popular programmable microprocessor platform (ESP32 by Espressif Systems): M5StickC kit featuring the microprocessor board in a plastic enclosure with built-in screen, rechargeable battery, LED light and a plug-in speaker module.  The kit was supplemented with the AMG8833 infrared thermal array sensor module capable of imaging temperature data at a distance with 8x8 resolution.  The hardware components were chosen with an eye to availability from online distributors in the US, based on available inventory for shipping components directly to the students.

Over the course of several weeks the project evolved around a firmware framework supporting full integration of the hardware components via Arduino IDE, the integrated development environment students have been learning during the semester.  Core programming functionality was provided by code libraries found online, adapted to use with the particular hardware configuration.  The code grew to include “blob tracking” functionality enabling persistent detection and tracking of people over successive frames of thermal sensor data, adapted from an algorithm designed for computer vision applications with a video camera.

Based on the technology framework developed over remote working sessions, the final project for the course instructed students to design and implement a functional prototype of a wearable “social distancing device” in a DIY (Do It Yourself) enclosure.  The students were given freedom to come up with physical form, imagine use scenarios for the device, its location on the body, and integrate hardware outputs such as built-in screen graphics and plug-in sound module.  The assignment also required the prototype to demonstrate core IoT functionality by logging collected sensor data to the cloud via wireless networking and the Adafruit IO API.

[TODO] Specific details and instructions for (re-)creating the project by anyone interested in the underlying technology and its implementation aspects will be provided in separate posts listed below, attempting to document the overall effort as a set of tutorials.

