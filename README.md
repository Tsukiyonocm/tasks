# Basic Project Outline

## A simple task manager.

## Input Task:
This will be the top of the program. To start this will have a simple circle with a + icon on it. 
Once clicked, this + icon slides to the left edge of the screen and a input box grows to the right for you to 
type your task into. Once enter is hit, this is added as a Task Item down below.


## Task Item:
Taking the input from the above input line, this will display that task as an item with two clickable
icons to its right and one to the left. The first will be a down arrow which will show a list of sub items if there are any. If 
there are not, it will show only an simple input in order to input your sub items. To the right of the arrow is a X or trash can 
icon which will be used to delete a task. To the left of the input title is a clickable checkbox which strikes through the task
and all sub-items when completed.


## Sub Items: 
These will have all the same functionality of the task items above. Sub items will not be viewable 
by default, before the arrow icon is clicked they are hidden. Once clicked, they slide down display each sub items as well as an
input for additional ones to be added.


## Step 1: Basic Architecture
1. Create a simple HTML and CSS layout of the features (no javascript at all). This will work as a scaffolding of what the items
need to look like after everything is all setup. This step will also not require any animations either. So in this case the Input
Task icons will be all the way right as well as having the input fully extended.


## Step 2: Animation
1. Create Animation for Task Input menu. The feature will start with just the circle in the center of the area. Once clicked it will
roll all the way to the right. Once there, the input will push out to the left for the input field. 
2. Create the dropdown animation for Sub-items within a Task Item. These will be hidden by default. Once the arrow is clicked it drops
down displaying all the subtasks. If there are no subtasks, then it will display only a input field to input a new subtask. Once the
arrow is clicked again it will slide back up to be hidden from view again.
3. There might be some very basic JavaScript that will need to be setup for these steps. This could very well just be for testing purposes,
but this might make it into the final variation of the app. As such, great care should be taken to make sure that variable names are named 
properly and the code is relatively clean. (There will likely be revisions later once things get fully functioning)


## Step 3: JavaScript - Input Task
1. If not setup in the animation section, setup the click event listener to start the animation for the click button.
2. Create a variable in order to store the new Todo's in.
3. Catch the value from the input field.
4. Push this value to the Todo's variable. (likely an array, though maybe an object?)
5. Create a function to create the new Todo and to populate it with all functions (checkbox, arrow, X).



## Step 4: JavaScript - Task Items
1. Create double click event in order to update the Task value if entered incorrectly.
2. Click event on checkbox that puts a strike-through through all the text for the input as well as all sub-items.
3. Click event to delete the entire item and all sub-tasks.
4. Click event on arrow to drop down the sub-items. This event must close it again if clicked again.



## Step 5: JavaScript - Sub-items
1. Create double click event in order to update the Task value if entered incorrectly.
2. Click event on checkbox that puts a strike-through through all the text for the input as well as all sub-items.
3. Click event to delete the entire sub-task.



## Step 6: JavaScript - Completed Items
1. Completed Items that are not deleted are moved to the bottom of the list. Sub-items are still viewable if clicked on. Deleted items are
removed permanently. Initially this will be unable to be undone.



## Step 6: Local Storage
1. All variables need to be stored locally. Will update this step as I understand more about how local storage works.



## Step 7: Future Updates
1. Adding a date/time to the app in general. This will be used on a day to day habit so having this feature will be nice to have available.
While its nice to have, its not essential which is why this will be added at a later time.
2. Once date/time is added, this can be added into each todo as well in order to display when it was created, or to even set an expected
end date to the tasks at hand. 
3. Have a second tab on the display which will showcase all of the completed todo's instead of having them all viewable on the page directly.
Once again, a nice feature but not required. There is a good chance most of the tasks will be deleted instead of marked as completed.
That, or will be deleted soon after completion to clean things up.
4. Attaching to a database such as Mango or another. This will likely be far in the future as I know nothing about working with
databases currently. This will likely also require a web host for it to be posted online since Github and Netlify do not support
databases on their free services.
5. Update the CSS to utilize SASS instead of static CSS. 
6. Filter to sort and hide out the completed tasks from the incomplete tasks. This could probably be utilized in the future to also sort
particular tasks as well. Future thought will be needed for how to 
implement this.  


## Tech Being Used
CSS - I will probably stay away from SASS currently just because I am out of practice all together and just need to get my feet wet again.
That said, I will be trying to use Flexbox for this project to keep my familiarity of that up front and center.<br>
JS - Vanilla JS only, will be using no libraries.

## Color Values
Primary Background - RGB(33,39,62) (dark blue /grey)

Input/Task Background - RGB(48,54,81) (lighter blue / grey)

Add Task Icon - RGB(95,199,138) (green)

Add Task Background - RGB(22,31,55) (navy blue)

Text Color - RGB(219,219,221) (near white)

Hover?

TrashCan? maybe add icon green


## Icons
Plus - `<i class="fas fa-plus"></i>` 

Trash - `<i class="fas fa-times"></i>`



