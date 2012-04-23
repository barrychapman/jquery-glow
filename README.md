jquery-glow
===========

Allows animation of text-shadow (textShadow) property on $.animate

Note: this requires jquery.ui.js

Demo
====

For a fancy glow effect that fades in and out, use the following code:

```javascript
$(document).ready(function() {
    $("#basic").click(function() { 
        $('.text').animate({color: "#ffffff;", textShadow: "0 0 15px #ccc;"}, 
            1000,
            function() { 
                $('.text').animate({ color: "#AFACAF;", textShadow: "0 0 0 #fff;"}, 1000);
            }
        );
    });
});
```

Demo available at: http://jsfiddle.net/barrychapman/qa5z7/