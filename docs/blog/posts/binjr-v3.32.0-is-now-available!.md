---
draft: false
date:
  created: 2026-11-20
  updated: 2026-11-20
image: assets/images/binjr_card.png
tags:
  - News
  - Releases
  - v3.32.0
authors:
  - binjr
categories:
  - binjr
  - New releases
comments: true
---
# [binjr v3.32.0](https://github.com/binjr/binjr/releases/tag/v3.32.0) is now available! 🎉
Released on Fri, 20 Nov 2026
<!-- more -->

### What's new?
* _[New] [CSV]_ Fetching data from a CSV file with large number of individual data points is now much faster and uses less memory.  
* _[New] [CSV]_ Added a built-in profile for CSV values indexed by line numbers (i.e. without timestamps).  
* _[New] [Dependencies]_ Updated the embedded Java runtime to 25.0.5.1 (November security update)
* _[New] [UI]_ Panning or zooming on a chart using the mouse wheel now feels smoother and more responsive.  
* _[New] [Core]_ Automatically infer parallelism based on available processors.
* _[Fixed] [Core]_ Charts are not refreshed when adding series to an empty chart whose default time range is the same as the one currently selected.  
* _[Fixed] [UI]_ Reordering charts or timeseries on a worksheet using drag and drop no longer works.  

### Links
* [Download]( https://binjr.eu/download/latest_release/)
* [Getting starting](https://binjr.eu/documentation/getting-started/)
* [Report an issue](https://github.com/binjr/binjr/issues)