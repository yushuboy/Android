# facedetection

项目使用的余老师的[libfacedetection](https://github.com/ShiqiYu/libfacedetection)库进行人脸检测，已集合了opencv.

Just transport this lib to Andtoid and run successful with some optimization.

I also build an apk in the Android/release folder so you can just install on your android device to test it.

Modified cmakelist.txt for android and configures for opencv. So all you need to do is to add opencv for android to it and RUN IT.

Here is the steps for developers:

1. clone this porject and make sure cmake,ndk and lldb(if u need debug c++ code) is downloaded.

2. download opencv sdk for android from OpenCV-release.

3. import OpenCV-android-sdk/sdk/java to this porject as a module so android can use it.

4. copy opencv c++ header OpenCV-android-sdk/sdk/natvie/jni/include/opencv2 to this project libfacedetection/mobile/Android/app/src/main/cpp/ so jni can use it.

5. copy opencv libs OpenCV-android-sdk/sdk/natvie/libs/ and staticlibs OpenCV-android-sdk/sdk/natvie/staticlibs/ to this project direct libfacedetection/mobile/Android/app/src/main/jniLibs/ for compile.

6. run it!
 
