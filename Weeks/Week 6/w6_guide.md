# Historical Figures
Your goal is to create an app where users can communicate with a “historical figure” through LLMs. Users should be able to send a message and get a response from the LLM.<br>
Begin your project by duplicating this [project template](https://x.thunkable.com/projects/697bfe9356673573f9be93cf/aec9c6b9-bb97-412c-8b67-02bbfdb6e014/designer). The project is completely empty besides a block that you will use to access the LLM. If you experience any issues with accessing or duplicating the template, please speak with your teacher.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_1.png)
Add a text input for users to type in a message to submit to the LLM. We will rename it to “Prompt Input”.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_2.png)
Add a button to submit the message to the LLM. We will rename it to “Submit Prompt”. In the properties panel, replace the default value “Button” with “Submit Prompt”.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_3.png)
Add a layout to the screen, then do the following:
1. Delete Container1 and Container2 from the layout.
2. In the layout's properties panel, enable **Scrollable**.
3. Resize the layout to your desired size.
We are setting up to create a scrollable label using this layout.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_4.png)
Add a label inside the layout to display the response from the LLM. We will rename it to “Response”. Now, do the following:
1. Change the **Width** and **Height** of the label to “Fill container”. We want the label to fit within the layout.
2. Clear the default text “Label” so the label is blank before the LLM returns a response.
**Now, we will move onto blocks.**
---

# Historical Figures
<span style="font-weight:bold">Block:</span> <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span>

![Block](./Weeks/Week 6/images/w6_block_callOpenAITextComplete.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Open AI</span> drawer under <span style="font-weight:bold">Logic Modules</span> in the project template.</span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block takes in a text <span style="background-color:#735ca5;font-weight:bold;color:white">Prompt</span> for OpenAI to generate text around and will produce either a **response** or an **error**. A **response** is the generated text from the LLM answering the <span style="background-color:#735ca5;font-weight:bold;color:white">Prompt</span>. An **error** is the specific explanation for when an issue has occurred.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_5.png)
There is already the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block on the screen. We will need this block to enable communication between the user and the LLM. It is currently grayed out because it is not connected to any blocks.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_6.png)
Now, we want to add functionality to the button we added for the user to submit a message to the LLM. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Prompt Click</span> block.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_7.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Response's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Prompt Click</span> block. We want the “Response” label to update when the “Submit Prompt” button is clicked.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_8.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Response's Text to</span> block. We want the response from the LLM to be displayed in the “Response” label.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_9.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Prompt Input's Text</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">Prompt</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block. We want the LLM to receive and respond to the text that the user submits.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #1: Basic LLM Response]</span><br>
Preview the app. Check that the LLM produces a response to the text submitted by the user. You may need to wait a few seconds before there is a response. If there is an error message, you may need to speak with your teacher to figure out the issue.<br>
If it works, the “Response” label should display a response to the text submitted by the user. Next, we want the LLM to communicate as a historical figure.<br>
**Let's move to the Design tab.**
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_11.png)
Add a label to display the name of the historical figure. We will rename it to “Historical Figure”. In the properties panel, replace the default value “Label” with “Shakespeare”.<br>
**Now, we will move onto blocks.**
---

# Historical Figures
<span style="font-weight:bold">Block:</span> <span style="background-color:#df6078;font-weight:bold;color:white">join</span>

![Block](./Weeks/Week 6/images/w6_block_join.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#df6078">Text Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span>.</span><br>
The <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block is used to join text values together. In this case, the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> blocks each containing “hello ” and “world” are joined together to be a single text value: “hello world”. Spaces are not automatically added, so they must be typed into the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> blocks when necessary, such as in “hello ”. Other blocks containing text values, such as a variable or a component's text, may be connected to this block.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_12.png)
Replace the <span style="background-color:#70ce9c;font-weight:bold;color:white">Prompt Input's Text</span> block with the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block in the <span style="background-color:#735ca5;font-weight:bold;color:white">Prompt</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block. We want to add more information to the prompt given to the LLM so that it can communicate like a historical figure.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_13.png)
In the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block:
1. Replace the text in the top <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block containing “hello ” with “You are Shakespeare, respond as such: ” (make sure there is a space after the colon, otherwise the colon will immediately be followed by the next text value with no space in between).
2. Delete the bottom <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block and replace it with the <span style="background-color:#70ce9c;font-weight:bold;color:white">Prompt Input's Text</span> block.
We want the LLM to receive the prompt:<br>
**“You are Shakespeare, respond as such: [MESSAGE]”**, where [MESSAGE] is the text that the user submits.<br>
This makes it so that the LLM will respond to the message as Shakespeare.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #2: Respond as Shakespeare]</span><br>
Preview the app. Check that the LLM produces a response to the text submitted by the user as Shakespeare. Again, you may need to wait a few seconds before there is a response.<br>
If it works, the “Response” label should display a response to the text submitted by the user as Shakespeare. Next, we want the LLM to communicate as a historical figure of the user's choice.<br>
**Let's move to the Design tab.**
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_15.png)
Add a text input for users to type in the name of a historical figure. We will rename it to “Name Input”.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_16.png)
Add a button to submit the name of a historical figure. We will rename it to “Submit Name”. In the properties panel, replace the default value “Button” with “Submit Name”.<br>
**Let's move back to the Blocks tab.**
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_17.png)
Now, we want to add functionality to the button we added for the user to submit the name of a historical figure. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Name Click</span> block.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_18.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Historical Figure's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Name Click</span> block. We want the “Historical Figure” label to update when the user submits the name of a historical figure.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_19.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Name Input's Text</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Historical Figure's Text to</span> block. We want the “Historical Figure” label to display the name of the historical figure that the user submitted.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_20.png)
Now we will adjust the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block so that it takes in the name of the historical figure that the user submitted:
1. Click the plus icon in the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block twice to add 2 more slots for text values to be joined.
2. First, move <span style="background-color:#70ce9c;font-weight:bold;color:white">Prompt Input's Text</span> to the 4th slot.<br>
3. Next, you must split up the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block in the prompt so that “Shakespeare” can be replaceable. Edit the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block in the 1st slot to be “You are ” (make sure there is a space after “are”).
4. Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Historical Figure's Text</span> block to the 2nd slot.
5. Connect a new <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block to the 3rd slot and write in “, respond as such: ” (make sure there is a space after the colon).
We want the LLM to receive the prompt:<br>
**“You are [HISTORICAL FIGURE], respond as such: [MESSAGE]”**, where [HISTORICAL FIGURE] is the name of a historical figure that the user submits and [MESSAGE] is the text that the user submits.<br>
This makes it so that the LLM will respond to the message as the historical figure that the user has chosen.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #3: Custom Historical Figure]</span><br>
Preview the app. Check that the LLM produces a response to the text submitted by the user as the historical figure submitted by the user. Again, you may need to wait a few seconds before there is a response.<br>
If it works, you now have an app that allows users to communicate with a “historical figure” of their choice through LLMs!
---

# Historical Figures
<span style="font-weight:bold">[Extension #1: Historical Figures Selection Screen]</span><br>
Instead of giving users the ability to pick a historical figure of their choice, provide them with pre-selected options to choose from on a **Selection** screen.<br>
Starting with:
1. Add another screen to the project to facilitate the selection process. You may need to rearrange the screens in the component tree.
2. On the **Selection** screen, add buttons per historical figure.
3. Update the **Communication** screen so that the selected historical figure is used.
4. You may want to add a “Back” button so users can return to the **Selection** screen.
---

