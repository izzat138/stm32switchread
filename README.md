# stm32knightrider
This repository documents the details of Knight Rider project on an STM32F103C8T6 MCU using STM32CubeIDE, an open-source C/C++ development platform for STM32 microcontrollers and microprocessors.

We are required to program an STM32 MCU using open-source STM32CubeIDE in C language to implement the Knight Rider lights. A C code is included in this repository for reference.

stm32knightrider contains the project that use pins GPIOA-PIN0, GPIOA-PIN4, GPIOA-PIN6, GPIOA-PIN7, GPIOB-PIN0, GPIOB-PIN1, GPIOB-PIN10 and GPIOB-PIN11 to light up the LEDs with the Knight Rider pattern.



## Group Members (Driven Raven)
1. Ashraf Aminin bin Arman Alim
2. Izzat bin Idris



## Project Prerequisites
1. STM32CubeIDE software
2. STM32 MCU



## Hardware Requirements
1. Leds - 8
2. 1k ohm resistors - 8



## Project Procedures
1. Start a new STM32 project on STM32CubeIDE and input part number according to the MCU being used.

![Semantic description of image](/image/pic1.jpg)


<br/>
<br/>


2. Input valid project name and click finish.

![Semantic description of image](/image/pic2.png)


<br/>
<br/>


3. Assign any output pins as the GPIO output pin by clicking the pin in the pinout view. Configuration for SYS under system core pull-down menu is set to **serial wire** for debugging mode and **SysTrick** as timebase source. Save the project to generate C code for given project configurations.

![Semantic description of image](/image/pic3.png)


<br/>
<br/>


4. Only a section of the generated code is modified. In this project, the executing loop is added with built-in functions to blink the LED on the MCU with 0.5 seconds interval. 

![Semantic description of image](/image/pic4.png)


<br/>
<br/>


5. Under project properties(Right click project, select properties), select to convert builds to binary and hex files under MCU Post build outputs. Apply the changes.

![Semantic description of image](/image/pic6.png)


<br/>
<br/>


6. Start building the debug for the current project.

![Semantic description of image](/image/pic5.png)


<br/>
<br/>


7. Connect the STM32 with all the components as shown below

![Semantic description of image](/image/schematic.png)


<br/>
<br/>


8. STM32 ST-LINK Utility is utilized to program the SM32F103C8T6 MCU through an ST-LINK V2. The generated binary/hex files are opened through this application.

![Semantic description of image](/image/pic7.png)


<br/>
<br/>


9. Connect the STM32 MCU through the USB port with the ST-LINK V2. Then, connect with the MCU in the utility and start to program it.

![Semantic description of image](/image/pic8.png)


<br/>
<br/>


# Project Demo

https://user-images.githubusercontent.com/106621749/203887910-23e8e2eb-df35-451b-80b0-0079ab214625.mp4

*Youtube URL: https://youtu.be/yMYyeOzHdus*


<br/>
<br/>


# Reflections

This basic STM32 project creation facilitates us to understand the capabilities and utilities provided by STM32CubeIDE to program an STM32 MCU. This repository can be referred for any future project creations.

In addition, counterfeit ST-LINK is an ongoing issue being investigated by STMicroelectronics. In the recent releases of STM32CubeIDE, a counter measure is made by STMicroelectronics to prevent the programming of an STM32 MCU with a counterfeit ST-LINK. However, to overcome the difficulty of finding and owning an actual ST-LINK, STM32 ST-LINK Utility can be used to program STM32 MCU instead with a cloned ST-LINK.




# References

*Youtube URL (Creation of Blinky project): https://youtu.be/kXg467nVd_A*
