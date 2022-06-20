# Audio, Video, Images



## [Video and Audio Content](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content)

**Explain how the ability to use video and audio on the web has evolved since the early 2000s.**   
To use video and audio content there were plugins that were needed that didnt work well with html and css as well as having security issues. It wasn't a very easy thing to use.  
**Describe the use of the src and controls attributes in the `<video>` element.**  
the src attribute provides the path to the video you would like to link. Controls allow the user to control the playback however they prefer.  
**Why is it important to have fallback content inside the `<video>` element?**  
- For accesibility readers
- In case the video doesn't load or is taken down theres some context.
- There's a link to bookmark the video for later. 
<br>
**[A Complete Guide To Grid](https://css-tricks.com/snippets/css/complete-guide-grid/)**  

**How does Grid layout differ from Flex?**    
- Flexbox can optionally wrap
- Flex box can make rows and columns but you really only get more control over one of those things.
- grid is defined on the parent. Flexbox is mostly on the children
- grid is better at overlapping
- Grid is sturdier
- flexbox can push things away
**Grid container, grid item, and grid line are a few important terms to understand when using Grid. Please describe these terms in a few sentences.**    
>**Grid container**: The element on which display: grid is applied. It’s the direct parent of all the grid items. In this example container is the grid container. 
````
<div class="container">
  <div class="item item-1"> </div>
  <div class="item item-2"> </div>
  <div class="item item-3"> </div>
</div>
````
>**Grid Item**: The children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but sub-item isn’t.  
````
  <div class="container">
  <div class="item"> </div>
  <div class="item">
    <p class="sub-item"> </p>
  </div>
  <div class="item"> </div>
</div>
````
> **Grid Line**: The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column. Here the yellow line is an example of a column grid line.  


## [Responsive Images](https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images)  

**Besides making a site visually appealing across different screen sizes, why should developers make images responsive?**  
**Define the following `<img>` attributes srcset and sizes. Write an example of how they are used.**  
**How is srcset more helpful for responsive images than CSS or JavaScript?**  
