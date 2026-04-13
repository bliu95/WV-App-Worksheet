# High Low with Alerts & Timers
You will redesign your High Low - Part 1: Random Number Guesser project from Week 2 to include an alert that indicates that the user has successfully guessed the correct number, then a timer to show how much time has passed. First, make a duplicate of your project so your changes do not affect your original project.
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_1.png)
Starting in the blocks tab, you should see the blocks from the original project.
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_2.png)
Find **Alerts** under the **App Features** section. Click the **plus sign** next to **Alerts** to add an alert to your project.
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_3.png)
In the pop-up panel, let's populate the **Title** and **Message** to indicate to the user that they have successfully guessed the correct number. We will also clear the **cancelButton Text** so the alert will only show 1 button when it appears.
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_4.png)
Now, we want to add the alert's functionality to the blocks. We want it to appear when the user's guess is equal to the correct answer, so we will do the following:
1. Remove the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Result's Text to</span> block from the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> section.
2. Add the <span style="background-color:#735ca5;font-weight:bold;color:white">call Alert1's Show</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> section.
Instead of simply updating the "Result" label, we now indicate that the user's guess is correct in a more elegant way.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">call Alert's Show</span></div><img src="./Weeks/Week 10/images/w10_block_callAlertsShow.png" alt="Block: call Alert's Show"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Alert Blocks</span> drawer under <span style="font-weight:bold">App Features</span> after an Alert has been added.</span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">call Alert's Show</span> block is used to display the alert to the user. Its output <span style="background-color:#70ce9c;font-weight:bold;color:white">wasConfirmed</span> is set to "true" if the user clicks the confirm button and "false" if the user clicks the cancel button.</div></div>
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #1: Verify Alert]</span><br>
Preview the app. Check if the alert pops up after the user guesses the correct number.<br>
If it works, you now have updated your random number guesser to use alerts to indicate when the user has found the answer!<br>
**Let's move to the Design tab.**
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_6.png)
Add a label to display the elapsed time. We will rename it to "TimerLabel". In the properties panel, clear the default text "Label" so the label is blank.<br>
**After adding the components, let's move on to the Blocks tab.**
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_7.png)
Find **Timers** under the **App Features** section. Click the **plus sign** next to **Timers** to add a timer to your project.
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_8.png)
In the pop-up panel, let's change the **Interval** to 1 second and enable the **Loops** toggle.<br>
Having the **Interval** set to 1 second means the timer will fire for every 1 second that has passed. This is how we would be able to display elapsed time that increases for every second that has passed while the timer is on.<br>
Having **Loops** toggled means the timer will continue running after it has started, meaning the timer will continue to fire for every 1 second until it is manually stopped.
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_9.png)
Now, we will add functionality to the timer:
1. Add the <span style="background-color:#735ca5;font-weight:bold;color:white">call Timer1's Start</span> block to the top of the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block so the timer starts as soon as the user makes their first guess.
2. Add the <span style="background-color:#735ca5;font-weight:bold;color:white">call Timer1's Stop</span> block below the <span style="background-color:#735ca5;font-weight:bold;color:white">call Alert1's Show</span> block within the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> section so the timer stops when the user's guess is correct.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">call Timer's Start</span></div><img src="./Weeks/Week 10/images/w10_block_callTimersStart.png" alt="Block: call Timer's Start"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Timer Blocks</span> drawer under <span style="font-weight:bold">App Features</span> after a Timer has been added.</span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">call Timer's Start</span> block is used to start the timer.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">call Timer's Stop</span></div><img src="./Weeks/Week 10/images/w10_block_callTimersStop.png" alt="Block: call Timer's Stop"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Timer Blocks</span> drawer under <span style="font-weight:bold">App Features</span> after a Timer has been added.</span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">call Timer's Stop</span> block is used to stop the timer.</div></div>
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_10.png)
Create a variable with the <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span> block to hold the elapsed time. We will rename it to <span style="background-color:#f7c9bd;font-weight:bold">timePassed</span>. Then set its value to 0 using the <span style="background-color:#6789cc;font-weight:bold;color:white">specify number</span> block.
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_11.png)
Now, let's work on displaying the elapsed time. We will first add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Timer1 Fires</span> block. Remember, the interval for the timer is set to 1 second, which means it will fire for every 1 second that has passed while the timer is on.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#f3aa44;font-weight:bold;color:white">when Timer Fires</span></div><img src="./Weeks/Week 10/images/w10_block_whenTimerFires.png" alt="Block: when Timer Fires"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Timer Blocks</span> drawer under <span style="font-weight:bold">App Features</span> after a Timer has been added.</span><br>
The <span style="background-color:#f3aa44;font-weight:bold;color:white">when Timer Fires</span> block is used to set something to run when the timer fires.</div></div>
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_12.png)
Next, we want to update the <span style="background-color:#f7c9bd;font-weight:bold">timePassed</span> variable to increase by 1 every time the timer fires. To do that, we will add the <span style="background-color:#f87956;font-weight:bold;color:white">change variable by</span> block within the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Timer Fires</span> block.<br>
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_13.png)
Finally, we will display the elapsed time in the "TimerLabel". First, we will add the <span style="background-color:#3f9e83;font-weight:bold;color:white">set TimerLabel's Text to</span> block. Then, we will:
1. Connect the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set TimerLabel's Text to</span> block.
2. Replace the top <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with the <span style="background-color:#f87956;font-weight:bold;color:white">app variable timePassed</span> block.
3. In the bottom <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block, replace the text "world" to " seconds".
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_14.png)
For final touches, when the timer stops, we also want the <span style="background-color:#f7c9bd;font-weight:bold">timePassed</span> variable to be reset. We will add the <span style="background-color:#f87956;font-weight:bold;color:white">set variable to</span> block below the <span style="background-color:#735ca5;font-weight:bold;color:white">call Timer1's Stop</span> block and set its value to 0 using the <span style="background-color:#6789cc;font-weight:bold;color:white">specify number</span> block.
---

# High Low with Alerts & Timers
![Setup](./Weeks/Week 10/images/w10_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #2: Verify Timer]</span><br>
Preview the app. Check if the timer starts and the elapsed time displays.<br>
If it works, you now have a random number guesser that displays an alert to indicate when the user has found the answer and shows the elapsed time that the user has spent playing the game!
---

# High Low with Alerts & Timers - Extension #1: Reset Game
<span style="font-weight:bold">[Extension #1: Reset Game]</span><br>
Currently, there is no way to reset the game should the user wish to play again. In this extension, you will add this functionality to the game.