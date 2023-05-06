# The website for the MATH student council 
This repo contains the website for the MATH student council at KU.

## Site structure
The pages for this site are located in `/content/`, each folder contains an `index.md` file which can be freely edited. 

To add a new page, create a new folder under `/content/`. For example `/content/revy`. Now create an `index.md` file under the folder with the following contents (as an example)
```
---
title: "Revy videoer"
omit_header_text: true
featured_image: 'img/hero-bg.jpg'
menu:
  main:
    weight: 1
---

...
```
Between the `---` block are the parameters that specify the page:

- `title` will be the title of the page, which is also shown under the navigation menu. 
- `featured_image` is the background image for the header
- `menu` controls whether the page should be showing in the navigation menu 

There are other options that are available, see [ananke Hugo theme](https://github.com/theNewDynamic/gohugo-theme-ananke)

## How to guides: 

### Adding a new course video 
To add a new course video to 'Kursusvideoer' simply edit `content/videos/index.md` and add a new HTML div element to the video grid. 
```html
  <div class="video-grid-item">
    {{< youtube ID-OF-VIDEO-HERE >}}
  </div>
```
This edit can be done through the browser, you can make a pull request or commit directly to the main branch if you are an admin. 
