# Getting started

There are two ways to get up and running with ***binjr***; download a ready-made application bundle for your OS and CPU achitecture, 
or build it yourself from sources.

## Download an application bundle

The simplest way to start using ***binjr*** is to download an application bundle from the [download page](../download/latest_release.md).

These bundles contain all the dependencies required to run the app, including a copy of the Java runtime specially
crafted to only include the required components and save disk space.

## Build from source

You can also build or run the application from the source code.

### Prerequisites:

* [Git](https://git-scm.com/open)
* [OpenJDK 25 or later](https://adoptium.net/marketplace/)

!!! Info "Optional"
    If you want to build native installer packages, you'll also need the following platform specific prerequisites: 
    
    === "Linux (.deb)"
        * Debian package archive manipulation tool (dpkg-deb)
    
    === "Linux (.rpm)"
        * RPM Package Manager
        
    === "macOS (.dmg)"
        * Xcode command line tools.
    
    === "Windows (.msi)"
        * [WiX 6.0.0 or later](https://github.com/wixtoolset/wix/releases/tag/v6.0.2).


### Build

1. Clone the [repo from Github](https://github.com/binjr/binjr/): 
    ``` sh
    git clone https://github.com/binjr/binjr/
    ```
   
2. Use the included gradle wrapper to:

    - Build all the modules
    
        === "Linux / macOS"
            ``` sh
            sh gradlew build
            ```
          
        === "Windows"
            ``` bat
            gradlew.bat build
            ```
   
    - Build and start the application   
      
        === "Linux / macOS"
            ``` sh
            sh gradlew run
            ```
      
        === "Windows"
            ``` bat
            gradlew.bat run
            ```           

    - Build all application bundles for the platform on which you run the build     

        === "Linux / macOS"
            ``` sh
            sh gradlew clean packageDistribution  
            ```

        === "Windows"
            ``` bat
            gradlew.bat clean packageDistribution  
            ```
                   
        !!! Warning  
            Make sure you run the `clean` task in between two executions of a `package<...>`
            task in the same environment.
            
    - Build a specific application bundle for the platform on which you run the build
    
        === "Linux (.tar.gz)"
            ``` sh
            sh gradlew clean packageAsTar  
            ```
    
        === "Linux (.deb)"
            ``` sh
            sh gradlew clean packageAsDeb  
            ```
    
        === "Linux (.rpm)"
            ``` sh
            sh gradlew clean packageAsRpm  
            ```
    
        === "macOS (.tar.gz)"
            ``` sh
            sh gradlew clean packageAsMacApp  
            ```
    
        === "macOS (.dmg)"
            ``` sh
            sh gradlew clean packageAsDmg  
            ```
    
        === "Windows (.zip)"
            ``` bat
            gradlew.bat clean packageAsZip  
            ```
    
        === "Windows (.msi)"
            ``` bat
            gradlew.bat clean packageAsMsi  
            ```
          
        !!! Warning
            Please note that it is generally not possible to cross-build application bundles (e.g. build a bundle for
            macOS while running under Windows)  

## Trying it out

If you'd like to experience binjr's visualization capabilities but do not have a compatible data source handy, you can use
the [demonstration data adapter](https://github.com/binjr/binjr-adapter-demo).

It is a plugin which embeds a small, stand-alone data source that you can readily browse using ***binjr***.

1. Make sure ***binjr*** is installed on your system and make a note of the folder it is installed in.
2. Download the `binjr-adapter-demo-3.x.x.zip` archive from https://github.com/binjr/binjr-adapter-demo/releases/latest
3. Copy the `binjr-adapter-demo-3.x.x.jar` file contained in the zip file into the `plugins` folder of your
   ***binjr*** installation.
4. Start ***binjr*** (or restart it if it was runnning when you copied the plugin) and open the `demo.bjr`
   workspace contained in the zip (from the command menu, select `Workspaces > Open...`, or press Ctrl+O)

