

Rasterex Web SDK Core release notes


Pro version 37.28

### Fixed a problem with annotation fill style reading from RXML when using Hexadecimal colors.
### Fixed a problem with Arc measurement position when using RXML save and load.
### Added a new callback RxCore.GUI_Error that returns the error status and function name.


```javascript
RxCore.GUI_Error.connect(function (functionName, Error) {

    console.log("An error ", Error, " occured in ", functionName);
  
});
```

Pro version 37.27

### Fixed a problem with RxCore.setLineStyle where it affected the global line width.


Pro version 37.26
### New method RxCore.uploadOnlyPDF(), this uploads a PDF created in client to server. The method takes no parameters and uploads to the default upload folder.
### New method RxCore.uploadPDFOnlyCustom(endpoint), this uploads a PDF created in client to server using a custom endpoint.
### New callback RxCore.GUI_CacheCreated this returns 3 parameters OriginalURL, FileNameSRC and CacheURL. This callback is used in combination with new methods RxCore.uploadOnlyPDF and RxCore.uploadPDFOnlyCustom and will return the name of the file in the created cache folder and the url to the cache folder.

```javascript
    RXCore.onGuiCacheCreated((OriginalURL: string, FileNameSRC : string, CacheURL : string) => {
      console.log("cache created", FileNameSRC, OriginalURL, CacheURL );
    }); 
```

Pro version 37.25
### New method RxCore.openExtractedPageInViewer(fileName, pageNumber). This method can be used to create a new PDF  document in the viewer from a single page of a currently open PDF document. The new method takes two parameters, fileName and pageNumber. fileName is the name given to the new single page document, pageNumber is the 0 indexed page number from the original document that is to be used to create the new single page document. To use the new method the latest iframefoxit.js from this project is also needed.


Pro version 37.21

### Added check for when fixed scale value is set for a page before calculating annotaion dimensions.
### Added new magnifier object that can be used to create a panel in UI.
### Added option to use magnifier with overlay alignment.
### Added magnification support for PDF.
### Fixed, server side compare alignment values were not always correct depending on screen scaling.
### Fixed some issues with overlay compare alignment UI point stability.


Basic version 36.34

### No news.

Pro version 37.14
Basic version 36.34

### Undo - redo fix for text annotations.
### New watermark render fumction for unicode texts.



Pro version 37.12
Basic version 36.34

### Print update for PDF without visible paging.

Pro version 37.1
Basic version 36.34

### Added asynchronous page handling for printing PDF with Foxit.

Pro version 35.99
Basic version 36.34

### Fixed problem with drawing measurement and annoations on rotated PDF page.
### Added foxit iframe wrapper files

Pro version 35.95
Basic version 36.34

### Added possibility to use Legacy PDFJS tested with version 2.16.105

Pro version 35.95
Basic version 36.32

### Opening file on startup from defaultconfig.xml should now work again.

Pro version 35.95
Basic version 36.31

### Fixed problem with new moveable signature object.
### Fixed problem with area holes input output for XML and JSON.

Pro version 35.93
Basic version 36.3

### Synchronized PDFJS and Foxit versions with new methods.

Pro version 35.925
Basic version 36.3

### Support for new PDFJS module and new internal TextLayerbuilder.


Pro version 35.925
Basic version 36.24

### Added configuration option to disable markup rotation.


Pro version 35.925
Basic version 36.24

### Pro version - Fixed a problem related to opening large PDF from a URL
### Pro version - Disabled loading of PDF bookmarks automatically on file load to prevent problems with large number of Bookmarks.



Pro version 35.9
Basic version 36.22

### Basic version - Fixed a minor issue with continuous adding of notes where the size of the notes where resized when the adding of notes where terminated.

### Pro version - Fixed a problem related to touch events that caused a freeze on mobile devices.
### Pro version - Fixed a problem where the Foxit sub system called a function that caused a display problem for other open files of other formats.


Pro version 35.87
Basic version 36.21

### Fixed a minor issue with continuous adding of text that produced duplicates when clicking outside a created text without creating a new text annotation. Also fixed limitation when moving a free pen annotation.


Pro version 35.86
Basic version 36.2

### 1 Added support for continuous adding of text annotations using RxCore.markupAddMulti(true); This require use of new TextInputCtrl, new span based text input element in main.html template and AngularJS based UI.

Pro version 35.85
Basic version 36.12

### 1 Annotations should now be displayed on visible pages instead of earlier only on current page.


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





 
