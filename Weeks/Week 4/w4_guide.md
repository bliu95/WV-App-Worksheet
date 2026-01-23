# Quiz App - Simple Quiz
Your goal is to build a quiz app. Users should be able to see questions, provide an answer, check if the answer is correct, and move on to the next question.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_1.png)
Create a local data source that has the questions and answers for your quiz. Rename the column containing the questions to "Questions" and rename the column containing the answers to "Answers".
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_2.png)
Add a label to display a question. We will rename it to "Question".
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_3.png)
Add a text input for users to type in an answer. We will rename it to "Text_Input".
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_4.png)
Add a button for users to submit an answer. We will rename it to "Submit".
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_5.png)
Add a label to indicate whether the user's answer was correct or incorrect. We will rename it to "Result".<br>
**Now, we will move onto blocks.**
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_6.png)
Create a variable with the <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span> block to keep track of which question the user is on. We will rename it to <span style="background-color:#f7c9bd;font-weight:bold">questionNumber</span>.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_7.png)
Set the variable <span style="background-color:#f7c9bd;font-weight:bold">questionNumber</span> to 1 by connecting the <span style="background-color:#6789cc;font-weight:bold;color:white">specify number</span> block to the <span style="background-color:#f87956;font-weight:bold;color:white">initialize variable to</span> block and setting it to <span style="background-color:#c2d0eb;font-weight:bold">1</span>.
---

# Quiz App - Simple Quiz
<span style="font-weight:bold">Block:</span> <span style="background-color:#f3aa44;font-weight:bold;color:white">when Screen Opens</span>

![Block](./Weeks/Week 4/images/w4_block_whenScreenOpens.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold">Screen</span> drawer (with the name of your screen) under <span style="font-weight:bold">UI Components.</span></span><br>
The <span style="background-color:#f3aa44;font-weight:bold;color:white">when Screen Opens</span> block is used to run the blocks within the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> section when the screen is opened.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_8.png)
We want the first question to show up on the screen when the user starts the app. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Screen1 Opens</span> block.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_9.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Question's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Screen1 Opens</span> block. We want the "Question" label to be populated with the first question in the quiz when the app starts.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_10.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">get value from</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Question's Text to</span> block. Make sure the column whose value is being retrieved is <span style="background-color:#c7bedc;font-weight:bold">Questions</span>. We want the "Question" label to be populated with a question retrieved from the data source.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_11.png)
Connect the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">get value from</span> block. From the data source, we want to retrieve the question with the row id corresponding to the question that the user is on, which is being tracked with the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> block.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #1: Display First Question]</span><br>
Preview the app. See if the "Question" label displays the first question from the data source when the app starts.<br>
If it works, the "Question" label will function as expected, but there is no other functionality for the app. We want the user to be able to submit an answer and get an indication of whether their answer is correct or not.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_13.png)
Now, we want to add functionality to the button we added for the user to submit an answer. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_14.png)
Connect the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block to perform an action based on two conditions when the button is clicked: (1) when the answer is correct and (2) when the answer is incorrect.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_15.png)
Connect the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. We want to use it to compare the user's answer to the correct answer.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_16.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block to the left side of the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block. This corresponds to the user's answer.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_17.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">get value from</span> block to the right side of the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block. Make sure the column whose value is being retrieved is <span style="background-color:#c7bedc;font-weight:bold">Answers</span>. We want to compare the user's answer with the correct answer that is retrieved from the data source.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_18.png)
Connect the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">get value from</span> block. From the data source, we want to retrieve the correct answer with the row id corresponding to the question that the user is on, which is being tracked with the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> block.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_19.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Result's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. Replace "Label" with "Correct". We want the "Result" label to indicate that the user's answer is correct when it is equal to the correct answer.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_20.png)
Connect another <span style="background-color:#3f9e83;font-weight:bold;color:white">set Result's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">else</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. Replace "Label" with "Incorrect". Since we already checked when the user's answer is correct, the only possibility left is whether the user's answer is incorrect. There is no need to use the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block here, so we can simply add the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Result's Text to</span> block.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #2: Answer Validation]</span><br>
Preview the app. See if the "Result" label accurately indicates when an answer is correct and when an answer is incorrect.<br>
If it works, the "Result" label will function as expected, but the quiz will not move onto the next question. Also, the answer that the user typed remains in Text_Input.
---

