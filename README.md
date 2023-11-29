# Nucleo-F446RE

Nucleo-F446RE is a 32-bit microcontroller that uses ARM Cortex M-4 processor. The Integrated Development Environment (IDE) used to program the microcontroller is STM32CubeIDE. 
STM32CubeIDE incorporates STM32 configuration and offers multiple features and functionalities for user experience. 
It supports C/C++ language including standard and advanced debugging features. The STM32CubeIDE can be downloaded from the website and the ST-Link Debugger must be downloaded as well in order to load the program into the microcontroller. 
STM32CubeIDE is based on the Eclipse development environment which uses the concept of a workspace that houses all the project files in the computer directory.

To program the Nucleo-F446RE, the action item is started off by connecting the microcontroller to PC or laptop using a Type A to Mini B USB cable. 
In the device manager, ensure that PC is able to detect the board. When the board is powered on, 3 LEDs on the board will light up. 
Launch the IDE and start new IDE project. In the board selector column, select the board that is going to program, in this case, select the Nucleo-F446RE as the target board. 
In the project setup pop-up, give the name for the project. Under the option, select the C language as the targeted language. 
After confirming the selection, in the initialize all peripherals with default mode pop-up, select ‘Yes’ to initialize all peripherals. 
Then, switch on the perspective to enable collection of windows, panes and views in Eclipse. After completing the configuration setting, the IDE will download the respective libraries for user configuration in the project.
