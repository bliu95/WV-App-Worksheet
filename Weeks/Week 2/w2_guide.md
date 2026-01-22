# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_1.png)
Add a text input for users to type in a guess. We will rename it to "Text_Input".
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_2.png)
Add a button for users to submit the guess. We will rename it to “Submit”.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_3.png)
Add a label to indicate whether the guess was correct, too high, or too low. We will rename it to "Result".<br>
**Now, we will move onto blocks.**
---

# High Low - Part 1: Random Number Guesser
<span style="font-weight:bold">Block:</span> <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span>

![Block](./Weeks/Week 2/images/w2_p1_block_initAppVar.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#f87956">Variables Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span> block is used to create a variable when the app starts. The dropdown menu can be used to select the variable type or scope (app, stored, or cloud). It is good practice to give variables unique names so you can distinguish between different variables.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_4.png)
Create a variable with the <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span> block to hold the correct answer. We will rename it to <span style="background-color:#f7c9bd;font-weight:bold">answer</span>.
---

# High Low - Part 1: Random Number Guesser
<span style="font-weight:bold">Block:</span> <span style="background-color:#6789cc;font-weight:bold;color:white">specify number</span>

![Block](./Weeks/Week 2/images/w2_p1_block_specifyNum.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#6789cc">Math Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#6789cc;font-weight:bold;color:white">specify number</span> block is used to specify a number you want to use in your app. You can edit the number in the block to be any number of your choice.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_5.png)
Set the variable <span style="background-color:#f7c9bd;font-weight:bold">answer</span> to a number of your choice by connecting the <span style="background-color:#6789cc;font-weight:bold;color:white">specify number</span> block to the <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span> block. We will set it to <span style="background-color:#c2d0eb;font-weight:bold">50</span>. This will be a temporary pre-set answer for testing purposes which we will change later.
---

# High Low - Part 1: Random Number Guesser
<span style="font-weight:bold">Block:</span> <span style="background-color:#f3aa44;font-weight:bold;color:white">when Button Click</span>

![Block](./Weeks/Week 2/images/w2_p1_block_whenButtonClick.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold">Button</span> drawer (with the name of your button) under <span style="font-weight:bold">UI Components.</span></span><br>
The <span style="background-color:#f3aa44;font-weight:bold;color:white">when Button Click</span> block is used to run the blocks within the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part when the button is clicked.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_6.png)
Now, we want to add functionality to the button we added for the user to submit a guess. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block.
---

# High Low - Part 1: Random Number Guesser
<span style="font-weight:bold">Block:</span> <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span>

![Block](./Weeks/Week 2/images/w2_p1_block_if.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#f3aa44">Control Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> block checks a statement and runs the block inside <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> if the statement is true. Think of it as: "If this statement is true, then do this."
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_7.png)
Connect the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block to perform an action based on a condition when the button is clicked.
---

# High Low - Part 1: Random Number Guesser
<span style="font-weight:bold">Block:</span> <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span>

![Block](./Weeks/Week 2/images/w2_p1_block_comparison.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#45b4a9">Logic Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block compares two values and returns True or False based on whether the condition is met. The comparison operator <span style="background-color:#b9e1dd;font-weight:bold">=</span> is used to check if two values are equal to one another and returns True if they are equal or False if they are not. Use the dropdown menu to select a different comparison operator, such as <span style="background-color:#b9e1dd;font-weight:bold"><</span> or <span style="background-color:#b9e1dd;font-weight:bold">></span>.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_8.png)
Connect the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> block to compare the user's guess to the answer.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_9.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block to the left side of the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block. The <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block retrieves the text that the user types into the text input component. This corresponds to the user’s guess.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_10.png)
Connect the <span style="background-color:#f87956;font-weight:bold;color:white">app variable answer</span> block to the right side of the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block. Now, we can compare the user’s guess from the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block to the answer that is stored in the <span style="background-color:#f87956;font-weight:bold;color:white">app variable answer</span> block.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_11.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Result's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> block. Replace "Label" with "Correct". We want the “Result” label to indicate that the guess is correct when it is equal to the answer.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #1: Correct Answer Check</span>]: Preview the app. See if the Result label indicates whether the guess is correct.<br>
If it works, the “Result” label will indicate whether the guess is correct, but there is no indication whether the guess is incorrect. When the guess is incorrect, we want the “Result” label to indicate whether the guess is too high or too low.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_13.png)
Click the plus icon next to <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> to add an <span style="background-color:#f3aa44;font-weight:bold;color:white">else if</span> section. The <span style="background-color:#f3aa44;font-weight:bold;color:white">else if</span> section will allow us to check another condition when the guess is not equal to the answer.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_14.png)
Connect the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">else if</span> section. This time, we will use the <span style="background-color:#b9e1dd;font-weight:bold"><</span> comparison operator.
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block to the left side of the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block and the <span style="background-color:#f87956;font-weight:bold;color:white">app variable answer</span> block to the right side of the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block.
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Result's Text to</span> block inside the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">else if</span> section.
Replace "Label" with "Too low".
We want the "Result" label to indicate that the guess is too low when it is lower than the answer.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #2: Too Low Logic</span>]: Preview the app. See if the "Result" label indicates whether the guess is too low.<br>
If it works, now the “Result” label will indicate whether the guess is correct or too low, but there is no indication whether the guess is too high. When the guess is too high, we want the “Result” label to indicate that the guess is too high.
---

# High Low - Part 1: Random Number Guesser
<span style="font-weight:bold">Block:</span> <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span>

![Block](./Weeks/Week 2/images/w2_p1_block_ifElse.png)

<span style="font-style:italic">This block can also be found in the <span style="font-weight:bold;color:#f3aa44">Control Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
In an <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block, the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part runs if the statement is true and the <span style="background-color:#f3aa44;font-weight:bold;color:white">else</span> part runs if the statement is false. Think of it as: "If this statement is true, then do this. Otherwise, do this instead."
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_16.png)
Click the plus icon next to <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> to add an <span style="background-color:#f3aa44;font-weight:bold;color:white">else</span> section. The <span style="background-color:#f3aa44;font-weight:bold;color:white">else</span> section will run when the guess is neither equal to nor lower than the answer.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_17.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Result's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">else</span> section. Replace "Label" with "Too high". Since we already checked when the guess is equal to or lower than the answer, the only possibility left is whether the guess is too high. There is no need to use the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block here, so we can simply add the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Result's Text to</span> block.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #3: Too High Logic</span>]: Preview the app. See if the "Result" label indicates whether the guess is too high.<br>
If it works, now the “Result” label will indicate whether the guess is correct, too low, or too high, but there is only one possible answer which was pre-set to 50 in Step 5. The number should be randomly chosen so the user won’t know what the answer is every time.
---