# Quiz App - Simple Quiz
<span style="font-weight:bold">Block:</span> <span style="background-color:#f87956;font-weight:bold;color:white">change variable by</span>

![Block](./Weeks/Week 4/images/w4_block_changeVariableBy.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#f87956">Variables Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#f87956;font-weight:bold;color:white">change variable by</span> block incrementally changes the variable by the defined number. In this case, the variable <span style="background-color:#f7c9bd;font-weight:bold">name</span> increases by 1 every time this block is run.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_22.png)
Connect the <span style="background-color:#f87956;font-weight:bold;color:white">change variable by</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block. We want the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> to increase by 1 every time the user has answered a question.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_23.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Question's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block. Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">get value from</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Question's Text to</span> block. Make sure the column whose value is being retrieved is <span style="background-color:#c7bedc;font-weight:bold">Questions</span>. Connect the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">get value from</span> block. We want the "Question" label to update to the next question after one question has been answered.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_24.png)
To clear the text in Text_Input, connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Text_Input's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block. Make sure that the text remains blank. This will reset Text_Input when the "Question" label is updated.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #3: Advance to Next Question]</span><br>
Preview the app. Check that when the answer is correct, the user sees the next question and what the user types in Text_Input clears after each question.<br>
If it works, now you can see all the questions in the quiz; however, once you have answered the last question, you will see that the app tries to show a question that does not exist by filling in the "Question" label with "null". We should end the quiz after the last question has been answered.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_26.png)
Connect another <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block to perform an action based on two conditions when the button is clicked: (1) when the user has not yet reached the last question and (2) when the user has reached the last question.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_27.png)
Connect the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block with the <span style="background-color:#b9e1dd;font-weight:bold"><</span> comparison operator to the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. We want to use it to compare the question that the user is on and the total number of questions in the quiz.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_28.png)
Connect the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> block to the left side of the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block. This corresponds to the question that the user is on.
---

# Quiz App - Simple Quiz
<span style="font-weight:bold">Block:</span> <span style="background-color:#735ca5;font-weight:bold;color:white">number of rows in</span>

![Block](./Weeks/Week 4/images/w4_block_numberOfRowsIn.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Data Sources Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">number of rows in</span> block returns an integer corresponding to how many rows are in a given data source.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_29.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">number of rows in</span> block to the right side of the <span style="background-color:#45b4a9;font-weight:bold;color:white">comparison</span> block. Now, we can compare the question that the user is on from the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> block with the total number of questions in the quiz that is retrieved from the <span style="background-color:#735ca5;font-weight:bold;color:white">number of rows in</span> block.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_30.png)
Now, we can move the <span style="background-color:#f87956;font-weight:bold;color:white">change variable by</span> block, the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Question's Text to</span> block, and the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Text_Input's Text to</span> block into the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. We do want to make sure that the 3 blocks do not run once the last question in the quiz has been answered, i.e., when the <span style="background-color:#f87956;font-weight:bold;color:white">app variable questionNumber</span> is equal to the total number of questions in the quiz that is retrieved from the <span style="background-color:#735ca5;font-weight:bold;color:white">number of rows in</span> block.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_31.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Question's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">else</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. Replace "Label" with "The quiz is over". We want the "Question" label to indicate when the user has reached the end of the quiz.
---

