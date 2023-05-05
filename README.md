# The website for the MATH student council 
This repo contains the website for the MATH student council at KU.

## How to guides: 

### Adding a new course video 
To add a new course video to 'Kursusvideoer' simply edit `content/videos/index.md` and add a new HTML div element to the video grid. 
```html
  <div class="video-grid-item">
    {{< youtube ID-OF-VIDEO-HERE >}}
  </div>
```
This edit can be done through the browser, you can make a pull request or commit directly to the main branch if you are an admin. 
