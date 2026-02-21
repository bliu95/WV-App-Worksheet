# Data Filtering App
Your goal is to create a filtering app. Users should be able to select a filter and see the items that satisfy the filter in a data viewer.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_1.png)
Create a new local data source. We will rename Column 1 to “Item” and Column 2 to “Category”. Fill out the table with data. We will use grocery list data as an example, but feel free to choose your own topic, ensuring that the categories in Column 2 can be used to filter the items in Column 1.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_2.png)
Add a data viewer list to display the data. We will rename it to “Data_Viewer_List”.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_3.png)
In the properties panel for Data_Viewer_List, do the following:
1. Connect the data source.
2. Populate the **Title** property with the “Item” column.
3. Populate the **Subtitle** property with the “Category” column.
At this point, you may want to resize Data_Viewer_List to better fit your data.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #1: Verify Data Display]</span><br>
Preview the app. See if your data displays correctly.<br>
If it works, the data from your data source will be displayed in Data_Viewer_List. Now, let’s add an option to filter the items by category.<br>
**Let's continue in the Design tab.**
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_5.png)
Open your data source and click **Add Filter View**. We will need a filter view to allow filtering items by category.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_6.png)
In the **Add Filter View** pop-up panel:
1. Rename the filter view to something meaningful, such as “By Category”.
2. Change the selected column from “Item” to “Category”.
3. Type in one of your categories in the box that says “Type value”, such as “Produce” in the example.
4. Click **Create Filter View**.
In the example, this filter view contains one filter rule, “Where Category = Produce”, which means only the items with the category “Produce” will be shown in the filter view.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_7.png)
In the properties panel for Data_Viewer_List, replace Default View with the filter view you created in the last step, such as “By Category”, under **Filter View**.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #2: Verify Filter View]</span><br>
Preview the app. See if it now displays the rows that satisfy the filter.<br>
If it works, Data_Viewer_List will now show only the rows that satisfy the filter rule that you have set. Let’s make it so that we can dynamically update the filter rules so we can change the category to filter by.<br>
**Let's continue in the Design tab.**
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_9.png)
Add a text input for users to enter a category to filter by. We will rename it to “Filter Input”.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_10.png)
Add a button for users to submit a category. We will rename it to “Apply Filter”. In the properties panel, replace the default value “Button” with “Apply Filter”.<br>
**Now, we will move onto blocks.**
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_11.png)
Now, we want to add functionality to the button we added for the user to submit a category to update the filter. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Apply Filter Click</span> block.<br>
---

# Data Filtering App
<span style="font-weight:bold">Block:</span> <span style="background-color:#735ca5;font-weight:bold;color:white">update filter for</span>

![Block](./Weeks/Week 5/images/w5_block_updateFilterFor.png)

<span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Data Sources Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span> after a filter view has been created.</span><br>
The <span style="background-color:#735ca5;font-weight:bold;color:white">update filter for</span> block allows you to edit the conditions, also known as filter rules, in a filter view of your data source.<br>
The <span style="background-color:#75afc8;font-weight:bold;color:white">list</span> block shows the conditions in a filter view and can be used to add or remove conditions. The list can be empty, which means there are no conditions in the filter view.<br>
The <span style="background-color:#f89da2;font-weight:bold;color:white">create object with fields</span> block represents a single filter rule. Do not change the field texts “column”, “operator”, and “value”. You can, however, change or replace the <span style="background-color:#df6078;font-weight:bold;color:white">text</span> blocks connected to those fields.<br>
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_12.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">update filter for</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Apply Filter Click</span> block. We want the filter to be updated when the user clicks the “Apply Filter” button. 
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_13.png)
In the <span style="background-color:#f89da2;font-weight:bold;color:white">create object with fields</span> block, replace the text block attached to the <span style="background-color:#fbe4e9;font-weight:bold">value</span> field with the <span style="background-color:#70ce9c;font-weight:bold;color:white">Filter_Input's Text</span> block. This updates the filter rule so instead of the default filter rule, such as “Category = Produce”, it will now filter by the category that the user submits.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #3: Dynamic Filter]</span><br>
Preview the app. Check that when the user updates the filter rule, the data viewer updates to show the items that match.<br>
If it works, you now have an app that allows users to filter through items in a data source based on certain conditions, but there is no way of clearing the filter to show everything in the data source. Let’s add another button to allow that.<br>
**Let's move to the Design tab.**
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_15.png)
Add a button for users to clear the filter. We will rename it to “Clear Filter”. In the properties panel, replace the default value “Button” with “Clear Filter”.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_16.png)
Now, we want to add functionality to the button we added for the user to clear the filter. First, add the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Clear Filter Click</span> block.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_17.png)
Connect the <span style="background-color:#735ca5;font-weight:bold;color:white">update filter for</span> block to the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Clear Filter Click</span> block. We want the filter to be updated when the user clicks the “Clear Filter” button.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_18.png)
Now, we will delete the <span style="background-color:#f89da2;font-weight:bold;color:white">create object with fields</span> block to remove the filter rule from the filter view. This would display all of the items in the data source in Data_Viewer_List rather than only the items that match the filter rule, which is identical to Default View.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #4: Clear Filter]</span><br>
Preview the app. Check that when the user clears the filter rule, the data viewer updates to show all items in the data source, which is identical to the Default View.<br>
If it works, you now have an app that allows users to filter through items in a data source based on certain conditions and clear the filter to show everything in the data source; however, the app still starts with a filtered list of items instead of all the items in the data source. Let’s make the final touches to allow that.<br>
**Let's move to the Design tab.**
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_20.png)
Open your data source and click into your filter view, such as “By Category”, click the **trash can icon** next to the filter rule to remove it. Now that we can add a filter rule dynamically using blocks, we no longer need this placeholder filter rule.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_21.png)
Click **Save**. We want our filter view to start off with no filter rules, so it will look identical to Default View when the app starts.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_22.png)
The filter view should now look identical to Default View. You may click back and forth between the two views to verify.
---