# High Low - Part 1: Random Number Guesser
<span style="font-weight:bold">Block:</span> <span style="background-color:#6789cc;font-weight:bold;color:white">random integer from [1] to [100]</span>

![Block](./Weeks/Week 2/images/w2_p1_block_randInt.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#6789cc">Math Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#6789cc;font-weight:bold;color:white">random integer from [1] to [100]</span> block returns a random integer within a specified range, inclusive of the provided integers.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_p1_19.png)
Replace the <span style="background-color:#6789cc;font-weight:bold;color:white">specify number</span> block with the <span style="background-color:#6789cc;font-weight:bold;color:white">random integer from [1] to [100]</span> block. We no longer want the answer to be pre-set, but rather a random number that will generate each time the app is opened.
---

# High Low - Part 1: Random Number Guesser
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #4: Random Number</span>]: Preview the app. See if the number is different each time.<br>
If it works, you now have a fully-functional random number guesser!
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_1.png)
In Part 2, we will create a real-time communication system. Two users will communicate: a Guesser makes guesses while a Clue Giver provides feedback.

In a new project, add a text input for the two users to type in their message. We will rename it to "Text_Input".
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_2.png)
Add a button for users to submit their message. We will rename it to "Submit".
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_3.png)
Add a label to display submitted messages. We will rename it to "Message".<br>
**Now, we will move onto blocks.**
---

# High Low - Part 2: Real-Time Updates
<span style="font-weight:bold">Block:</span> <span style="font-weight:bold;">Cloud Variable</span>

