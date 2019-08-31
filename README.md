# Project2-JS-and-Boostrap
Project 2 using JavaScript and Bootstrap to create a sample company website.

## Code Snippets
### Bootstrap CDN integration in `index.html`
```html
 <!-- Bootstrap CSS -->
    <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.3.1/css/bootstrap.min.css"
        integrity="sha384-ggOyR0iXCbMQv3Xipma34MD+dH/1fQ784/j6cY/iJTQUOhcWr7x9JvoRxT2MZw1T" crossorigin="anonymous">
```
### Function Handling the live preview of cars being selected from the dropdown menu:
```javascript
function carPreview(model) {
  let theKey = document.getElementById("carPreview");
  let forPrev = document.getElementsByClassName("forPreview");
  let theImgValue = document.getElementById("forChange").value;
  let theImage = document.getElementById("carDisplay");

  switch (theImgValue) {
    case "xm72": {
      theImage.src =
        "http://backgrounds4k.net/wp-content/uploads/2016/11/Tesla-Model-X-backgrounds-ultra-hd.jpg";
      break;
    }
    case "xm73": {
      theImage.src =
        "http://backgrounds4k.net/wp-content/uploads/2016/11/Tesla-Model-X-ultra-high-definition-backgrounds.jpg";
      break;
    }
    case "xm74": {
      theImage.src =
        "https://pixelz.cc/wp-content/uploads/2018/08/audi-r8-white-uhd-4k-wallpaper.jpg";
      break;
    }
    case "xm75u": {
      theImage.src =
        "http://wallpaperask.com/wp-content/uploads/Cars-full-hd-wallpapers-1080p-dowload.jpg";
      break;
    }
    case "xm76": {
      theImage.src =
        "http://backgrounds4k.net/wp-content/uploads/2016/11/BMW-i8-uhd-desktop.jpg";
      break;
    }
  }
```

### BootStrap function checking for validity of the input
```javascript
(function() {
  "use strict";
  window.addEventListener(
    "load",
    function() {
      // Fetch all the forms we want to apply custom Bootstrap validation styles to
      var forms = document.getElementsByClassName("needs-validation");
      // Loop over them and prevent submission
      var validation = Array.prototype.filter.call(forms, function(form) {
        form.addEventListener(
          "submit",
          function(event) {
            if (form.checkValidity() === false) {
              event.preventDefault();
              event.stopPropagation();
            }
            form.classList.add("was-validated");
          },
          false
        );
      });
    },
    false
  );
})();
```


### The live deployment can be viewed at https://sunilale0.github.io/Project2-JS-and-Boostrap/
