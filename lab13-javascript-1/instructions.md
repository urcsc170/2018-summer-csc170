# Lab 13: JavaScript, Part 1
*Due: Monday, June 18, 2018*

For this lab, you will take a set of HTML and CSS **starter files**, downloaded from Blackboard, and add JavaScript using three techniques: external; embedded; and event

In the starter files, to help you find the places where you're supposed to install the JavaScript, look for the HTML comments in the files provided that say, “PART 1…”, “PART 2…” et cetera.

# Part 0: Setup

- Download the file: [lab13_starter-files.zip](http://csc170.org/rkostin/distribution/lab13_starter-files.zip) and expand the files on your computer or thumb drive  into a folder named **lab13**

# Part 1: Add an embedded script

- Near the bottom of the HTML document, just above the closing body tag, add an embedded JavaScript block using the `<script>` tag, and write an alert that pops open a dialog box and says a message.
- After you confirm that the pop-up dialog box works, comment-out the JavaScript inside the `<script>` tags using "//" (two slashes) at the beginning of the line so it doesn’t work anymore (because it’s annoying).

# Part 2: Use a JavaScript event to change an image

Apply the following events to the first IMG element near the top of the HTML document (line 21)

- Add the following JavaScript event to the image element to change the source (the “src”) to **images/cat2.jpg** when a mouse hovers over that element
  - `onmouseover="this.src='images/cat2.jpg'"`

- Add the following JavaScript event to the *same image element* to change the source (the “src”) back to **images/cat1.jpg** when a moves out from hovering over that element
  - `onmouseout="this.src='images/cat1.jpg'"`

# Part 3: Connect to an external script

- Near the bottom of the HTML document, just below the embedded JavaScript you created in Part 1, using another `<script>` tag, connect an external JavaScript file named: **js/scripts.js** (that file already exists - it came with the starter files)

# Part 4: Use JavaScript to run a function

- Within the second `<figure>` element in the HTML document, add an ID attribute to the image (line 35) to uniquely identify it in the HTML document (you pick the name of the ID)

- Also add an ID attribute to the BUTTON element (line 37) to uniquely identify it in the HTML document (you pick the name of the ID)

- In the attached JavaScript file (**js/scripts.js**), follow the comments in the code to power the script to make the button work as intended.
  - _You need to *replace* the blanks (____________) with the IDs you added on the IMG and the BUTTON; make sure you put the right ID in the right blank_

# Part 5: Check and Upload your Work

- Make sure both hover events (onmouseover and onmouseout) work and the button works.


- Validate the HTML file (**http://validator.w3.org/**)

When you are done with your webpage, close everything and use an FTP tool to access your account on **csc170.org** and upload your **lab13** folder

- In a web browser (any), go to this address to check your handiwork:  
  **www.csc170.org/accountname/lab13/index.html**<br>
  (where “*accountname*” is your account name)

# Part 6: Report your work

- In our CSC 170 Blackboard section in the Lab 13 assignment, post a link to your webpage to receive credit for this Lab.