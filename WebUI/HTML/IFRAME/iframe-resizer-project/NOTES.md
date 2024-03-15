


Frame not downsizing
The most likely cause of this problem is having set the height of an element to be 100% of the page somewhere in your CSS. This is normally on the html or body elements, but it could be on any element in the page. This can sometimes be got around by using the taggedElement height calculation method and added a data-iframe-height attribute to the element that you want to define the bottom position of the page. You may find it useful to use position: relative on this element to define a bottom margin or allow space for a floating footer.

Not having a valid HTML document type in the iFrame can also sometimes prevent downsizing. At it's most simplest this can be the following.

<!DOCTYPE html>
IFrame not resizing
The most common cause of this is not placing the iframeResizer.contentWindow.min.js script inside the iFramed page. If the other page is on a domain outside your control and you can not add JavaScript to that page, then now is the time to give up all hope of ever getting the iFrame to size to the content. As it is impossible to work out the size of the contained page, without using JavaScript on both the parent and child pages.