# powr-notifications
POWR Notification Bar


Place these lines in the ```<head> ```



```<!-- jQuery --><script src="https://code.jquery.com/jquery-3.4.1.min.js"></script>```


```<!-- Notification Banner JS --><script src="/src/jquery.notificationbanner.min.js"></script>```

2. download and Unzip the src folder from the repository and drop it in the site root, so it's accessible on sitename.com/src/ 

3. Place the following immediately after the ```<body>``` opening tag:

```<div class="notificationHeader"></div>```

4. Paste the following in the ```<head>``` of the site: 
```
<script>
(function($){
         function makeItNotified(){
                  $(".notificationHeader").notificationBanner({
                           text: "Brand new site coming soon...",
                           position: "top",
                           background: "#d8a500"
                  });
         }
         $(document).ready(makeItNotified);
})(jQuery);
</script>
