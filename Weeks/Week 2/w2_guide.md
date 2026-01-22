# High Low
![Setup](./Weeks/Week 2/images/w2_p1_1.png)
Start with adding a text input to the screen. This will be used for users to type in a guess
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_2.png)
Add a button. This will be used to submit.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_3.png)
Add a label. This will be used to tell the user if the guess they submitted was too high or too low.
---

# High Low
Now, we will move onto blocks.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_4.png)
Create a variable by using the <span style="background-color:coral">intialize variable</span> block. Give it a name that reflects the purpose of the variable. In this example, we will call it <span style="font-style: italics">answer</span>
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_5.png)
Add number and connect it with the <span style="background-color:coral">intialize variable</span> block. This will set the default value of the variable to that number. Type in any number. For this example, we will type in 50.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_6.png)
Now click the button you added earlier under <span style="font-style: italics">UI Components</span>. Add a <span style="background-color:#ffce42">When Button Click</span> block. Because we named our button <span style="font-style: italics">submit</span>, the block will say <span style="background-color:#ffce42">When Submit Click</span>.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_7.png)
Add an <span style="background-color:#ffce42">if</span> block and connect it inside the <span style="background-color:#ffce42">When Submit Click</span> block. 
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_8.png)
Add an <span style="background-color:#20b2aa">equals</span> block and connect it with the <span style="background-color:#ffce42">if</span> block.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_9.png)
Add and put <span style="background-color:#90ee90">Text Input's Text</span> block to one side of the <span style="background-color:#20b2aa">equals</span> block. In this example, we will put it on the left side.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_10.png)
In the <span style="background-color:coral">variable</span> drawer, add and connect the <span style="font-style: italics">answer</span> variable to the remaining empty slot in the <span style="background-color:#20b2aa">equals</span> block. 
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_11.png)
Add a <span style="background-color:#3cb371">set label's text</span> block and connect it inside the <span style="background-color:#ffce42">if</span> block.

Change the default text that comes with the <span style="background-color:#3cb371">set label's text</span> block from "Label" to "Correct".
---

# High Low
[<span style="font-weight:bold">Checkpoint #1: Setup & Correct Answer</span>]: Preview your app Preview the app. Type in the answer. See if it indicates whether the answer is correct.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_13.png)
Press the <span style="font-weight:bold">+</span> button on top left of the <span style="background-color:#ffce42">if</span> block. This will add an <span style="font-style: italics">else-if</span> to the block.
---

# High Low
Now we are going to add another set of blocks that are almost identical. It should be almost a repeat of the blocks you just added.

Start with adding an <span style="background-color:#20b2aa">equals</span> block and connect it with the <span style="background-color:#ffce42">if</span> block.

Click the <span style="font-weight:bold">=</span> sign in the <span style="background-color:#20b2aa">equals</span> block. Change it to a <span style="font-weight:bold"><</span> sign
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_13.png)
Add and put <span style="background-color:#90ee90">Text Input's Text</span> block to one side of the <span style="background-color:#20b2aa">less than</span> block. In this example, we will put it on the left side.

In the <span style="background-color:coral">variable</span> drawer, add and connect the <span style="font-style: italics">answer</span> variable to the remaining empty slot in the <span style="background-color:#20b2aa">less than</span> block. 
---

# High Low
Add a <span style="background-color:#3cb371">set label's text</span> block and connect it inside the <span style="background-color:#ffce42">if</span> block.

Change the default text that comes with the <span style="background-color:#3cb371">set label's text</span> block from "Label" to "Too low".
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_17.png)
This is what your blocks should look like now.
---

# High Low
[<span style="font-weight:bold">Checkpoint #2: Too Low Logic</span>]: Preview your app Preview the app. Type in a guess that is lower than the answer. Check to see if the label shows "Too low".
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_19.png)
Press the <span style="font-weight:bold">+</span> button on the right of the <span style="font-style: italics">do</span> section of the <span style="background-color:#ffce42">if</span> block. This will add an <span style="font-style: italics">else</span> to the block.
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_20.png)
Add a <span style="background-color:#3cb371">set label's text</span> block and connect it inside the <span style="background-color:#ffce42">if</span> block.

Change the default text that comes with the <span style="background-color:#3cb371">set label's text</span> block from "Label" to "Too high".
---

# High Low
[<span style="font-weight:bold">Checkpoint #3: Too High Logic</span>]: Preview your app Preview the app. Type in a guess that is higher than the answer. Check to see if the label shows "Too high".
---

# High Low
![Setup](./Weeks/Week 2/images/w2_p1_22.png)
Lastly, replace the number that connect with your variable that holds the correct answer to the <span style="background-color:#4682b4">random integar text</span> 
---

# High Low
[<span style="font-weight:bold">Checkpoint #4: Random Number</span>]: Preview the app. See if the number is different each time when you preview the app.