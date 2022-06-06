# Workbench 1.x CSS
CSS Style Destined to look like Workbench 1.x [Live Demo](https://xproot.github.io/Workbench1CSS/)

## Usage

Import the [css file](https://raw.githubusercontent.com/xproot/Workbench1CSS/main/workbench1.css) by first downloading it and then import it however you desire.
Below are two ways.

- In the html file, on the <head> part, add this 
```
<link rel="stylesheet" type="text/css" href="workbench1.css">  
```
- In your main CSS file, on the first line, add this
```
@import url('workbench1.css');  
```
---
 
**By the way:** The [**Topaz New**](https://www.dafont.com/topaz-new.font) font is recommended, use it by adding 
```
@font-face {
    font-family: "Topaz";
    src: url(/assets/fonts/TopazNew.ttf);
    font-display: swap;
}

  (...)
 
html, body { 
(...)
  font-family: Topaz, Arial, Helvetica, sans-serif; 
(...)
}
```

---
  
In order to use the stylesheet by its fullest, Your body should look like this
```
<body>
  <div class="topbar">
    <span>Example GitHub File</span><span class="margin">Text with margin</span>   
    (Optional)
    <div class="buttons">
      <img alt="Disabled" width="25" height="20" src="wb1.gif"><img alt="Disabled" width="28" height="20" src="wb2.gif"> 
    </div>
    (You'll have to upload the images to your webserver)
  </div>
</body>
```
  
That will give you a bar like this
  
![image](https://user-images.githubusercontent.com/49620652/172032152-d39fe635-f599-49d9-bc38-c5f0ac5c1125.png)


In order to add windows you should follow this Template
```
<div class="window">
  <div class="titlebar">
    <span>Title</span>
    (Optional)
    <div class="buttons">
      <img alt="Disabled" width="25" height="20" src="wb1.gif"><img alt="Disabled" width="28" height="20" src="wb2.gif">
    </div>
    (You'll have to upload the images to your webserver)
  </div>
  <div class="content">
    Content
  </div>
</div>
```
Our Document should look like this now
  
![image](https://user-images.githubusercontent.com/49620652/172032161-385d2547-c641-47f6-8c6d-ceb0f33e30e6.png)

In order to make the window to take up all the free space, we're going to add the ```fullwidth``` class to the ```<div class="window">``` element
  
```
<div class="fullwidth window">
  <div class="titlebar">
    <span>Title</span>
    (Optional)
    <div class="buttons">
      <img alt="Disabled" width="25" height="20" src="wb1.gif"><img alt="Disabled" width="28" height="20" src="wb2.gif">
    </div>
    (You'll have to upload the images to your webserver)
  </div>
  <div class="content">
    Content
  </div>
</div>
```
  
![image](https://user-images.githubusercontent.com/49620652/172032192-48bf21db-e928-45cf-b9a4-2569a636f868.png)
  
Nice! Now one more last thing, to hide the scrollbars you should add the ```noscroll``` class to the ```<div class="content">``` element
  
```
<div class="fullwidth window">
  <div class="titlebar">
    <span>Title</span>
    (Optional)
    <div class="buttons">
      <img alt="Disabled" width="25" height="20" src="wb1.gif"><img alt="Disabled" width="28" height="20" src="wb2.gif">
    </div>
    (You'll have to upload the images to your webserver)
  </div>
  <div class="noscroll content">
    Content
  </div>
</div>
```
  ![image](https://user-images.githubusercontent.com/49620652/172032238-db37419e-79b3-495c-9f29-72e1a4724c0f.png)
