:star2: Camera2Scanner <font color=#0366d6 size=4 >Version 1.0.1</font>
============================

## 目录
* [功能介绍](#功能介绍)
* [更新计划](#更新计划)
* [版本记录](#版本记录)

## 功能介绍
Android平台基于[zBar](https://github.com/ZBar/ZBar)的开源扫码框架，要求<font color=#0366d6>SDK21</font>及以上。 

-  使用camera2API
-  自动对焦
-  扫描界面可任意定制

## 更新计划
-  针对<font color=#0366d6>SDK21</font>及以上，优化camera2API的使用。
-  针对<font color=#0366d6>SDK21</font>以下，提供旧的cameraAPI的支持。
-  增加Zxing支持。

## 版本记录
-  V1.0.2   `2018/03/14`

    1. 新增抽象类`GraphicDecoder`，将条码解析模块进行抽离。
    2. 新增`ZBarDecoder`，采用ZBar解析条码，并增加解析类型及解析精度设置。
    3. 修改`ScannerFrameView`，扫描线动画由属性动画实现。
    4. 修改`Camera2Scanner`，修复释放相机可能导致的异常，增加扫描框区域设置。
    5. 其他微调。

-  V1.0.1   `2018/02/09`

    1. 新增`ScannerFrameLayout`，为`RelativeLayout`的子类，可对扫描框的位置和大小进行设置。
    2. 修改`ScannerFrameView`，可对扫描框内部进行定制。
    
-  V1.0.0

    初次提交代码。
