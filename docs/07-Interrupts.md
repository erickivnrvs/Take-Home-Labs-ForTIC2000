# Interrupts
One of the key aspects of using a microcontroller is being able to handle interruptions. This allows us to have multiple tasks running at the same time and decide when and how to handle them.

## What is an interruption?
Before working with interruptions, let's understand what is an interruption. Let's put it side by side using an analogy. Imagine you're using your phone. You can do multiple tasks like listen to music, watch videos, and so on. You, as the user, can decide which one to do at a certain time. Now, while one of this tasks is running, you receive a phone call. The actual task stops and now the system focuses on showing you the information of the incoming call. Now your attention is focused on either answering or hanging up. Once the incoming call is done (the task has been handled), your phone goes back to whatever task it was running before the call.

On a microcontroller, the logic works the same way. We'll have a "main" branch that is constantly running, while other minor tasks will be running on the background. Once any of this tasks is done, it sends a flag to indicate that it has been finished. The microcontroller momentarily stops the main bracnch, handles the request, and then goes back to where it left at the main branch (hence the name "interruption").

## Hardware and Software interrupts
There are two kinds of interrupts; Hardware and Software interrupts. Hardware interrupts happen whenever there is any sort of physical change on a given input (either digital or analog). 

Sofwtare interrupts, on the other hand, are usually used to indicate when an inner process (for example, any sort of data processing or mathematical calculation) is done, a register stores this information so that the flow of the program can decide which steps need to be done.

## Using the interrupt block on the C2000 Microcontroller blockset
