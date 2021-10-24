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

## CUSTOMIZATIONS

You can change how you'll be notified when a task is added in your Todoist account, today we have two options on how to do it:

### Using Rofi as notification

This is the default behavior, when a task is added, Rofi will be re-opened with the success message.

### Using notify-send

This method will use `notify-send` that uses your SO default notification system. To use this option you need to set at least one environment variable:

```
$ echo "export $ROFI_TODOIST_NOTIFICATION=notify-send > ~/.bash_profile
```

Also, you can configure where you clone this repository to use the Todoist icon on the notification:

```
$ echo "export $ROFI_TODOIST_ROOT_PATH=path-where-you-clonned > ~/.bash_profile
```

Those examples assume that you're using Bash, if you're using zshel, fish or other one you must change the `.bash_profile` file to the right one.
