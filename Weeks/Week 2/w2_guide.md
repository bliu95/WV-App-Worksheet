# High Low
![Setup](./Weeks/Week 2/images/w2_p1_1.png)
Add a <span style="background-color:#90ee90">text input</span> for users to type in a guess. Rename it to <span style="font-style: italics">Text_Input</span>.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_2.png)
Add a <span style="background-color:#90ee90">button</span> for users to submit the guess. Rename it to <span style="font-style: italics">Submit</span>.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_3.png)
Add a <span style="background-color:#90ee90">label</span> to indicate whether the guess was correct, too high, or too low. Rename it to <span style="font-style: italics">Result</span>.
---

# High Low
Now, we will move onto blocks.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_4.png)
Create a variable with the <span style="background-color:coral">initialize variable to</span> block to hold the correct answer. Rename it to <span style="font-style: italics">answer</span>.

<span style="font-weight:bold">Block:</span> <span style="background-color:coral">initialize variable to</span>
![Block](./Weeks/Week 2/images/w2_p1_block_initvar.png)
Used to create a variable when the app starts. The dropdown menu can be used to select the variable type or scope.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_5.png)
Set the variable <span style="font-style: italics">answer</span> to a number of your choice by connecting the <span style="background-color:#4682b4">specify number</span> block to the <span style="background-color:coral">initialize variable to</span> block. Set it to 50.

<span style="font-weight:bold">Block:</span> <span style="background-color:#4682b4">specify number</span>
![Block](./Weeks/Week 2/images/w2_p1_block_number.png)
Used to specify a number you want to use in your app. You can edit the number in the block.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_6.png)
Add the <span style="background-color:#ffce42">when Submit Click</span> block to add functionality to the button.

<span style="font-weight:bold">Block:</span> <span style="background-color:#ffce42">when Button Click</span>
![Block](./Weeks/Week 2/images/w2_p1_block_whenclick.png)
Used to run the blocks within the do part when the button is clicked.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_7.png)
Connect the <span style="background-color:#ffce42">if</span> block to the <span style="background-color:#ffce42">when Submit Click</span> block to perform an action based on a condition.

<span style="font-weight:bold">Block:</span> <span style="background-color:#ffce42">if</span>
![Block](./Weeks/Week 2/images/w2_p1_block_if.png)
Checks a statement and runs the block inside do if the statement is true.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_8.png)
Connect the <span style="background-color:#20b2aa">comparison</span> block to the if part of the <span style="background-color:#ffce42">if</span> block to compare the user's guess to the answer.

<span style="font-weight:bold">Block:</span> <span style="background-color:#20b2aa">comparison</span>
![Block](./Weeks/Week 2/images/w2_p1_block_comparison.png)
Compares two values and returns True or False based on whether the condition is met.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_9.png)
Connect the <span style="background-color:#90ee90">Text_Input's Text</span> block to the left side of the <span style="background-color:#20b2aa">comparison</span> block.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_10.png)
Connect the <span style="background-color:coral">app variable answer</span> block to the right side of the <span style="background-color:#20b2aa">comparison</span> block.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_11.png)
Connect the <span style="background-color:#3cb371">set Result's Text to</span> block to the do part of the <span style="background-color:#ffce42">if</span> block. Replace "Label" with "Correct".
---

# High Low
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #1: Correct Answer Check</span>]: Preview the app. See if the Result label indicates whether the guess is correct.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_13.png)
Click the <span style="font-weight:bold">+</span> icon next to the if to add an <span style="font-style: italics">else if</span> section.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_14.png)
Connect the <span style="background-color:#20b2aa">comparison</span> block to the else if section. Use the <span style="font-weight:bold"><</span> comparison operator. Connect <span style="background-color:#90ee90">Text_Input's Text</span> block and the <span style="background-color:coral">app variable answer</span> block.

Add a <span style="background-color:#3cb371">set Result's Text to</span> block inside the else if section. Change the text to "Too low".
---

# High Low
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #2: Too Low Logic</span>]: Preview the app. See if the Result label indicates whether the guess is too low.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_16.png)
Click the <span style="font-weight:bold">+</span> icon next to do to add an <span style="font-style: italics">else</span> section.

