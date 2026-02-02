---
draft: false
date:
  created: 2026-02-02
  updated: 2026-02-02
image: assets/images/binjr_card.png
tags:
  - News
  - Releases
  - v3.28.0
authors:
  - binjr
categories:
  - binjr
  - New releases
comments: true
---
# [binjr v3.28.0](https://github.com/binjr/binjr/releases/tag/v3.28.0) is now available! 🎉
Released on Mon, 2 Feb 2026
<!-- more -->

### What's new?
_[New] [Dependencies]_ Updated the embedded runtimes for Java and JavaFX to version 25.0.2.
_[Fixed] [Flatpak]_ Disable in-app update checks when the binjr runs as a flatpak.  
_[Fixed] [Flatpak]_ The "System" UI theme ignores system-wide color scheme setting when binjr runs as a flatpak.  
_[Fixed] [Flatpak]_ Config files should not be stored outside the application's sandbox.
_[Fixed] [UI]_ On Linux, changes to system-wide color scheme while binjr is running isn't reflected by the "System" UI theme.  
_[Fixed] [Core]_ Built-in plugins are loaded twice on startup.  
_[Fixed] [Core]_ Changing UI theme should only be attempted on the main FX thread.   


### Links
* [Download]( https://binjr.eu/download/latest_release/)
* [Getting starting](https://binjr.eu/documentation/getting-started/)
* [Report an issue](https://github.com/binjr/binjr/issues)