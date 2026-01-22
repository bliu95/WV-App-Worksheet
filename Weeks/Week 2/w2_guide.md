# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_1.png)
Add a <span style="background-color:#90ee90">text input</span> component to the screen. Rename it to <span style="font-style: italics">Text_Input</span>. This will be used for users to type in a guess.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_2.png)
Add a <span style="background-color:#90ee90">button</span> for guess submission. Rename it to <span style="font-style: italics">Submit</span>.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_3.png)
Add a <span style="background-color:#90ee90">label</span> to display results. Rename it to <span style="font-style: italics">Result</span>. This will tell the user if the guess was correct, too high, or too low.
---

# High Low - Part 1
Now, we will move onto blocks.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_4.png)
Create an app variable using the <span style="background-color:coral">initialize variable</span> block. Name it <span style="font-style: italics">answer</span>. This will store the correct answer.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_5.png)
Add a <span style="background-color:coral">specify number</span> block and connect it with the <span style="background-color:coral">initialize variable</span> block. Set it to 50 as a temporary preset value.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_6.png)
Click the Submit button under <span style="font-style: italics">UI Components</span>. Add a <span style="background-color:#ffce42">When Submit Click</span> block.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_7.png)
Add an <span style="background-color:#ffce42">if</span> block and connect it inside the <span style="background-color:#ffce42">When Submit Click</span> block.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_8.png)
Add a <span style="background-color:#20b2aa">comparison</span> block and connect it with the <span style="background-color:#ffce42">if</span> block.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_9.png)
Add the <span style="background-color:#90ee90">Text_Input's Text</span> block to the left side of the <span style="background-color:#20b2aa">comparison</span> block.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_10.png)
In the <span style="background-color:coral">variable</span> drawer, add and connect the <span style="font-style: italics">answer</span> variable to the right side of the <span style="background-color:#20b2aa">comparison</span> block.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_11.png)
Add a <span style="background-color:#3cb371">set Result's Text</span> block and connect it inside the <span style="background-color:#ffce42">if</span> block's do section.

Change the text to "Correct".
---

# High Low - Part 1
[<span style="font-weight:bold">Checkpoint #1: Correct Answer Check</span>]: Preview the app. Type in 50 (the answer). Verify that the label shows "Correct".
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_13.png)
Press the <span style="font-weight:bold">+</span> button on the top left of the <span style="background-color:#ffce42">if</span> block to add an <span style="font-style: italics">else-if</span> section.
---

# High Low - Part 1
Add a <span style="background-color:#20b2aa">comparison</span> block and connect it with the <span style="background-color:#ffce42">else-if</span> section.

Click the <span style="font-weight:bold">=</span> sign and change it to <span style="font-weight:bold"><</span> (less than).
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_14.png)
Add <span style="background-color:#90ee90">Text_Input's Text</span> to the left side and the <span style="font-style: italics">answer</span> variable to the right side of the <span style="background-color:#20b2aa">less than</span> block.
---

# High Low - Part 1
Add a <span style="background-color:#3cb371">set Result's Text</span> block inside the else-if section.

Change the text to "Too low".
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_17.png)
This is what your blocks should look like now.
---

# High Low - Part 1
[<span style="font-weight:bold">Checkpoint #2: Too Low Logic</span>]: Preview the app. Type in a guess lower than 50. Verify that the label shows "Too low".
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_19.png)
Press the <span style="font-weight:bold">+</span> button on the right of the <span style="font-style: italics">do</span> section to add an <span style="font-style: italics">else</span> section.
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_20.png)
Add a <span style="background-color:#3cb371">set Result's Text</span> block inside the else section.

Change the text to "Too high".
---

# High Low - Part 1
[<span style="font-weight:bold">Checkpoint #3: Too High Logic</span>]: Preview the app. Type in a guess higher than 50. Verify that the label shows "Too high".
---

# High Low - Part 1
![Setup](./Weeks/Week 2/images/w2_p1_22.png)
Replace the <span style="background-color:coral">specify number</span> block (50) with a <span style="background-color:#4682b4">random integer from 1 to 100</span> block.
---

# High Low - Part 1
[<span style="font-weight:bold">Checkpoint #4: Random Number</span>]: Preview the app multiple times. Verify that the answer is different each time by testing your guesses.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_1.png)
In Part 2, we will create a real-time communication system. Two users will communicate: a Guesser makes guesses while a Clue Giver provides feedback.

Start by adding a <span style="background-color:#90ee90">text input</span> component. Rename it to <span style="font-style: italics">Text_Input</span>.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_2.png)
Add a <span style="background-color:#90ee90">button</span> for submitting messages. Rename it to <span style="font-style: italics">Submit</span>.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_3.png)
Add a <span style="background-color:#90ee90">label</span> for displaying messages. Rename it to <span style="font-style: italics">Message</span>.
---

# High Low - Part 2
Now, we will move onto blocks using cloud variables.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_4.png)
Create a <span style="background-color:#9370db">cloud variable</span> named <span style="font-style: italics">text</span>. Cloud variables allow data to be shared across devices in real-time.

**Important:** Use a cloud variable, not an app variable!
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_5.png)
Add a <span style="background-color:#ffce42">When Submit Click</span> block.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_6.png)
Add a <span style="background-color:#9370db">set cloud variable</span> block inside the When Submit Click block.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_7.png)
Connect <span style="background-color:#90ee90">Text_Input's Text</span> to the <span style="background-color:#9370db">set cloud variable</span> block. This will save the typed text to the cloud.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_8.png)
Add a <span style="background-color:#9370db">when cloud variable initializes or changes</span> block. This triggers whenever the cloud variable updates.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_9.png)
Add a <span style="background-color:#3cb371">set Message's Text</span> block inside the when cloud variable changes block.
---

# High Low - Part 2
![Setup](./Weeks/Week 2/images/w2_p2_10.png)
Connect the <span style="background-color:#9370db">cloud variable text</span> block to the <span style="background-color:#3cb371">set Message's Text</span> block.
---

# High Low - Part 2
[<span style="font-weight:bold">Checkpoint #5: Real-Time Updates</span>]: Preview the app on two devices or browser tabs. Type a message and submit. Verify that the message appears on both screens.
---

# High Low - Extension 1
![Setup](./Weeks/Week 2/images/w2_ext1_1.png)
**Extension 1: Multiple Screens**

In this extension, you will create dedicated screens for the Guesser and Clue Giver.

Start by copying your Part 2 project.
---

# High Low - Extension 1
![Setup](./Weeks/Week 2/images/w2_ext1_2.png)
Create 3 screens total:
1. A home screen to choose your role
2. A Guesser screen for making guesses
3. A Clue Giver screen for providing feedback
---

# High Low - Extension 1
![Setup](./Weeks/Week 2/images/w2_ext1_3.png)
Use the <span style="background-color:#ffce42">navigate to</span> block to direct users to the appropriate screen based on their role selection.
---

# High Low - Extension 1
![Setup](./Weeks/Week 2/images/w2_ext1_4.png)
Add communication blocks between screens so the Guesser and Clue Giver can interact in real-time using cloud variables.
---

# High Low - Extension 1
[<span style="font-weight:bold">Checkpoint #6: Multiple Screens</span>]: Preview the app. Test that you can navigate between screens and that communication works between the Guesser and Clue Giver screens.