# Data Filtering App
![Setup](./Weeks/Week 5/images/w5_checkpoint.png)
<span style="font-weight:bold">[Checkpoint #5: All Items on Startup]</span><br>
Preview the app. Check that when the app starts, the data viewer shows all items in the data source, as if it was Default View.<br>
If it works, you now have a fully-functioning data filtering app!
---

# Data Filtering App - Extension #1: Add New Item
<span style="font-weight:bold">[Extension #1: Add New Item]</span><br>
Allow the user to add new items to the data source.<br>
You may choose to use functions for this extension, but it is not required. A function is a block of code that performs a specific task. If you use the same code set multiple times in your project, you can work more efficiently using functions.

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">create function</span></div><img src="./Weeks/Week 5/images/w5_ext1_block_createFunction.png" alt="Block: create function"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Functions Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
This block is used to create a function. Replace <span style="background-color:#c7bedc;font-weight:bold">do something</span> with a clear function name. Clear function names can help make your code more readable.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">run function</span></div><img src="./Weeks/Week 5/images/w5_ext1_block_runFunction.png" alt="Block: run function"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Functions Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span> after a function has been created.</span><br>
Once you have created your function, you can use it at any time using the function block you have named.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">create function with inputs</span></div><img src="./Weeks/Week 5/images/w5_ext1_block_createFunctionWithInputs.png" alt="Block: create function with inputs"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Functions Blocks</span> drawer under <span style="font-weight:bold">Core Blocks.</span></span><br>
Pressing the plus icon in the block used to create a function would add an input variable. You can then treat that input as a local variable in your function, meaning it can only be used from within the function. There can be multiple input variables for one function.</div></div>

<div class="block-intro"><div class="block-intro-header">Block: <span style="background-color:#735ca5;font-weight:bold;color:white">run function with inputs</span></div><img src="./Weeks/Week 5/images/w5_ext1_block_runFunctionWithInputs.png" alt="Block: run function with inputs"><div class="block-intro-description"><span style="font-style:italic">This block can be found in the <span style="font-weight:bold;color:#735ca5">Functions Blocks</span> drawer under <span style="font-weight:bold">Core Blocks</span> after a function with inputs has been created.</span><br>
This time, in order to use the function, you must also provide the input variables that the function block calls for.</div></div>
---

# Data Filtering App - Extension #2: Multiple Choice Filter Options
<span style="font-weight:bold">[Extension #2: Multiple Choice Filter Options]</span><br>
Instead of the user typing in a filter, which can potentially lead to errors due to typos or capitalization, have them select between multiple possible filter options.<br>
While there are many ways to approach this extension, here are three recommended methods, in order from simple to complex:
1. Buttons
2. Icons
3. Data Viewer Grid
You may choose to use functions for this extension to avoid repetitive code as well, but it is not required.<br>
<hr>
**Method 1 - Buttons**<br>
Add a button for each option to filter by.<br>
<hr>
**Method 2 - Icons**<br>
Add an icon for each option to filter by.<br>
The icon component is used to display an icon and can be made clickable using blocks. The icon displayed in the icon component can be customized via the **Icon Type** property in the properties panel.
<img src="./Weeks/Week 5/images/w5_ext2_icons.png" alt="Method 2 - Icons" style="max-width:100%;margin:0.5rem 0;border-radius:4px"><br>
<hr>
**Method 3 - Data Viewer Grid**<br>
Use a Data Viewer Grid with a custom layout to display the filter options.<br>
While a Data Viewer List displays your data as a list, the Data Viewer Grid displays your data in a grid.<br>
Instructions:
1. In the Design tab, add a new screen for designing a custom Data Viewer Layout.
2. Add a Layout to the new screen.
3. Delete Container2 from the Layout.
4. In Container1's properties panel, set **Direction** to “vertical”.
5. Add an icon and a label in Container1.
6. Adjust the **Width** and **Height** of Container1 and the icon and label within Container1. This will determine the appearance of each item in the Data Viewer Grid.
7. Select the Layout in the Component Tree.
8. Click the **three vertical dots** next to the layout's name in the properties panel.
9. Select **Save as Data Viewer Layout**.
    a. Give your data viewer layout a detailed **Layout Name**.
    b. Select “Grid” in **Layout Type**.
    c. Enable **Advanced Binding**.
    d. Add the icon's iconType to the list of **Bindable Properties**. This allows the icon type to be adjustable.
    e. Click **OK**.
10. In your data source, add a new table to map the category to its corresponding iconType (e.g., the “Dairy” category uses the “Milk” iconType).
11. Add a Data Viewer Grid to the main screen.
12. In the Data Viewer Grid's properties panel, do the following:
    a. Connect the data source.
    b. Select the new table used to map the category to its corresponding iconType.
    c. Select your custom Data Viewer Layout as the **Item Appearance**.
    d. Populate the **Icon** property with the “iconType” column.
    e. Populate the **Label** property with the “Category” column.
13. Adjust the Data Viewer Grid's appearance as needed.
14. In the Blocks tab, use the <span style="background-color:#f3aa44;font-weight:bold;color:white">when Data_Viewer_Grid Item Click</span> block to update the filter by the user's selected category.
    * **Hint:** You can expand the tree in the UI components to open the blocks drawer for elements within the Data Viewer Grid.
Sample Data Viewer Grid:
<img src="./Weeks/Week 5/images/w5_ext2_sampleDataViewerGrid.png" alt="Method 3 - Data Viewer Grid" style="max-width:100%;margin:0.5rem 0;border-radius:4px">
