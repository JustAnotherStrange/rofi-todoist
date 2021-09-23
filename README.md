# rofi-todoist
## WARNING: THIS IS A WORK IN PROGRESS. 
This is a rofi tool written in bash for viewing, adding, completing, and modifying Todoist tasks using https://github.com/sachaos/todoist. 

![DEMO](https://github.com/JustAnotherStrange/rofi-todoist/raw/master/demo.gif)

Current status: Works enough for me. Submit any issues or PR's you'd like if you find issues.
## USAGE
Use List Tasks option to list tasks. Selecting a task from this menu will prompt with actions to do, such as complete the task or modify it. 

Use the Add task option to add a task using explicit syntax. 

Use the Quick Add option to add a task using the Todoist smart Quick Add feature, where it recognizes the time, name, and date of the task by reading a sentence you write. 

At any time press the escape key to exit, and press the exit option to go up a menu.

You can pass the argument `fq` to open a `fast_quick_add` and skip the menu page in the system.
