# Final Project Documentation
## What I did
First, I created a personal website off github's hosting platform. 
Next, I went to http://racheldevorah.studio and opened the developer window and used the html and css files as reference for formatting and such.

My first real issue arrived when I had to position my image on the main page. At first the image didn't appear. This was because I didn't properly put the file path in my html file (my images are in a folder called "images").

My next issue came with positioning the photo with the "artist bio" paragraph. At first, the text appeared below the image, when I wanted the text and image side by side. I tried using margins and text align to move the image to the side and the text to the opposite side, but it still didn't work. The solution was to put the image and text in a `<div>` container, and then use the flex command to make them fit side by side within the container.

Next I added a nav bar. I added a home, about, media, and contact pages. At first, the buttons appeared on my website, but I got an error404 everytime I clicked one.

## ABDYD
Changed `<img src="juliancnotegrey.jpg">` to `<img src="/images/juliancnotegrey.jpg">`