# Quiz App - Simple Quiz
![Setup](./Weeks/Week 4/images/w4_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #4: End of Quiz]</span><br>
Preview the app. Check that the user can't go past the last question.<br>
If it works, you now have a fully-functional quiz app!
---

# Simple Quiz - Extension #1: Ignoring Answer Capitalization
<span style="font-weight:bold">[Extension #1: Ignoring answer capitalization]</span><br>
If the user types in an answer, but it's not capitalized exactly as the correct answer in the data source, it will be marked as incorrect. Change the blocks so that the answer can be correct, regardless of the capitalization.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#df6078;font-weight:bold;color:white">set case</span></div><img src="./Weeks/Week 4/images/w4_ext1_setCase.png" alt="Block: set case"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#df6078">Text Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#df6078;font-weight:bold;color:white">set case</span> block sets a piece of text to the selected case and returns the reformatted text. There are 3 letter case options: UPPER CASE, lower case, and Title Case.</div></div>
---

# Simple Quiz - Extension #2: Track Number of Correct Answers
<span style="font-weight:bold">[Extension #2: Track number of correct answers]</span><br>
Use another variable to track how many questions the user has answered correctly, and display the score on the screen.
---

# Simple Quiz - Extension #3: Questions in Random Order
<span style="font-weight:bold">[Extension #3: Questions in random order]</span><br>
Have the questions in the quiz appear in a random order.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#75afc8;font-weight:bold;color:white">shuffle list</span></div><img src="./Weeks/Week 4/images/w4_ext3_block_shuffleList.png" alt="Block: shuffle list"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#75afc8">Lists Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#75afc8;font-weight:bold;color:white">shuffle list</span> block generates a copy of a list with the items shuffled in a random order.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#75afc8;font-weight:bold;color:white">in list get</span></div><img src="./Weeks/Week 4/images/w4_ext3_block_inListGet.png" alt="Block: in list get"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#75afc8">Lists Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#75afc8;font-weight:bold;color:white">in list get</span> block allows you to get an item in a specified index or position from a list.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">list of values in</span></div><img src="./Weeks/Week 4/images/w4_ext3_block_listOfValuesIn.png" alt="Block: list of values in"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Data Sources Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">list of values in</span> block allows you to read an entire column of data from a table and returns it as a list you can then manipulate with the List Blocks.</div></div>
---

# Simple Quiz - Extension #4: Multiple Choice
<span style="font-weight:bold">[Extension #4: Multiple Choice]</span><br>
Instead of the user typing in the correct answer, have them select between multiple possible answers. You may want to put all the possible answers in the data table, and have a column to indicate the correct answer. You should make a new project for this extension.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">get row object from</span></div><img src="./Weeks/Week 4/images/w4_ext4_block_getRowObject.png" alt="Block: get row object from"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Data Sources Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">get row object from</span> block returns the row object of the specified row id. The row object can be used with Object Blocks.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#f89da2;font-weight:bold;color:white">get property of object</span></div><img src="./Weeks/Week 4/images/w4_ext4_block_getPropertyOfObject.png" alt="Block: get property of object"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#f89da2">Objects Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#f89da2;font-weight:bold;color:white">get property of object</span> block allows you to read the value of an object's property. If the object does not have a property with this name, it will return "undefined".</div></div>
---

# Simple Quiz - Extension #4.5: Multiple Choice with Functions
<span style="font-weight:bold">[Extension #4.5: Multiple Choice with Functions]</span><br>
**Prerequisite:** If you have not done Extension #4 and created a multiple-choice quiz, please do so first before doing this extension.<br>
A function is a block of code that performs a specific task. If you use the same code set multiple times in your project, you can work more efficiently using functions. In this extension, you will practice using functions.<br>
First, make a copy of your project containing a quiz app with multiple-choice questions. Now, use functions to reduce as many repetitive blocks as possible.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">create function</span></div><img src="./Weeks/Week 4/images/w4_ext4.5_block_createFunction.png" alt="Block: create function"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Functions Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
This block is used to create a function. Replace do something with a clear function name. Clear function names can help make your code more readable.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">run function</span></div><img src="./Weeks/Week 4/images/w4_ext4.5_block_runFunction.png" alt="Block: run function"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Functions Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span> after a function has been created.</span><br>
Once you have created your function, you can use it at any time using the function block you have named.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">create function with inputs</span></div><img src="./Weeks/Week 4/images/w4_ext4.5_block_createFunctionWithInputs.png" alt="Block: create function with inputs"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Functions Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
Pressing the plus icon in the block used to create a function would add an input variable. You can then treat that input as a local variable in your function, meaning it can only be used from within the function. There can be multiple input variables for one function.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">run function with inputs</span></div><img src="./Weeks/Week 4/images/w4_ext4.5_block_runFunctionWithInputs.png" alt="Block: run function with inputs"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Functions Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span> after a function with inputs has been created.</span><br>
This time, in order to use the function, you must also provide the input variables that the function block calls for.</div></div>
