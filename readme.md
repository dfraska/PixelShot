# PixelShot
[![](https://img.shields.io/badge/API-19%2B-brightgreen.svg?style=flat)](https://android-arsenal.com/api?level=19)
[![APK](https://img.shields.io/badge/Download-Demo-brightgreen.svg)](https://github.com/Muddz/PixelShot/raw/master/demo.apk)

PixelShot is an awesome Android library that can save any `View` or `SurfaceView` as an image in `JPG`,`PNG` or `.nomedia`  
The library works on a asynchronous and handles errors of I/O operations and memory handling for you. 

## Example of simplest usage:

Filename will be named from a timestamp.   
Path will default to `/Pictures` in internal storage.   
Image format will default to `.JPG`

```java
   PixelShot.of(view).setResultListener(this).save();
```

## Example of a detailed usage:
```java
    PixelShot.of(view).setResultListener(this)
                      .setFilename("Hello World")
                      .setPath("MySickApp/media/pictures")
                      .toPNG()
                      .save();
```
    
### THERE ARE SOME PROBLEMS IN BINTRAY MAKING IT NOT AVAILABLE AT THE MOMENT! (22 Sept 2018)
## Installation

Add the dependency in your `build.gradle`
```groovy
dependencies {
    implementation 'com.muddzdev:pixelshot:1.0.0'  
}
```
 ----

## License

    Copyright 2018 Muddi Walid

    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License
    You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.
