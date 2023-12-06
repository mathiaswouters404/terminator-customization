# terminator-customization

## Steps:

1. **Open** Terminator

2. Right click -> **Preferences**

3. In the **Layouts** tab (to the right of the **Profiles** tab), edit the default one, you will see that it says **Window | window0** and **Terminal | child1**

4. For the **Terminal | child1**, you can set: a **Profile** (to choose from the installed ones), a **Default command**, and a **Working directory**

5. **Set** it/them to whatever you like, **close**, **reopen** again...

6. ... and **voilá**!


## Steps:

1. After setting up your layout, right-click on any terminal background and choose **Preferences → Layouts** tab and click on **Add** button

2. Give it a name and hit **Close**

3. This should create the mentioned ```~/.config/terminator/config``` file

4. Now you can start terminator using the saved layout using: ```terminator -l yourLayout``` (replace yourLayout with whatever you chose on step 2)

5. **(optional)** Edit the ```~/.config/terminator/config``` file so that where it says ```[layouts]``` and nested below it ```[[yourLayout]]```, rename yourLayout to default and remove/rename the previous default layout. Now, when Terminator starts without any parameters, it will load your custom ```[[default]]``` layout!

6. **(optional)** Edit the ```[[[terminalx]]]/ command = a custom command;bash``` eg: ```command = ssh user@IP;bash``` (ending with bash) for each terminal, so that it will run your custom command during startup!!
