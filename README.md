# bringins
 jQuery plugin to show contents on a webpage as an animated page
<br>
Developed by Arun Thomas
<br>
www.ajarunthomas.com
<br>
<br>
<a href="http://www.ajarunthomas.com/jquery/bringins/demo/" target="_blank" style="text-decoration:none">Demo</a>
<a download href="http://www.ajarunthomas.com/jquery/bringins/js/bringins.js" target="_blank" style="text-decoration:none">Download</a>
<br><br>
<a href="http://www.ajarunthomas.com/jquery/bringins/" target="_blank" style="text-decoration:none">Website</a>
##USAGE
###Step 1 : Include js
```
<script type="text/javascript" src="js/jquery-1.12.0.min.js"></script>
<script type="text/javascript" src="js/bringins.js"></script>
```
###Step 2 : create your content to be shown as a bringins page
```
<div id="sampledata" class="bringins-content">
    Your content goes here...
</div>
```
Note : You can define your custom CSS for this content and make sure you have included the 'bringins-content' class
###Step 3 : Activate the plugin
```
$(document).ready(function() {
    $('#sampledata').bringins();
});
```
this will bring up the page once the DOM is loaded
### more options
In the below example we will specify the plugin to initiate on mouse click
```
$(document).ready(function() {  
    $('#btn').click(function(){
        $('#sampledata').bringins({
            "position":"center",    //animation of the bringins page
            "color":"black",    //background color of the page
            "closeButton":"white",  //color of the close button
            "width":"100%", //width of the bringins page
            "margin":100,   //margin of the content inside the page
            "zIndex":999    //z-index of the page
        });
    });     
}); 
```