![Block](./Weeks/Week 2/images/w2_p2_block_initCloudVar.png)

Cloud variables allow you to store data in the cloud. This data can be accessed from multiple devices, which is suitable for data that your user may want to access from multiple devices.<br>
Remember, this is the same <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span> block introduced in Part 1. Use the dropdown menu to select the <span style="background-color:#f7c9bd;font-weight:bold">cloud</span> variable type.
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_4.png)
Create a cloud variable with the <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span> block. We will rename it to <span style="background-color:#f7c9bd;font-weight:bold">text</span>. We want to use a cloud variable instead of an app variable this time so that the data can be accessed from multiple devices.
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_5.png)
Now, we want to add functionality to the button we added for the users to submit a message. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block.
---

# High Low - Part 2: Real-Time Updates
<span style="font-weight:bold">Block:</span> <span style="background-color:#f87956;font-weight:bold;color:white">set variable to</span>

![Block](./Weeks/Week 2/images/w2_p2_block_setVarTo.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#f87956">Variables Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#f87956;font-weight:bold;color:white">set variable to</span> block allows you to set a variable to a value within a block event.
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_6.png)
Connect the <span style="background-color:#f87956;font-weight:bold;color:white">set variable to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block. We want the cloud variable <span style="background-color:#f7c9bd;font-weight:bold">text</span> to update when the "Submit" button is clicked.
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_7.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block to the <span style="background-color:#f87956;font-weight:bold;color:white">set variable to</span> block to set the cloud variable <span style="background-color:#f7c9bd;font-weight:bold">text</span> to the text written in Text_Input when the “Submit” button is clicked, since we want that information to be accessible across multiple devices.
---

# High Low - Part 2: Real-Time Updates
<span style="font-weight:bold">Block:</span> <span style="background-color:#f3aa44;font-weight:bold;color:white">when variable initializes or changes</span>

![Block](./Weeks/Week 2/images/w2_p2_block_whenVarChange.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#f87956">Variables Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span> after a variable has been created.</span><br>
You can use the <span style="background-color:#f3aa44;font-weight:bold;color:white">when variable initializes or changes</span> block to define how the app behaves when the variable initializes or changes.
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_8.png)
Add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when variable initializes or changes</span> block. We want changes to be made when the cloud variable <span style="background-color:#f7c9bd;font-weight:bold">text</span> is altered.
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_9.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Message's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when variable initializes or changes</span> block. We want the “Message” label to change whenever the cloud variable is altered.
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_p2_10.png)
Connect the <span style="background-color:#f87956;font-weight:bold;color:white">cloud variable text</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Message's Text to</span> block. We want the “Message” label to be populated with the information stored in the cloud variable <span style="background-color:#f7c9bd;font-weight:bold">text</span> so that the users can communicate with one another.
---

# High Low - Part 2: Real-Time Updates
![Setup](./Weeks/Week 2/images/w2_checkpoint.png)
[<span style="font-weight:bold">Checkpoint #5: Real-Time Updates</span>]: Preview the app. Check the functionality of real-time message display.<br>
If it works, you now have a fully-functional guessing game that two players can play on separate devices!
---

# High Low - Extension #1: Multiple Screens
[<span style="font-weight:bold">Extension #1: Multiple Screens</span>]

**Extension 1: Multiple Screens**

In this extension, you will create dedicated screens for the Guesser and Clue Giver.

Make a copy of your project from Part 2.

Have 3 screens total:
1. A home screen to choose your role
2. A Guesser screen for making guesses
3. A Clue Giver screen for providing feedback

Give the Guesser and Clue Giver the components needed to input text on their respective screens.

<span style="font-weight:bold">Block:</span> <span style="background-color:#f3aa44;font-weight:bold;color:white">navigate to</span>

![Block](./Weeks/Week 2/images/w2_ext1_block_navigateTo.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#f3aa44">Control Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#f3aa44;font-weight:bold;color:white">navigate to</span> block takes the user to the defined screen.

Add the blocks for the Guesser and Clue Giver to communicate with each other using cloud variables.

Preview the app. Test that you can navigate between screens and that communication works between the Guesser and Clue Giver screens.
