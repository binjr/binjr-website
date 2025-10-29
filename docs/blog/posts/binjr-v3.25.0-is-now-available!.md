---
draft: false
date:
  created: 2025-10-29
  updated: 2025-10-29
image: assets/images/binjr_card.png
tags:
  - News
  - Releases
  - v3.25.0
authors:
  - binjr
categories:
  - binjr
  - New releases
comments: true
---
# [binjr v3.25.0](https://github.com/binjr/binjr/releases/tag/v3.25.0) is now available! 🎉
Released on Wed, 29 Oct 2025
<!-- more -->

### What's new?
* _[New] [Dependencies]_ Updated the embedded runtimes for Java and JavaFX to version 25.0.1.  
* _[New] [Dependencies]_ Source and target compatibility level for binjr's artifacts have been updated to 25.  
* _[New] [JVM GC Logs Adapter]_ Added support for ZGC garbage collector logs.  
* _[New] [CSV Adpater]_ CSV parser now supports comments.  
* _[New] [CSV Adapter]_ Only use localized number parser if mandated in a parsing profile, as the unlocalized parser is more lenient.  
* _[New] [HTTP Adapters]_ User Agent string can now be overridden.  
* _[New] [UI]_ Added a user preference to select the default timeline display mode on charts.  
* _[Fixed] [Installers]_ MacOS PKG installer does not associate the ".bjr" extension to binjr.  
* _[Fixed] [Core]_ Extra TemporalField endless loop when using adjustInto method.  
* _[Fixed] [HTTP Adapters]_ SSL context builder ignores user certificate keystore when validating certification paths on Windows and MacOS.  
* _[Fixed] [CSV Adapter]_ The wrong field is highlighted when the time pattern field is empty in CSV parsing profile dialog.  
* _[Fixed] [CSV Adapter]_ The number parser only takes three decimal digits into account when parsing CSV data.  
* _[Fixed] [CSV Adapter]_ The number parser does not recognize lower case 'e' as an exponent symbol when override locale for number parsing.  



### Links
* [Download]( https://binjr.eu/download/latest_release/)
* [Getting starting](https://binjr.eu/documentation/getting-started/)
* [Report an issue](https://github.com/binjr/binjr/issues)