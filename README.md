# Final Project Documentation
## What I did
First, I created a personal website off github's hosting platform. 
Next, I went to http://racheldevorah.studio and opened the developer window and used the html and css files as reference for formatting and such.

My first real issue arrived when I had to position my image on the main page. At first the image didn't appear. This was because I didn't properly put the file path in my html file (my images are in a folder called "images").

My next issue came with positioning the photo with the "artist statement" paragraph. At first, the text appeared below the image, when I wanted the text and image side by side. I tried using margins and text align to move the image to the side and the text to the opposite side, but it still didn't work. The solution was to put the image and text in a `<div>` container, and then use the flex command to make them fit side by side within the container.

Next I added a nav bar. I added a home, about, media, and links pages. At first, the buttons appeared on my website, but I got an error404 everytime I clicked one. I then googled what was wrong and stackoverflow.com told me that I need multiple html files. Adding more html files and making small changes between them based on what they need solved my issue.
Source: https://stackoverflow.com/questions/66146728/hosting-a-github-pages-server-with-multiple-html-files

Then I decided I wanted my nav bar to be centered, and fixed at the bottom of my page, so that when I scroll down, it sticks to the same position on the screen and does not overlap with any other content.
I also consulted stack overflow for this.
Source: https://stackoverflow.com/questions/643879/css-to-make-html-page-footer-stay-at-bottom-of-the-page-with-a-minimum-height-b
I still coudn't implement it properly in my code so I decided to prioritize functional aspects of the site rather than visual.

Next, I added an embeded youtube video of me playing drums in my "media" page. This was fairly straightforward since I could copy the embed code directly from youtube and paste it into my code. The issue was centering the video with the page.(I still don't know how to do this it hasn't been working).

I also added a video from instagram of my band playing.

Next I added the "links" page, with all of my various social medias and things. First I put in the hyperlinks and got those working.

I also decided to embed my band's single on my homepage, below my artist statement. The formatting worked perfectly the first time, which was very surprising.

## ABDYD
- Changed `<img src="juliancnotegrey.jpg">` to `<img src="/images/juliancnotegrey.jpg">`

- artist bio and statement paragraphs were not spaced properly - added `<br/><br/>` instead of `<br/>`

- in order to make artist statement and image line up side by side, I put them in a container and used a flex display:
`<div class="container">`
	`<img src="/images/juliancnotegrey.jpg" class="left-image">`
	`<div class="artiststatement">`
		`<h3><b>Artist Statement</b></h3>`
		`<p>"blah blah blah arist statement (didn't want to paste the whole thing cus its a wall of text)"</p>`
`</div>`

and in the CSS file:
`.container {
	display: flex;
	align-items: center;
	gap: 20px;
}

img {
	  width: 40%;
}

.artiststatement {
	flex: 1;
	color: white;
	width: 45%;
}`

## ChatGPT Interactions (Photos)
<img src="ChatGPTPhotos/gpt1.jpg">
<img src="ChatGPTPhotos/gpt2.jpg">
<img src="ChatGPTPhotos/gpt3.jpg">
<img src="ChatGPTPhotos/gpt4.jpg">
<img src="ChatGPTPhotos/gpt5.jpg">
<img src="ChatGPTPhotos/gpt6.jpg">
<img src="ChatGPTPhotos/gpt7.jpg">
<img src="ChatGPTPhotos/gpt8.jpg">
<img src="ChatGPTPhotos/gpt9.jpg">
<img src="ChatGPTPhotos/gpt10.jpg">

## What I learned from ChatGPT
- GPT pointed out that my nav bar was outside my body (this was an accident)
- GPT said I should use a div container instead of span, I don't exactly know why, but I assume span is used for something niche that I don't know about, while div is more general
- I learned the new commands in the 3rd photo (the comments from GPT helped)
- GPT helped me restructure my HTML and CSS files, which helped me understand how containers should be structured in order to work more effectively
- lastly GPT helped me put my embeded videos on the site, but I coudln't get them centered still