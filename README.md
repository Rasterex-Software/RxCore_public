Pro version 35.82.
### 1 Latest version.

Basic version 36.1
### 1 Synchronized with Pro version. Some new features are not compatible.

Pro version 35.79

### 1. Added watermark functionality (addWatermarkToPage, addWatermarkToAllPages and removeWatermarkFromAllPages)

### 2. Add annotation storage service.
### 3. Store annotations to bakcend db.
### 4. Added new image sub types returned by markup.getMarkupType(), RxCore.getMarkupTypes() and RxCore.getMarkupType(type, subtype)
### 5. Fixed issues for machines using non 1:1 screen resolution
   ### - Drop of image or stamp on pdf page page extent calculation issue.
   ### - Scaling of annotation on pdf page page extent calculation issue.
### 6. Fixed a problem with annotations being selected when swithcing user allowed annotation to be moved by non owning user.
### 7. Selection of annotation with negative widht or height now works.
### 8. RxCore.GUI_2DEntityInfoScreen and RxCore.GUI_2DEntityInfo callbacks now return whole block object instead of only the name.





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





 
