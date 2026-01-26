# Historical Figures
Create an app where users can communicate with a “historical figure” through LLMs. Users should be able to send a message and get a response from the LLM.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_1.png)
Add a text input for users to type in a message to submit to the LLM. We will rename it to “Text_Input”.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_2.png)
Add a button to submit the message to the LLM. We will rename it to “Submit”.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_3.png)
Add a label to display the response from the LLM. We will rename it to “Response”. You may want to resize the label.<br>
**Now, we will move onto blocks.**
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_4.png)
Under **Advanced Blocks**, click the plus icon next to Open AI Services to add an Open AI Service component.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_5.png)
Click the gear icon next to **Open_AI_Service1** to open up its properties. Under APIKey, click on the x icon to delete everything in the textbox and paste in the API Key provided by your teacher.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_6.png)
Now, we want to add functionality to the button we added for the user to submit a message to the LLM. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block.
---

# Historical Figures
<span style="font-weight:bold">Block:</span> <span style="background-color:#735ca5;font-weight:bold;color:white">call OpenAI Service's Text Completion</span>

![Block](./Weeks/Week 6/images/w6_block_callOpenAIServiceTextCompletion.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Open_AI_Service1</span> drawer under <span style="font-weight:bold">Advanced Blocks </span>after an Open AI Service component has been added.</span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">call OpenAI Service's Text Completion</span> block takes in a text <span style="background-color:#735ca5;font-weight:bold;color:white">prompt</span> for OpenAI to generate text around and has two outputs: <span style="background-color:#70ce9c;font-weight:bold;color:white">response</span> and <span style="background-color:#70ce9c;font-weight:bold;color:white">error</span>. <span style="background-color:#70ce9c;font-weight:bold;color:white">response</span> is the generated text from the LLM. If there was an issue with the API, <span style="background-color:#70ce9c;font-weight:bold;color:white">error</span> would show the issue, otherwise, <span style="background-color:#70ce9c;font-weight:bold;color:white">error</span> is “null”.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_7.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">call OpenAI Service's Text Completion</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block. We want the LLM to run when the “Submit” button is clicked.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_8.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">prompt</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call OpenAI Service's Text Completion</span> block. We want the LLM to receive and respond to the text that the user submits.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_9.png)
Connect the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block to the <span style="background-color:#735ca5;font-weight:bold;color:white">then do</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call OpenAI Service's Text Completion</span> block. Since the LLM can either produce a response or an error message, we want to make sure we account for both messages.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_10.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">error</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">if</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. You can click and drag the <span style="background-color:#70ce9c;font-weight:bold;color:white">error</span> block directly from the <span style="background-color:#735ca5;font-weight:bold;color:white">call OpenAI Service's Text Completion</span> block. When <span style="background-color:#70ce9c;font-weight:bold;color:white">error</span> is “null”, it is treated as False.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_11.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Response's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">do</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. We want the “Response” label to update when the LLM produces an error message.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_12.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">error</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Response's Text to</span> block. We want the “Response” label to display the error message when there is an error. This would help identify any issues that may occur.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_13.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Response's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">else</span> part of the <span style="background-color:#f3aa44;font-weight:bold;color:white">if-else</span> block. Now, we want the “Response” label to update when the LLM does not produce an error message (it outputs “null” for <span style="background-color:#70ce9c;font-weight:bold;color:white">error</span>), i.e., when there is a response.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_14.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">response</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Response's Text to</span> block. We want the “Response” label to display the response when the LLM has successfully produced a response. Once again, you can click and drag the <span style="background-color:#70ce9c;font-weight:bold;color:white">response</span> block directly from the <span style="background-color:#735ca5;font-weight:bold;color:white">call OpenAI Service's Text Completion</span> block.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #1: Basic LLM Response]</span><br>
Preview the app. Check that the LLM produces a response to the text submitted by the user. You may need to wait a few seconds before there is a response.<br>
If it works, the “Response” label should display a response to the text submitted by the user. Next, we want the LLM to communicate as a historical figure.<br>
**Let's move back to the Design tab.**
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_16.png)
Add a label to display the historical figure. We will rename it to “Historical Figure”. In the properties panel, replace the default value “Label” with “Shakespeare”.<br>
**Now, we will move onto the blocks.**
---

