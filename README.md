# cocoOS
A cooperative operating system based on coroutines

cocoOS is a free, open source, cooperative task scheduler, based on coroutines targeted for embedded microcontrollers like AVR, MSP430 and STM32.


Task procedures scheduled by cooperative kernels are so called RTC's, run to completion tasks. They execute from the first line of the procedure to the last line. 

The use of coroutines enables us to implement task procedures that does not have to execute all the way down to the last line of code. Instead execution can end in the middle e.g waiting for a semaphore to be released. When execution is resumed, it continues at that line. 

With coroutines, this can be done without having to save the complete task context when switching to another task.

 

Also, task procedures can be outlined in the same style as when using a traditional preemptive RTOS.

 

cocoOS is extremely portable to any target which makes it a perfect choice during early phases in the development when which OS to use is still an open issue. You can even run it under Linux or Windows.
