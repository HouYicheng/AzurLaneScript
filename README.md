# AzurLaneScript
Just for personal practice and use, anyone who is interested can see the code and try to do something.

#### The new functions added by each release can be seen at the release page, the bugs can be see through issues.

### Modules(To be Updated):

1. Screen Checker: Used for checking the stage of the game.
   1. Use the Yolo to do the computer vision part
   2. Needs a single thread for the function dealing
   3. Write the data back to a shared memory which the main thread will read from to check which command to use.
2.  Command Executer: Used for sending the command to the simulator.
   1. Use the simulator adb and port number to do the command executing.
   2. Planned Commands: click, long press, slide
   3. Planned to support different resolution