# Historical Figures
<span style="font-weight:bold">Block:</span> <span style="background-color:#df6078;font-weight:bold;color:white">join</span>

![Block](./Weeks/Week 6/images/w6_block_join.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#df6078">Text Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
The <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block is used to combine multiple pieces of text into one. In this case, the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> blocks each containing “hello ” and “world” are joined together to be a single text value: “hello world”. Spaces are not automatically added, so they must be typed into the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> blocks when necessary, such as in “hello ”. Other blocks containing text values, such as a variable or a component’s text, may be connected to this block.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_17.png)
Replace the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block with the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block in the <span style="background-color:#735ca5;font-weight:bold;color:white">prompt</span> part of the <span style="background-color:#735ca5;font-weight:bold;color:white">call OpenAI Service's Text Completion</span> block. We want to add more information to the prompt given to the LLM so that it can communicate like a historical figure.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_18.png)
In the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block:
1. Replace the text in the top <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block containing “hello ” with “You are Shakespeare, respond as such: ”. Make sure there is a space after the colon, otherwise the colon will immediately be followed by the next text value with no space.
2. Delete the bottom <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block containing “world” and replace it with the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> block.
We want the LLM to receive the prompt:<br>
**“You are Shakespeare, respond as such: [MESSAGE]”**, where [MESSAGE] is the text that the user submits.<br>
This makes it so that the LLM will respond to the message as Shakespeare.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #2: Shakespeare Response]</span><br>
Preview the app. Check that the LLM produces a response to the text submitted by the user as Shakespeare. Again, you may need to wait a few seconds before there is a response.<br>
If it works, the “Response” label should display a response to the text submitted by the user as Shakespeare. Next, we want the LLM to communicate as a historical figure of the user’s choice.<br>
**Let's move back to the Design tab.**
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_20.png)
Add a text input for users to type in the name of a historical figure. We will rename it to “Name Input”.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_21.png)
Add a button to submit the name of a historical figure. We will rename it to “Submit Name”.<br>
**Now, we will move onto the blocks.**
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_22.png)
Now, we want to add functionality to the button we added for the user to submit the name of a historical figure. Add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Name Click</span> block.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_23.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Historical Figure's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Name Click</span> block. We want the “Historical Figure” label to update when the user submits the name of a historical figure.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_24.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Name Input's Text</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Historical Figure's Text to</span> block. We want the “Historical Figure” label to display the name of the historical figure that the user submitted.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_25.png)
Now we will adjust the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block so that it takes in the name of the historical figure that the user submitted:
1. Click the plus icon in the <span style="background-color:#df6078;font-weight:bold;color:white">join</span> block twice to add 2 more slots for text values to be joined.
2. First, move <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> to the 4th slot.
3. Next, you must split up the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block in the prompt so that “Shakespeare” can be replaceable. Edit the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block in the 1st slot to be “You are ” (make sure there is a space after “are”).
4. Now, connect <span style="background-color:#70ce9c;font-weight:bold;color:white">Name Input's Text</span> to the 2nd slot.
5. Connect a new <span style="background-color:#df6078;font-weight:bold;color:white">text</span> block to the 3rd slot with “, respond as such: ” (make sure there is a space after the colon).
We want the LLM to receive the prompt:<br>
**“You are [HISTORICAL FIGURE], respond as such: [MESSAGE]”**, where [HISTORICAL FIGURE] is the name of a historical figure that the user submits and [MESSAGE] is the text that the user submits.<br>
This makes it so that the LLM will respond to the message as the “historical figure” that the user has chosen.
---

# Historical Figures
![Setup](./Weeks/Week 6/images/w6_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #3: User-Selected Historical Figure]</span><br>
Preview the app. Check that the LLM produces a response to the text submitted by the user as the historical figure submitted by the user.<br>
If it works, you now have an app that allows the user to communicate with a “historical figure” of their choice through LLMs!
---
