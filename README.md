# CSS backdrop-filter polyfill

**Demo:** https://ahsane.github.io/backdrop-polyfill-chrome/index.html

Backdrop filter polyfill for browsers that do not support it

#### Safari already has backdrop-filter support, so this is not needed for it.

## Documentation
First add the script
`<script src="backdrop-polyfill-chrome.js"></script>`

Then use the API
`backdrop(backdropsource, backdropapply, blur, scroller)`

backdropsource: The dom element where backdrop is going to be applied from

backdropapply: The dom element where backdrop is going to be applied to

blur: The amout of blur (equivalent to `backdropfilter: blur`)

scroller: `(string [yes/no])` Keep this to *yes*. 

Example: `backdrop(document.documentElement.outerHTML, document.getElementById('xx'), 20, "yes");`

- **Current limitation:** This works only for static content. 
