
# RxCore
 Rasterex Web SDK Core

 Pro version 35.5

### 1 Added new method for controlling Annotation visibility on startup RxCore.markupDisplayOnload(onOff) onOff = boolean if true annotations are displayed when the file is loaded if false they are not displayed.

 Pro version 35

### 1 Added support for PDF annotation conversion to Rasterex markup.
### 2 New method for drawing revision polygon.
### 3 Fixed fill for measure rectangle.
### 4 New method to upload modified local PDF.


Pro version 33.993

### 1. Added new method RxCore.hideMarkupByMarkupNumbers(markupNumbers, onOff)
    Takes an array of markupnumbers and set the display property on or off.
    
### 2. Added new property on Markup object this.takeOffObject 
    Default value will be undefined.

 Pro version 33.992
 Basic version 36.00


## Updated in these versions.

Latest code merges and fixes and new methods as of October 30.

Pro

### 1. Thumbnails was not generated for all pages, fixed.
### 2. New method to set Markup user and display name.

    RxCore.setUser(szsign, szdisplayname);
    Require that defalutconfig.xml has value
        <CanChangeSignature>True</CanChangeSignature>

### 3. Configuration updated to support setting user name on startup.
### 4. Code merge for stamp support.
### 5. Code merge for new scaling support.

Basic

### 5. Code merge for new scaling support.





 
