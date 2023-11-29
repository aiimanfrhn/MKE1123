#How to modify the program

To modify the program, open the main.c file. 
In the main function which is the beginning of the program, within the while (1) loop, add the code to blink the LED. 
In the while loop, the program will be executed in a repetition mode. ST’s hardware abstraction layer (HAL) makes controlling of some of the peripherals in the microcontroller. 
Here, we use HAL_Delay(500); to provide delay of 500ms. So, the LED should blink every 500ms. In the next line, add in the HAL_GPIO_TogglePin(LD2_GPIO_Port, LD2_Pin);. 
This line of code toggle the GPIO pin which will trigger the LED2 to blink via the GPIO port. 
There’s library functions that were used to initialize the system clocks and various peripherals. In this program, we will just leave it as default with baud rate of 115200.   
Then, under the ‘Run’ column, build and launch a debug session. Wait for the configuration to complete and the status of the debugging can be viewed through the console. 
When the process completes and reflects a success status, the LED2 on the board starts to blink. 
