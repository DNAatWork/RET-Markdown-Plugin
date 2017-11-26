<!-- HTML CODE-->
<link rel="stylesheet" type="text/css" href="https://carlosvegame.github.io/RET-Markdown-Plugin/docs/demo/style.css"/>
<link type="text/css" rel="stylesheet" href="http://sachinchoolur.github.io/lightslider/dist/css/lightslider.min.css" />                  
<script src="//ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>
<script src="http://sachinchoolur.github.io/lightslider/src/js/lightslider.js"></script>



**This README.md file should be modified to describe the features, installation, configuration, and general usage of this plugin.**

The **ReT Md Editor** Plugin is for [Grav CMS](http://github.com/getgrav/grav). REader Text-editor (ReT.md), is a markdown editor plugin for grav themes, inspired from TinyMCE Editor grav plugin and pandao/editor.md.


<ul id="lightSlider">
  <li>
  <img src="docs/img2.png" class="slider-image" />
      <h3>First Slide</h3>
      <p>Lorem ipsum Cupidatat quis pariatur anim.</p>
  </li>
  <li>
      <h3>Second Slide</h3>
      <p>Lorem ipsum Excepteur amet adipisicing fugiat velit nisi.</p>
      <img src="docs/img3.png" class="slider-image" />
  </li>
  <li>
  <img src="docs/img4.png" class="slider-image" />
      <h3>Second Slide</h3>
      <p>Lorem ipsum Excepteur amet adipisicing fugiat velit nisi.</p>
  </li>
</ul>





## Installation

Installing the ReT Md Editor plugin can be done in one of two ways. The GPM (Grav Package Manager) installation method enables you to quickly and easily install the plugin with a simple terminal command, while the manual method enables you to do so via a zip file.


### GPM Installation (Preferred)

The simplest way to install this plugin is via the [Grav Package Manager (GPM)](http://learn.getgrav.org/advanced/grav-gpm) through your system's terminal (also called the command line).  From the root of your Grav install type:

    bin/gpm install ret-md-editor

This will install the ReT Md Editor plugin into your `/user/plugins` directory within Grav. Its files can be found under `/your/site/grav/user/plugins/ret-md-editor`.

### Manual Installation

To install this plugin, just download the zip version of this repository and unzip it under `/your/site/grav/user/plugins`. Then, rename the folder to `ret-md-editor`. You can find these files on [GitHub](https://github.com/githubid/grav-plugin-ret-md-editor) or via [GetGrav.org](http://getgrav.org/downloads/plugins#extras).

You should now have all the plugin files under

    /your/site/grav/user/plugins/ret-md-editor

> NOTE: This plugin is a modular component for Grav which requires [Grav](http://github.com/getgrav/grav) and the [Error](https://github.com/getgrav/grav-plugin-error) and [Problems](https://github.com/getgrav/grav-plugin-problems) to operate.

## Configuration

Before configuring this plugin, you should copy the `user/plugins/ret-md-editor/ret-md-editor.yaml` to `user/config/plugins/ret-md-editor.yaml` and only edit that copy.

Here is the default configuration and an explanation of available options:

```yaml
enabled: true
```

## Usage

**Describe how to use the plugin.**

## Credits

**Did you incorporate third-party code? Want to thank somebody?**

## To Do

- [ ] Remake demo
- [ ] add options
- [ ] Clean Code
- [ ] Add theme css, rm defualt css


<script type="text/javascript">
$(document).ready(function() {
    $("#lightSlider").lightSlider({
        item: 3,
        autoWidth: false,
        slideMove: 1, // slidemove will be 1 if loop is true
        slideMargin: 10,

        addClass: '',
        mode: "slide",
        useCSS: true,
        cssEasing: 'ease', //'cubic-bezier(0.25, 0, 0.25, 1)',//
        easing: 'linear', //'for jquery animation',////

        speed: 400, //ms'
        auto: false,
        loop: false,
        slideEndAnimation: true,
        pause: 2000,

        keyPress: false,
        controls: true,
        prevHtml: '',
        nextHtml: '',

        rtl:false,
        adaptiveHeight:false,

        vertical:false,
        verticalHeight:500,
        vThumbWidth:100,

        thumbItem:10,
        pager: true,
        gallery: false,
        galleryMargin: 5,
        thumbMargin: 5,
        currentPagerPosition: 'middle',

        enableTouch:true,
        enableDrag:true,
        freeMove:true,
        swipeThreshold: 40,

        responsive : [],

        onBeforeStart: function (el) {},
        onSliderLoad: function (el) {},
        onBeforeSlide: function (el) {},
        onAfterSlide: function (el) {},
        onBeforeNextSlide: function (el) {},
        onBeforePrevSlide: function (el) {}
    });
});
</script>
