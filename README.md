Download Link: https://assignmentchef.com/product/solved-embsys100-module-8-user-defined-vector-table
<br>
The goals for the assignment this week:

<ol>

 <li>Practice setting up a user-defined vector table.</li>

 <li>Practice dealing with interrupts and the use of the SysTick timer.</li>

</ol>

Problems:

<ol>

 <li>Starting from the blinking LED code that you created using the GPIO registers:

  <ol>

   <li>Define your own vector table.</li>

   <li>Enable use of CMSIS in project options settings.</li>

   <li>Add the files “<strong>h</strong>” &amp; “<strong>system_stm32f4xx.h</strong>” to the folder where “main.c” is saved. <em>You should be able to get these files thru STM32CubeMX. You could also get them by downloading the zip file “CMSIS_STM32_Device_Specific_Files.zip” from canvas site under the link </em><a href="https://canvas.uw.edu/courses/1325909/files/folder/EMBSYS%20100%2019/Assignments/A06"><em>Assignment</em></a><a href="https://canvas.uw.edu/courses/1325909/files/folder/EMBSYS%20100%2019/Assignments/A06"><em></em></a><a href="https://canvas.uw.edu/courses/1325909/files/folder/EMBSYS%20100%2019/Assignments/A06"><em>A06 folder</em></a></li>

   <li>Enable the use of the SysTick timer and its interrupt.</li>

   <li>Replace the delay() function with the use of the SysTick timer to blink the user LED.</li>

   <li>Set a break point inside the SysTick_Handler interrupt and capture a snapshot of the stack once inside the interrupt and LR value. Explain what are the values stored on the stack at the moment the Handler gets invoked.</li>

  </ol></li>

</ol>

<ol start="2">

 <li><strong><u>Bonus:</u></strong> Improve your delay function to rely on the use of the SysTick timer instead of the busywait loop.

  <ol>

   <li>Function prototype: <strong>void delay(uint32_t delayInMilliseconds) </strong></li>

   <li>Use the function in your main.c file to blink the LED every 2 seconds.</li>

   <li><u>Hint:</u> Setup the SysTick timer to trigger an interrupt every 1ms.</li>

  </ol></li>

</ol>