---
draft: false
date:
  created: 2026-10-26
  updated: 2026-10-26
image: assets/images/binjr_card.png
tags:
  - News
  - Releases
  - v3.31.0
authors:
  - binjr
categories:
  - binjr
  - New releases
comments: true
---
# [binjr v3.31.0](https://github.com/binjr/binjr/releases/tag/v3.31.0) is now available! 🎉
Released on Mon, 26 Oct 2026
<!-- more -->

### What's new?

* _[New] [UI]_ Linked worksheets that are not visible are no longer refreshed immediately when the timeline change, but only when they become visible again. This greatly speeds up rendering for the worksheets that *are* visible.  
* _[New] [Flatpak]_ The file picker dialog box now uses the system Desktop Environment and honors theming.  
* _[New] [Core]_ Changed default garbage collector tuning, in order to increase performances on large queries, at the expense of being less eager to release uncommitted memory to the OS.  
* _[New] [Dependencies]_ Replaced GCToolkit with GCSee as the dependency used for parsing JVM GC logs.  
* _[New] [Dependencies]_ Updated embedded runtime (Java 25.0.5 / JavaFX 27.0.1)  

### Links
* [Download]( https://binjr.eu/download/latest_release/)
* [Getting starting](https://binjr.eu/documentation/getting-started/)
* [Report an issue](https://github.com/binjr/binjr/issues)