---
draft: false
date:
  created: 2025-11-29
  updated: 2025-11-29
image: assets/images/binjr_card.png
tags:
  - News
  - Releases
  - v3.26.0
authors:
  - binjr
categories:
  - binjr
  - New releases
comments: true
---
# [binjr v3.26.0](https://github.com/binjr/binjr/releases/tag/v3.26.0) is now available! 🎉
Released on Sat, 29 Nov 2025
<!-- more -->

### What's new?
* _[New] [UI]_ Added new chart types as possible data representation for time series data:
    * Impulse charts: vertical bars with a height proportional to value being plotted.  
    * Vertical markers: to mark a series of instants on the timeline, as vertical lines that takes up the whole height of a chart.  
    * Duration markers: to represent durations as vertical bands with a width proportional to the duration being plotter.  
* _[New] [UI]_ Added an option to highlight the 'current' column the table view (which displays the Y values for each series on the selected chart at the time currently marked by the crosshair).
* _[Fixed] [UI]_ NaN value show as phantom sample in top left corner of scatter charts.  
* _[Fixed] [JVM GC Logs Adapter]_ Heap generation sizes are not extracted from G1 GC logs.  
* _[Fixed] [JVM GC Logs Adapter]_ GC allocation rate calculation is incorrect.  
* _[Fixed] [Core]_ Pressing `Reset Time Range` sometimes fails to correctly identify the lowest timestamp for the current series.  
* _[Fixed] [CSV, Logs]_ Timestamp parsing in CSV and Log file adapters ignore timezone offsets.  

### Links
* [Download]( https://binjr.eu/download/latest_release/)
* [Getting starting](https://binjr.eu/documentation/getting-started/)
* [Report an issue](https://github.com/binjr/binjr/issues)