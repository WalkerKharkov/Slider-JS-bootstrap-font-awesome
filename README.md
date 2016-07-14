# Slider-JS-bootstrap-font-awesome

This plug-in contains slider for review a images on your site. It is requires bootstrap3 and font-awesome.

Slideshow can be configured by using the following settings:

    controlsColor - contains color of slider controls.  default lightgray
    controlsActiveColor - contains color of slider active control. default #B34EE9
    counter - contains start opacity of first slide image. default 0
    imgPath - contains path, where are the images. default "img/"
    startindex - contains number of image, which will start slideshow. default 0
    delay - contains value of animation delay (show/hide image). default 50
    colorDelay - contains active control change color delay time. default null
    pause - contains the time for which the picture on the screen is delayed. default 40
    elem - contains DOM element that is the parent of the slider. default document.body
    title - contains information about show/hide the hint for images (boolean). default false
    
Object "images" contains data of images: name, alt, href attribute and title. It's required argument.    
    
    Example of using:
    
    var images = {
        "0" : {
            "name" : "1.jpg",  
            "alt" : "image 1",
            "href" : "",
            "title" : "image 1"
        },
        "1" : {
            "name" : "2.jpg",
            "alt" : "image 2",
            "href" : "http://www.gogle.com",
            "title" : "google image"
        }
    };
    
    var settings = {                         // settings are optionally. you can use all, several or nothing settings
        "controlsColor": "red",
        "imgPath" : "img/",
        "elem" : document.querySelector("#img")
    };
    
    

    var slider = new Slider (images, settings);
