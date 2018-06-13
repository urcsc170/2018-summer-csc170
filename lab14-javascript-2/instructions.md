# Lab 14: JavaScript, Part 2
*Due: Monday, June 18, 2018*

For this lab, you will do much the same as what you did in Lab 13 except this time you’ll use your own content from Lab 12, and insert some simple JavaScript behaviors.

## Step 0 (prep): Get Two New Identically-sized Images

Find and prepare two new images

- The two new images must be related to your website’s topic
- The two new images must have identical height and width
- The two new images must have a width dimension of no less than 200px and no more than say about 300px

Preparing identically-sized images might take some extra work using software on your PC or Mac.

- On a PC, the application “Paint” comes with Windows and will work well enough
- On a Mac, the application “Preview” has “tools” that will work well enough
- The two new images must have filenames that comport to the rules for naming web files (all lower case, no spaces)

## Step 1: Copy Lab 12

- Make a copy of your Lab 12 (*not Lab 13!*) - put it in a folder named **lab14**
- Add the two images you created in the previous step into the **images** folder

## Step 2: Create a Home Page

- Rename your **start.php** file to **index.php**
- In the **index.php** file, directly under the *nav.inc* statement create a new element:<br> `<section> </section>`

- Add an H2 in the SECTION element - some kind of welcome message, something like this: `<h2>Welcome to The World of William Shakespeare</h2>` <br>_(It doesn’t have to say, “Welcome to….”  You can be creative here)_
- Add these two classes to the SECTION tag, `class="hero full-width"`
- Within the SECTION element, add a FIGURE element and a DIV like this:

```html
<section class="hero full-width">
  <h2>Welcome to The World of William Shakespeare</h2>
  <figure>

  </figure>

  <div>

  </div>
</section><!--.hero-->
```

- Edit your **inc/nav.inc** file:
  - Add a list item to the new **index.php** file
  - Have the text for the link say something like "Home" ...or something like that
  - Save and close the **inc/nav.inc** file

## Step 3: Add Styles to the Home Page

- Edit the **inc/html-top.inc** file:

  - Change the TITLE to say "Lab 14..." instead of Lab 12

  - Add a new LINK to a new stylesheet (that you'll create next) like this

    ```css
    <link rel="stylesheet" href="css/home.css">
    ```

- Save and close the **inc/html-top.inc** file

- Create a new file in the **css** folder named **home.css**

- Edit the new **css/home.css** file

  - Here you can add whatever styles you want to make your HTML form look like it's a part of your website.  At the bare minimum, try these styles...

  ```css
  .hero { 
  	display: grid;
  	grid-template-columns: 1fr 2fr;
  	border-bottom: 1px solid #333333; 
  }
  .hero h2 { grid-column: 1 / 3; }
  ```

  ...do more as you'd like.  (Not graded.)

- Save and close the **css/home.css** file

## Step 4: Add a Swappable Image

Back in the **index.php** file...

- Within the new FIGURE element, add an IMG tag to embed one of the new images; something like this:

```html
<figure>
  <img src="images/______.jpg" alt="_________">
  <figcaption>Some words  - you write here</figcaption>
</figure>
```

…In the blanks (above) use whatever you named one of your new images in the SRC and write its description in the ALT

- Add the JavaScript **onmouseover** event to the image element to change the source (the “src”) to the other new image when a mouse hovers over that element
- Add another JavaScript **onmouseout** event to the *same image element* to change the source (the “src”) to back to the original image when the mouse moves *out* from hovering over that element

## Step 5: Add Some Hidden Content

Still editing the **index.php** file...

- Insert two DIV elements within the DIV after the FIGURE element like this:

```html
<div>
    <div>
       
    </div>
    <div>
        
    </div>
</div>
```

- Add a button element that says “More…” between the two DIVs like this:

```html
<div>
    <div>
       
    </div>
    
    <button>More...</button>
    
    <div>
        
    </div>
</div>
```

- “Steal” some content from your ARTICLE and/or ASIDE
  - A good candidate is some “Introduction” content if you have one
  - You need at least two paragraphs with headings; insert the two paragraphs (and their headers preferably) into the two DIVs (respectively); something like this (using your content, not Shakespeare)

```html
<div>
	<div>
		<h2>About Shakespeare</h2>
		<p>William Shakespeare was an English poet...p>
	</div>
	<button>More...</button>
	<div>
		<h2>More About Shakespeare</h2>
		<p>His extant works, including...</p>
	</div>
</div>
```

- Delete the rest of the content on the page: the ARTICLE, ASIDE, and FOOTER

From an appearance standpoint, you should have something that looks like this:

![screen capture](media\figure1.png)

- Save and close **index.php**

### Power the 'More...' Button
- Add an ID to the BUTTON element
- Add an ID to the second DIV element
- In the file system, add a new folder named: **js**
- Make a copy of the JavaScript file from Lab 13 (js/**scripts.js**) and copy it to your new **js** folder in lab14
- Near the bottom of the Index page, just above the closing BODY tag, add an embedded JavaScript block using the `<script>` tag to connect the external JavaScript file named: **js/scripts.js**
- As necessary, edit the **js/scripts.js** file to work with lab14
  - Change the name of the toggler to whatever you used in your HTML document
  - Change the name of the togglee to whatever you used in your HTML document
- Change the default display setting from “inline” to “none” like this:
`toggle_element.style.display = 'none';`

## Step 6: Upload, Test and Report your Work

If your home page works correctly:

- When you first load the webpage the second paragraph is NOT showing
- When you hover your mouse over the image, it changes
- When you move your mouse away from the image, it changes back
- When you click the “More…” button, the hidden paragraph appears
- When you click the “More…”button again, the paragraph disappears again

When you are done with your webpage, close everything and use an FTP tool to access your account on **csc170.org**and upload your files:

In a web browser (any), go to this address to check your handiwork: 

**www.csc170.org/accountname/lab14/index.php**<br>(where “*accountname*” is your account name)

- Make sure the HTML and CSS pass their respective validators.
- In our CSC 170 Blackboard section in the Lab 14 assignment, post a link to your webpage to receive credit for this Lab.

