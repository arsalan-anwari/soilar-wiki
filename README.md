
# About

Soilar is the go-to solution which allows professionals and consumers in the agricultural field to buy backwards compatible, modular and interchangeable components from different brands to get a fair and competitive price which is highly expandable with new unique features throughout the future. With the online platform you can also easily connect to professionals and freelancers in the field, get advice and guidance on new or existing technologies that can help your company grow or sell and advertise your new upcoming product to potential clients in the agricultural sector.

It is made of multiple different subprojects that in the end will result in the final product. The subprojects consist of:

- Researching how to increase crop yield in the agriculture sector by using smart devices like an IoT system to decrease the usage of fertilizers, water, nutrients and mechanical manual labor but still giving the target demographic the option to configure the system to an extent that is usable to them. -> Done
- Developing the radio software using the LoRa project. -> Done
- Writing the firmware for all the different embedded components used -> Pending
- Designing the outer case of the system. -> Pending
- Designing the PCB motherboard of the system. -> Pending
- Creating the front end application -> Not started
- Setting up a server and managing the backend in .NET -> Not started

## Research

In the field of soil science, there are already many discoveries made on how to design smart devices to measure and regulate the pH or moisture level. Whilst these being good ways to increase the crop yield, I have yet to see a system that goes into the more detailed and complicated aspects of farming like fungus detection and prevention, purification of filthy water, preventing diseases due to intensive tillage, checking and regulating nutrients in the soil and increasing the fertility of the soil by slowing down nitrification. When looking at existing solutions like the following example for a pH measurement IoT system or other studies online, we can clearly see a pattern of systems that only measure and regulate one or more aspects of the soil. And the systems that do measure the remaining aspects are mostly too expensive for everyone to afford. Another issue with current systems, is the fact that they mainly focus on measuring parameters in the soil and not so much on lesser known aspects of plant science, like in the air and others.

This is due to the negative effect which occurs when placing many sensitive measurement components in a small space. Doing this can result in sensors or components interfering with each other, which in turn decreases the accuracy of the measurements. In a report about the deterioration of measurements due to interference of multiple sensors RGB-D sensors, it is briefly mentioned that 95% of depth measurements can be lost when two sensors interfere with each other. Of course, these kinds of sensors are highly sensitive to noise and sensors used for IoT system in agriculture are not nearly this bad. But it can be still noted that even these types of sensors have a high percent chance to intervene with each other and can reduce the accuracy. This makes building all in one system that have multiple sensors more complex, which increases prices.

When designing a new alternative which builds up on all the work done by existing research, I understood that a complete package where all the above-mentioned aspects of farming are measured and regulated has yet to be developed or designed in such a way that is affordable for a large range of people of the target demographic. The purpose of this document is to design such a system and research what other functionality can be desired by professionals in the agricultural sector.

## Lora radio software

This contains firmware for things like RF modules in a generalized HAL written in C and C++. The library is made to be natively compatible with PlatformIO.

There are two branched where the different implementations for the different devices used are. The master branch is empty

## Firmware embedded components

Writing software that communicates with a range of different sensors, encoders, and other embedded hardware. Software that handles abstract communication between all these components and handles hot swapping.

## Outer case design

I have created an 3D model of the different cases and devices used. The ModuleTemplate(Endnode) can support multiple Submodules which a slotted in with a sliding mechanism. The GridNode(GateWay) had multiple extension ports where submodules can be added (for example for more GPU power or Storage).

The model was initially designed in Sketchup but then ported to FreeCAD, so it can be 3D printed more easily.

## PCB design

I have designed a PCB with electrical components in KiCAD and FreeCAD. It is based on an electrical circuit I designed on a protoboard.

It works with an STM32 microcontroller and is designed to prototype with two LoRa Transceivers (RFM95W).

## Front end application

In design phase

## Back-end management

In design phase
