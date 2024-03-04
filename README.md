# AzurLaneScript
Just for personal practice and use, anyone who is interested can see the code and try to do something.

#### The new functions added by each release can be seen at the release page, the bugs can be see through issues.

### Main Ideas:
1. The system is designed into frontend and back end. Backend is mainly used for executing the commands and listen to the frontend for messages. Frontend part is used to send commands to the bac end.
2. The frontend will send a json to the backend, then the backend will use a Task Generator to generate the cooresponding tasks. Task is a higher level concept than commands. Task can be seen as a combination of commands to execute one service. A service can be thought the same as the task, the difference is, the service is used in the frontend, and when it's sent to the backend, it uses a *factory class* to generate a task data structure.
3. After we have received tasks, push them into a stack according to the logical order.

### Modules(To be Updated):

1. Screen Checker: Used for checking the stage of the game.
   1. Use the Yolo to do the computer vision part
   2. Needs a single thread for the function dealing
   3. Write the data back to a shared memory which the main thread will read from to check which command to use.
2.  Command Executer: Used for sending the command to the simulator.
   1. Use the simulator adb and port number to do the command executing.
   2. Planned Commands: click, long press, slide
   3. Planned to support different resolution
3.  Task Generator: Used 