<span style="font-weight:bold">Block:</span> <span style="background-color:#ffce42">if-else</span>
![Block](./Weeks/Week 2/images/w2_p1_block_ifelse.png)
In an if-else block, the do part runs if the statement is true and the else part runs if the statement is false.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_17.png)
Connect the <span style="background-color:#3cb371">set Result's Text to</span> block to the do part of the else section. Replace "Label" with "Too high".
---

# High Low
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #3: Too High Logic</span>]: Preview the app. See if the Result label indicates whether the guess is too high.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_19.png)
Replace the <span style="background-color:#4682b4">specify number</span> block with the <span style="background-color:#4682b4">random integer from 1 to 100</span> block for a randomized answer.

<span style="font-weight:bold">Block:</span> <span style="background-color:#4682b4">random integer from 1 to 100</span>
![Block](./Weeks/Week 2/images/w2_p1_block_random.png)
Used to generate a random number between 1 and 100.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #4: Random Number</span>]: Preview the app. See if the number is different each time.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_1.png)
In Part 2, we will create a real-time communication system. Two users will communicate: a Guesser makes guesses while a Clue Giver provides feedback.

In a new project, add a <span style="background-color:#90ee90">text input</span> for the two users to type in their message. Rename it to <span style="font-style: italics">Text_Input</span>.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_2.png)
Add a <span style="background-color:#90ee90">button</span> for users to submit their message. Rename it to <span style="font-style: italics">Submit</span>.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_3.png)
Add a <span style="background-color:#90ee90">label</span> to display submitted messages. Rename it to <span style="font-style: italics">Message</span>.
---

# High Low - Part 2
Now, we will move onto blocks using cloud variables.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_4.png)
Create a <span style="background-color:#9370db">cloud variable</span> with the <span style="background-color:coral">initialize variable to</span> block. Rename it to <span style="font-style: italics">text</span>.

**Important:** Use a cloud variable, not an app variable!

<span style="font-weight:bold">Block:</span> <span style="background-color:#9370db">cloud variable</span>
![Block](./Weeks/Week 2/images/w2_p2_block_cloud.png)
Allows you to store data in the cloud. This data can be accessed from multiple devices.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_5.png)
Add the <span style="background-color:#ffce42">when Submit Click</span> block for the button.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_6.png)
Connect the <span style="background-color:#9370db">set cloud variable to</span> block to the <span style="background-color:#ffce42">when Submit Click</span> block to update the cloud variable <span style="font-style: italics">text</span>.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_7.png)
Connect the <span style="background-color:#90ee90">Text_Input's Text</span> block to the <span style="background-color:#9370db">set cloud variable to</span> block to set the cloud variable <span style="font-style: italics">text</span>.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_8.png)
Add the <span style="background-color:#ffce42">when cloud variable text initializes or changes</span> block to define how the app behaves when the variable changes.

<span style="font-weight:bold">Block:</span> <span style="background-color:#ffce42">when variable initializes or changes</span>
![Block](./Weeks/Week 2/images/w2_p2_block_whenchanges.png)
Used to define how the app behaves when the variable initializes or changes.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_9.png)
Connect the <span style="background-color:#3cb371">set Message's Text to</span> block to the <span style="background-color:#ffce42">when cloud variable text initializes or changes</span> block.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_10.png)
Connect the <span style="background-color:#9370db">cloud variable text</span> block to the <span style="background-color:#3cb371">set Message's Text to</span> block so users can communicate.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #5: Real-Time Updates</span>]: Preview the app. See if the Message label updates to what a user enters after clicking Submit.
---

# High Low - Extension 1
**Extension 1: Multiple Screens**

In this extension, you will create dedicated screens for the Guesser and Clue Giver.

Make a copy of your project from Part 2.
---

# High Low - Extension 1
Have 3 screens total:
1. A home screen to choose your role
2. A Guesser screen for making guesses
3. A Clue Giver screen for providing feedback
---

# High Low - Extension 1
Give the Guesser and Clue Giver the components needed to input text on their respective screens.
---

# High Low - Extension 1
Add the blocks for the Guesser and Clue Giver to communicate with each other using cloud variables.

<span style="font-weight:bold">Block:</span> <span style="background-color:#ffce42">navigate to</span>
![Block](./Weeks/Week 2/images/w2_ext1_block_navigate.png)
Takes the user to the defined screen.
---

# High Low - Extension 1
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #6: Multiple Screens</span>]: Preview the app. Test that you can navigate between screens and that communication works between the Guesser and Clue Giver screens.
