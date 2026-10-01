# Kristie Jones — Portfolio

## Open the website
Extract the ZIP first. Open index.html in your browser. Keep all HTML files in the same folder and keep the images folder alongside them. No installation is required.

## About Me
about.html includes the professional headshot, biography, education, and Contact Me section with your LinkedIn link. The photo is images/kristie-jones-headshot.png; keep it with the website files.

## Project pages
- portfolio-website.html — the personal portfolio website
- simple-bank-orderly.html — the Python banking application
- banking-test-suite.html — banking refactoring and testing
- youth-football-registration.html — youth football registration system
- bath-county-football.html — Bath County Football website

Each homepage project card opens its own page. Each project page has an overview, key features, three screenshot areas with captions, a learning section, and navigation back to the homepage.

## Add screenshots
1. Save a real screenshot in the images folder. PNG or WebP works well for interface text. Use lowercase filenames without spaces.
2. Open the corresponding project HTML file in a text editor and search for `Screenshot to be added`.
3. Replace only the content inside that slot's `<div class="screenshot">` with an image element, for example:

```html
<div class="screenshot">
  <img src="images/bank-main.png"
       alt="Simple Bank Orderly teller interface with the navigation menu on the left"
       decoding="async">
</div>
```

For screenshots below the first image, add `loading="lazy"` to the img element. An example filename is already provided in a comment above each screenshot slot. Keep the surrounding figure and figcaption, and update the caption to describe the actual screenshot. Images scale down to the page width while retaining their aspect ratio; they are not cropped.

For desktop captures, approximately 1400–1800 pixels wide is a useful starting point. For mobile captures, 390–780 pixels wide is usually sufficient. Export at the smallest size that keeps interface text readable. Use demonstration data in screenshots.

## Add another project
1. Copy the closest project page to a new HTML filename.
2. Update its title, description, overview, features, screenshots, and learning text.
3. Copy a homepage `<article class="project">` block inside `<div class="projects">`.
4. Change the new card's title, description, tags, and link to the new page filename.
5. Update the project-page Next links if you want to include the new page in that sequence.

## Styling and GitHub
The CSS is embedded in each HTML file, so each page works without a build tool. Colors are defined in the :root variables. To change the color scheme across the whole site, update those variables in every HTML file.

When you are ready to upload this website, include all seven HTML files and the images folder together. The homepage is index.html. This package does not publish the website or connect to your GitHub account.
