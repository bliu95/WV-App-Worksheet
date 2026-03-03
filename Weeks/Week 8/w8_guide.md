# AI Story App
Your goal is to build an app where OpenAI will create a multiple-choice story based on a user's story idea and complete the story based on the user's selected ending choice.<br>
Begin your project by duplicating this [project template](https://x.thunkable.com/projects/697bfe9356673573f9be93cf/aec9c6b9-bb97-412c-8b67-02bbfdb6e014/designer). The project is completely empty besides a block that you will use to access the LLM. If you experience any issues with accessing or duplicating the template, please speak with your teacher.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_1.png)
Add in a text input for users to type in a story idea. We will rename it to “Idea Input”. In the properties panel, you may optionally change the **Hint** from “Type here” to “What kind of story do you want?” to be clear for users.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_2.png)
Add a button for users to submit the story idea. We will rename it to “Submit Idea”. In the properties panel, replace the default value “Button” with “Generate Story”.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_3.png)
Add a layout to the screen, then do the following:
1. Delete Container1 and Container2 from the layout.
2. In the layout's properties panel, enable **Scrollable**.
3. Resize the layout to your desired size.
We are setting up to create a scrollable label using this layout.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_4.png)
Add a label inside the layout to display the response from the LLM. We will rename it to “Story”. Now do the following:
1. Change the **Width** and **Height** of the label to “Fill container”. We want the label to fit within the layout.
2. Clear the default text “Label” so the label is blank before the LLM returns a response.
**Now, we will move onto blocks.**
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_5.png)
There is already the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block on the screen. We will need this block to enable communication between the user and the LLM. It is currently grayed out because it is not connected to any blocks.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_6.png)
We want to add functionality to the button we added for the user to submit a prompt. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Idea Click</span> block.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_7.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Story's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Idea Click</span> block. We want “Story” to update after the user clicks the “Submit Idea” button.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_8.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Story's Text to</span> block. We want “Story” to display the output from the LLM after the user has submitted a prompt.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_9.png)
Connect the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">Prompt</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block. We will now prepare the prompt that will be sent to the LLM.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_10.png)
In the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block, do the following:
1. Replace the text in the top <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with “Create a one-paragraph multiple choice story with the idea provided below. The story will have three choices: A, B, or C, and make sure the choices are labeled with A, B, and C. The idea is: ”.
2. Delete and replace the bottom <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with the <span style="background-color:#70ce9c;font-weight:bold;color:white">Idea Input's Text</span> block.
We want the LLM to create a short multiple choice story using the user's story idea.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #1: Verify Story Generation]</span><br>
Preview the app. Check that the LLM generates a short multiple choice story using the idea submitted by the user.<br>
If it works, the “Story” label should display the output from the LLM which contains a short story and 3 choices for continuing the story. Now, make it possible for the user to select a choice and have the LLM complete the story based on the selected choice.<br>
**Let's move to the Design tab.**
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_12.png)
Add 3 buttons: one for choice A, one for choice B, and one for choice C. We will rename them to “ChoiceA”, “ChoiceB”, and “ChoiceC” respectively, and change the default value “Button” to “A”, “B”, and “C” respectively. Resize and rearrange the buttons so that they appear side-by-side.<br>
**Now, we will move onto blocks.**
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_13.png)
For each button, we will repeat the same steps. The only difference will be the prompt given to the LLM to indicate the selected choice. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when ChoiceA Click</span> block.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_14.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Story's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when ChoiceA Click</span> block. We want “Story” to update after the user clicks the “ChoiceA” button.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_15.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Story's Text to</span> block. We want “Story” to display the output from the LLM after the user has submitted a prompt.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_16.png)
Connect the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">Prompt</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block. Now do the following:
1. Replace the text in the top <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with “The user’s choice is A. Please use the indicated choice to finish up the story below: ”.
2. Delete and replace the bottom <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with the <span style="background-color:#70ce9c;font-weight:bold;color:white">Story's Text</span> block.
We want the LLM to finish up the story using the choice A ending.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #2: Test Choice A]</span><br>
Preview the app. Check that the LLM generates an ending based on the choice A option.<br>
If it works, the “Story” label should display the output from the LLM which contains the ending of the story based on choice A. Now, we will repeat the process for the Choice B.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_18.png)
Repeat the steps for Choice B:
1. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when ChoiceB Click</span> block.
2. Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Story's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when ChoiceB Click</span> block. We want “Story” to update after the user clicks the “ChoiceB” button.
3. Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Story's Text to</span> block. We want “Story” to display the output from the LLM after the user has submitted a prompt.
4. Connect the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">Prompt</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block. Replace the text in the top <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with “The user’s choice is B. Please use the indicated choice to finish up the story below: ”. Delete and replace the bottom <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with the <span style="background-color:#70ce9c;font-weight:bold;color:white">Story's Text</span> block.
We want the LLM to finish up the story using the choice B ending.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #3: Test Choice B]</span><br>
Preview the app. Check that the LLM generates an ending based on the choice B option.<br>
If it works, the “Story” label should display the output from the LLM which contains the ending of the story based on choice B. Now, we will repeat the process for Choice C.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_20.png)
Repeat the steps for Choice C:
1. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when ChoiceC Click</span> block.
2. Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Story's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when ChoiceC Click</span> block. We want “Story” to update after the user clicks the “ChoiceC” button.
3. Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Story's Text to</span> block. We want “Story” to display the output from the LLM after the user has submitted a prompt.
4. Connect the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">Prompt</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block. Replace the text in the top <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with “The user’s choice is C. Please use the indicated choice to finish up the story below: ”. Delete and replace the bottom <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block with the <span style="background-color:#70ce9c;font-weight:bold;color:white">Story's Text</span> block.
We want the LLM to finish up the story using the choice C ending.
---

