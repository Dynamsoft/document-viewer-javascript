# Dynamsoft Document Viewer
![version](https://img.shields.io/npm/v/dynamsoft-document-viewer.svg)
![downloads](https://img.shields.io/npm/dm/dynamsoft-document-viewersvg) 
![jsdelivr](https://img.shields.io/jsdelivr/npm/hm/dynamsoft-document-viewer.svg)
![](https://img.shields.io/snyk/vulnerabilities/npm/dynamsoft-document-viewer.svg)

[Dynamsoft Document Viewer (DDV)](https://www.dynamsoft.com/document-viewer/docs/introduction/index.html) is an SDK designed to provide different types of viewers to configure and achieve different processing flows for documents. 

It contains two main features,

- Data Management
- Different types of viewers:
    - Edit Viewer
    - Capture Viewer
    - Perspective Viewer
    - Browse Viewer
    - Custom Viewer

Besides, DDV provides the methods to integrate with your own customized image filter process and document boundary detect process. 

- Image filter
- Document detection (Recommend using [Dynamsoft Document Normalizer](https://www.dynamsoft.com/document-normalizer/docs/web/programming/javascript/))

With DDV, you can easily and efficiently create a document manage web application which meets your different requirements of working flow, user interface, style.

## Table of Contents
- [System Requirements](#system-requirements)
- [License Key](#license-key)
- [Installation](#installation)
- [Deployment](#deployment)
- [Documentation](#documentation)
- [Features](#features)
- [Contact Us](#contact-us)
- [License Agreement](#license-agreement)
- [Changelog](#changelog)

# System Requirements

The SDK requires the following features to work:

- Secure context (HTTPS deployment)

  When deploying your application / website for production, make sure to serve it via a secure HTTPS connection. This is required for two reasons
  
  - Access to the camera video stream is only granted in a security context. Most browsers impose this restriction.
	> Some browsers like Chrome may grant the access for `http://127.0.0.1` and `http://localhost` or even for pages opened directly from the local disk (`file:///...`). This can be helpful for temporary development and test.
  
  - Dynamsoft License requires a secure context to work.

- `WebAssembly`, `Blob`, `URL`/`createObjectURL`, `Web Workers`

  The above four features are required for the SDK to work.

## License Key

[![](https://img.shields.io/badge/Get-30--day%20FREE%20Trial%20License-blue)](https://www.dynamsoft.com/customer/license/trialLicense/?product=ddv&utm_source=npm)

## Installation

- Dynamsoft website
	
    **Dynamsoft Document Viewer**
    
    [![](https://img.shields.io/badge/Download-Offline%20SDK-orange)](https://www.dynamsoft.com/document-viewer/downloads)

- NPM

    ```bash
    npm install dynamsoft-document-viewer
    ```

## Deployment

Dynamsoft Document Viewer relies on the files in the `/dist/` folder to work. Make sure to put these files on your server and correctly refer to them by specifying the path with [`Dynamsoft.DDV.setConfig()`](https://www.dynamsoft.com/document-viewer/docs/api/namespace/ddv.html#static-setconfig) (relative and absolute paths are both fine).

If you are making use of the `CDN` [jsDelivr](https://cdn.jsdelivr.net/npm/ddv), you will still need to host the `/dist/` folder somewhere on your server and refer to it by specifying the path with [`engineResourcePath`](https://www.dynamsoft.com/document-viewer/docs/api/interface/configuration.html#engineresourcepath) by using [`Dynamsoft.DDV.setConfig()`](https://www.dynamsoft.com/document-viewer/docs/api/namespace/ddv.html#static-setconfig). 


## Documentation

* [Developer's Guide](https://www.dynamsoft.com/document-viewer/docs/introduction/index.html)
* [API Reference](https://www.dynamsoft.com/document-viewer/docs/api/index.html)

## Features

Generally, the features of DDV can be divided to two parts as below.

### Data Management

Data management is to manage the data which is imported into DDV. It is managed from the following two aspects:

-	Document Management: Document creation/deletion/merging, etc.
-	Page management: Pages in documents loading/saving/deleting/moving, etc.

### Viewers

Viewers are used to display the data. According to the different uses of viewers, DDV provides five different viewer types, which are implemented through five viewer classes.

-	Edit Viewer: Edit the pages in document, such as, rotating, cropping, filtering, etc. and adjust the layout of the display.
-	Capture Viewer: Control camera, play video stream, and capture the images from camera.
-	Perspective Viewer: Do page boundary manual adjustment & perspective transformation.
-	Browse Viewer: Display pages in multiple-mode, pages can be multiple selected.
-	Custom Viewer: No built-in UI or functionality, which is used for creating your own viewer.


[More](https://www.dynamsoft.com/document-viewer/docs/features/index.html)

## Contact Us

[Contact Dynamsoft](https://www.dynamsoft.com/company/contact/) to resolve any issue you encounter with the library.

## License Agreement

https://www.dynamsoft.com/company/license-agreement/

## Changelog

Check out the [release notes](https://www.dynamsoft.com/document-viewer/docs/releasenotes/index.html) of the Dynamsoft Document Viewer.


