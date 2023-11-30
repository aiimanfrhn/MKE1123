# Milestone 1 
STM32 Familiarization

# Team Member (Group 2): 

1. Yvonne Wong Liang Liang
2. Koay Yi Yun
3. Aiman Farhan


# How to Program Blinky (STM32)
To program the Nucleo-F446RE, the action item is started off by connecting the microcontroller to PC or laptop using a Type A to Mini B USB cable. 
In the device manager, ensure that PC is able to detect the board. When the board is powered on, 3 LEDs on the board will light up. 
Launch the IDE and start new IDE project. In the board selector column, select the board that is going to program, in this case, select the Nucleo-F446RE as the target board. 
In the project setup pop-up, give the name for the project. Under the option, select the C language as the targeted language. 
After confirming the selection, in the initialize all peripherals with default mode pop-up, select ‘Yes’ to initialize all peripherals. 
Then, switch on the perspective to enable collection of windows, panes and views in Eclipse. After completing the configuration setting, the IDE will download the respective libraries for user configuration in the project.

To modify the program, open the main.c file. 
In the main function which is the beginning of the program, within the while (1) loop, add the code to blink the LED. 
In the while loop, the program will be executed in a repetition mode. ST’s hardware abstraction layer (HAL) makes controlling of some of the peripherals in the microcontroller. 
Here, we use HAL_Delay(500); to provide delay of 500ms. So, the LED should blink every 500ms. In the next line, add in the HAL_GPIO_TogglePin(LD2_GPIO_Port, LD2_Pin);. 
This line of code toggle the GPIO pin which will trigger the LED2 to blink via the GPIO port. 
There’s library functions that were used to initialize the system clocks and various peripherals. In this program, we will just leave it as default with baud rate of 115200.   
Then, under the ‘Run’ column, build and launch a debug session. Wait for the configuration to complete and the status of the debugging can be viewed through the console. 
When the process completes and reflects a success status, the LED2 on the board starts to blink. 

# Link
https://www.youtube.com/watch?v=diDKnxnd_Go