# AI Story App
![Setup](./Weeks/Week 8/images/w8_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #4: Test Choice C]</span><br>
Preview the app. Check that the LLM completes the story based on the choice ending selected by the user.<br>
If it works, you now have an app that allows users to generate a short multiple choice story using LLMs!
---

# AI Story App - Extension #1: Story Log
<span style="font-weight:bold">[Extension #1: Story Log]</span><br>
Now, let’s add the ability to save the stories that the user generates. You may want to add a new screen to show the story log.<br>
Starting with:
1. Create a data source to store the story details.
2. Add the generated story in the data source.
3. After the user selects an ending choice, update the story in the data source to include the generated ending.
    a. You can either have an additional column to store the ending or combine the story and the ending in the same column.
    b. A variable would be helpful to keep track of the <span style="background-color:#70ce9c;font-weight:bold;color:white">row id</span> to reference the row in the data source that must be updated.
4. Add a new screen to display the story log in a Data Viewer List (e.g., **Story Log Screen**).

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">update value in</span></div><img src="./Weeks/Week 8/images/w8_ext1_block_updateValue.png" alt="Block: update value in"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Data Sources Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span>.</span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">update value in</span> block allows you to modify or update an existing cell in your data source. The column name and view are specified in the block itself. The **row id** and new **value** are passed as inputs.</div></div>
---

# AI Story App - Extension #2: View Individual Saved Story
<span style="font-weight:bold">[Extension #2: View Individual Saved Story]</span><br>
It is likely that you cannot view the entire contents of the story log in the Data Viewer List. Now, let’s allow users to view individual stories that are saved in the story log. You may want to add a new screen to display the contents of the selected story to be viewed.<br>
Starting with:
1. Add a new screen to display the contents of an individual saved story (e.g., **Story View Screen**).
2. On the new screen, add labels to hold the information for a single row in the data source, i.e., an individual saved story.
3. On the **Story Log Screen**, add blocks to identify the selected item in the Data Viewer List, which would be used to populate the labels on the **Story View Screen** based on the selected item.
    a. A variable would be helpful to keep track of the <span style="background-color:#70ce9c;font-weight:bold;color:white">row id</span> to reference the selected item from the Data Viewer List. 
    b. Don't forget to add blocks to navigate to the **Story View Screen**!
4. On the **Story View Screen**, add blocks to retrieve data from a single row in the data source based on the selected item from the Data Viewer List.
    a. **Hint:** You may use either the <span style="background-color:#735ca5;font-weight:bold;color:white">get row object from</span> + <span style="background-color:#f89da2;font-weight:bold;color:white">get property of object</span> blocks combination (highly-recommended method) or multiple <span style="background-color:#735ca5;font-weight:bold;color:white">get value from</span> blocks to retrieve data, as covered in Week 4.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">get row object from</span></div><img src="./Weeks/Week 8/images/w8_ext2_block_getRowObject.png" alt="Block: get row object from"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Data Sources Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span>.</span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">get row object from</span> block returns the row object of the specified **row id**. The row object can be used with the **Object Blocks**.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#f89da2;font-weight:bold;color:white">get property of object</span></div><img src="./Weeks/Week 8/images/w8_ext2_block_getPropertyOfObject.png" alt="Block: get property of object"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#f89da2">Objects Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span>.</span><br>
The <span style="background-color:#f89da2;font-weight:bold;color:white">get property of object</span> block allows you to read the value of an object's property. If the object does not have a property with this name, it will return “undefined”.</div></div>