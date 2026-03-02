# Fake Voices App
Your goal is to create an app that takes in a message, adjusts the pitch and rate based on the user's preference, and reads it out to the user. The synthetic voice changes depending on the user's settings.<br>
Begin your project by duplicating this [project template](https://x.thunkable.com/projects/697bfe9356673573f9be93cf/aec9c6b9-bb97-412c-8b67-02bbfdb6e014/designer). The project is completely empty besides a block that you will use to access the LLM for Extension #1. Please do not delete the block as you work on the main project. If you experience any issues with accessing or duplicating the template, please speak with your teacher.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_1.png)
Add a text input for users to type in a message. We will rename it to “Text_Input”.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_2.png)
Add a slider for users to adjust the pitch. We will rename it to “Pitch Slider”. In the properties panel, set the default **Value** to be 1, the **Step** to be 0.1, and the **Value range** to be from 0-2.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_3.png)
Add a slider for users to adjust the rate. We will rename it to “Rate Slider”. In the properties panel, set the default **Value** to be 1, the **Step** to be 0.1, and the **Value range** to be from 0-2.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_4.png)
Add 2 labels, one to display the pitch and the other to display the rate. We will rename them “Pitch” and “Rate”.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_5.png)
Add a button for users to submit the message. We will rename it to “Submit”.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_6.png)
Resize and rearrange the sliders and labels so they are side-by-side. This makes it easier to see which label is paired with which slider.<br>
**Now, we will move onto blocks.**
---

# Fake Voices App
<span style="font-weight:bold">Block:</span> <span style="background-color:#f3aa44;font-weight:bold;color:white">when Slider on Value Change</span>

![Block](./Weeks/Week 7/images/w7_block_whenSliderOnValueChange.png)

<span style="font-style:italic">This block can be found in the **Slider** drawer (with the name of your slider) under <span style="font-weight:bold">UI Components</span>.</span><br>
The <span style="background-color:#f3aa44;font-weight:bold;color:white">when Slider on Value Change</span> block fires as the value of the slider changes. The current value of the slider is retrieved via the <span style="background-color:#70ce9c;font-weight:bold;color:white">value</span> block.<br>
**NOTE:** This is different from the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Slider on Sliding Complete</span> block which fires only after the user lifts their finger or thumb off the slider.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_7.png)
First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Pitch Slider on Value Change</span> block. We want to make updates when the pitch slider moves. The value of the pitch that the slider holds can be retrieved from the <span style="background-color:#70ce9c;font-weight:bold;color:white">value</span> block.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_8.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Pitch's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Pitch Slider on Value Change</span> block. We want the “Pitch” label to update every time the pitch slider's value changes.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_9.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">value</span> from the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Pitch Slider on Value Change</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Pitch's Text to</span> block. We want the “Pitch” label to update to the value every time the pitch slider's value changes. You can click and drag the <span style="background-color:#70ce9c;font-weight:bold;color:white">value</span> block directly from the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Pitch Slider on Value Change</span> block.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_10.png)
Now, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Rate Slider on Value Change</span> block. We want to make updates when the rate slider moves. The value of the rate that the slider holds can be retrieved from the <span style="background-color:#70ce9c;font-weight:bold;color:white">value</span> block.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_11.png)
Connect the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Rate's Text to</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Rate Slider on Value Change</span> block. We want the “Rate” label to update every time the rate slider's value changes.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_12.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">value</span> from the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Rate Slider on Value Change</span> block to the <span style="background-color:#3f9e83;font-weight:bold;color:white">set Rate's Text to</span> block. We want the “Rate” label to update to the value every time the rate slider's value changes. You can click and drag the <span style="background-color:#70ce9c;font-weight:bold;color:white">value</span> block directly from the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Rate Slider on Value Change</span> block.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #1: Verify Slider Labels]</span><br>
Preview the app. See if the labels display the sliders' values when you use the sliders.<br>
If it works, the labels should update every time the sliders have a new value. Now, let's give a use to the sliders and their values.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_14.png)
Now, we want to add functionality to the button we added for the user to submit a message. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_15.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">say [text] in [language]</span> block (you were first introduced to this block in Project 1: First App) to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Submit Click</span> block.
---

# Fake Voices App
<span style="font-weight:bold">Block:</span> <span style="background-color:#735ca5;font-weight:bold;color:white">say [text] in [language]</span> (Advanced)

![Block](./Weeks/Week 7/images/w7_block_sayTextInLanguageAdvanced.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Speech Blocks</span> drawer under <span style="font-weight:bold">App Features</span>.</span><br>
The advanced <span style="background-color:#735ca5;font-weight:bold;color:white">say [text] in [language]</span> block allows the **pitch** and **rate** of speech to be altered.
For **pitch**, lower values correspond to lower pitch, and higher values correspond to higher pitch.
For **rate**, lower values correspond to slower speech, and higher values correspond to faster speech.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_16.png)
Right-click the <span style="background-color:#735ca5;font-weight:bold;color:white">say [text] in [language]</span> block and click on "Show advanced block" to get additional settings for the block. This will allow us to adjust the pitch and rate of the speech from the block.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_17.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Text_Input's Text</span> to the say part of the <span style="background-color:#735ca5;font-weight:bold;color:white">say [text] in [language]</span> block. We want the text that the user submitted to be read aloud.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_18.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Pitch Slider's value</span> to the at pitch part of the <span style="background-color:#735ca5;font-weight:bold;color:white">say [text] in [language]</span> block. We want the pitch to be set to the value selected by the user via the pitch slider.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_19.png)
Connect the <span style="background-color:#70ce9c;font-weight:bold;color:white">Rate Slider's value</span> to the with rate part of the <span style="background-color:#735ca5;font-weight:bold;color:white">say [text] in [language]</span> block. We want the rate to be set to the value selected by the user via the rate slider.
---

# Fake Voices App
![Setup](./Weeks/Week 7/images/w7_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #2: Test Speech Output]</span><br>
Preview the app. Type in a few words or a sentence, adjust the sliders, and click the button to submit the text. Check that the provided text is read aloud with an altered pitch and rate.<br>
If it works, you now have a synthetic voice with adjustable pitch and rate that reads aloud messages that users submit!
---

# Fake Voices App - Extension #1: Suggested Values
<span style="font-weight:bold">[Extension #1: Suggested Values]</span><br>
Now, let's allow users to get suggested pitch and rate values from the LLM to emulate a person of their choice.<br>
You will need to use the <span style="background-color:#735ca5;font-weight:bold;color:white">call Open AI's Text Complete</span> block that takes in a prompt requesting the pitch and rate values based on the user's person of choice and returns those values to the user so they can use them in the main project portion of the app.
