# Self hosting  


http://google.github.io/material-design-icons/#icon-font-for-the-web  
http://alistapart.com/article/the-era-of-symbol-fonts  
https://github.com/google/material-design-icons/blob/master/iconfont/codepoints  
https://material.io/guidelines/style/icons.html  
https://material.io/icons/  



```codes
@font-face {
  font-family: 'Material Icons';
  font-style: normal;
  font-weight: 400;
  src: url(https://example.com/MaterialIcons-Regular.eot); /* For IE6-8 */
  src: local('Material Icons'),
       local('MaterialIcons-Regular'),
       url(https://example.com/MaterialIcons-Regular.woff2) format('woff2'),
       url(https://example.com/MaterialIcons-Regular.woff) format('woff'),
       url(https://example.com/MaterialIcons-Regular.ttf) format('truetype');
}
``` 

```codes
.material-icons {
    font-family: 'Material Icons';
    font-weight: normal;
    font-style: normal;
    font-size: 24px;  /* Preferred icon size */
    display: inline-block;
    line-height: 1;
    text-transform: none;
    letter-spacing: normal;
    word-wrap: normal;
    white-space: nowrap;
    direction: ltr;

    /* Support for all WebKit browsers. */
    -webkit-font-smoothing: antialiased;
    /* Support for Safari and Chrome. */
    text-rendering: optimizeLegibility;

    /* Support for Firefox. */
    -moz-osx-font-smoothing: grayscale;

    /* Support for IE. */
    font-feature-settings: 'liga';
}
``` 

```codes
# new browser
<i class="material-icons">face</i>
# old browser
<i class="material-icons">&#xE87C;</i>
``` 

```codes
/* Rules for sizing the icon. */
.material-icons.md-18 { font-size: 18px; }
.material-icons.md-24 { font-size: 24px; }
.material-icons.md-36 { font-size: 36px; }
.material-icons.md-48 { font-size: 48px; }

/* Rules for using icons as black on a light background. */
.material-icons.md-dark { color: rgba(0, 0, 0, 0.54); }
.material-icons.md-dark.md-inactive { color: rgba(0, 0, 0, 0.26); }

/* Rules for using icons as white on a dark background. */
.material-icons.md-light { color: rgba(255, 255, 255, 1); }
.material-icons.md-light.md-inactive { color: rgba(255, 255, 255, 0.3); }

``` 

```codes
# size (default === 24px)
<i class="material-icons">face</i>

<i class="material-icons md-18">face</i>
<i class="material-icons md-24">face</i>
<i class="material-icons md-36">face</i>
<i class="material-icons md-48">face</i>

# color (Normal/Disabled)

# light background & dark foreground color
<i class="material-icons md-dark">face</i>
<i class="material-icons md-dark md-inactive">face</i>

# dark background & light foreground color
<i class="material-icons md-light">face</i>
<i class="material-icons md-light md-inactive">face</i>
``` 

```codes
# custom icon color

.material-icons.orange600 { color: #FB8C00; }

<i class="material-icons orange600">face</i>
``` 

