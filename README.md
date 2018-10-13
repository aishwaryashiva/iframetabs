# iframetabs
iFrame Tabs is a JQuery based solution for implementing a tab-based interface on web-pages. It forces the specified links on the web-pages to open the page inside an iframe based tab.

## How to use?
1. Include JQuery and FontAwesome first.
```
<script src="https://code.jquery.com/jquery-1.12.4.min.js" type="text/javascript"></script>
<script defer src="https://use.fontawesome.com/releases/v5.0.8/js/all.js"></script>
```
2. Now include iFrameTabs JavaScript file and Stylesheet file.
```
<script src="iframetabs.js"></script>
<link rel="stylesheet" type="text/css" media="screen" href="iframetabs.css" />
```
3. Now use following code where you want to add tab interface:
```
<div id="wrapper">
        <ul id="tabs">
            <!--these are the tabs that will be visible by default.-->
            <li class='current'><a class='tab' id='pages' href='#'>All Pages</a></li>
        </ul>
 <div id="content">
     <!--For each tab, add a div here with id=(Tab link id from above + _content)-->
     <div id="pages_content" class="tabdata">
     <!--any content here-->
     <!--Links with class="tablink" will be opened in another tab.-->
         <a href="page1.html" class="tablink">Page 1</a>
         <!--any content here-->
     </div>
 </div>
</div>
```
4. Now initialize iFrameTabs using following code:
```
<script>
  $(document).ready(function(){
     bindTabLinks();
  });
</script>
```
