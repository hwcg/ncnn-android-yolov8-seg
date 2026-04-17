我正在智谱大模型开放平台 BigModel.cn上打造AI应用，智谱新一代旗舰模型GLM-5已上线， 在推理、代码、智能体综合能力达到开源模型 SOTA 水平，通过我的邀请链接注册即可获得 2000万Tokens 大礼包，期待和你一起在BigModel上畅享卓越模型能力；链接：https://www.bigmodel.cn/invite?icode=AWIPeACitCqDzTPVT%2BksTAZ3c5owLmCCcMQXWcJRS8E%3D


# ncnn-yolov8-seg


This is a sample ncnn yolov8 object segment android project, it depends on **ncnn** library and **opencv**.

Method 1

- [How to convert yolov8 model to ncnn model?](https://github.com/Digital2Slave/ncnn-android-yolov8-seg/wiki/Convert-yolov8-model-to-ncnn-model)

Method 2

- [Convert yolov8‐seg to ncnn model step by step](https://github.com/Digital2Slave/ncnn-android-yolov8-seg/wiki/Convert-yolov8%E2%80%90seg-to-ncnn-model-step-by-step)

Method 3

- ~~`ultralytics 8.0.129` add YOLOv8 Tencent NCNN export #3529 https://github.com/ultralytics/ultralytics/pull/3529~~


## 1 How to build and run

### 1.1 Configure ncnn

* Download [ncnn-YYYYMMDD-android-vulkan.zip](https://github.com/Tencent/ncnn/releases).
* Extract **ncnn-YYYYMMDD-android-vulkan.zip** into **app/src/main/jni** folder and change the **ncnn_DIR** path to yours in **app/src/main/jni/CMakeLists.txt**.

> For example:`ncnn-20221128-android-vulkan`

### 1.2 Configure OpenCV

* Download [opencv-mobile-XYZ-android.zip](https://github.com/nihui/opencv-mobile)
* Extract **opencv-mobile-XYZ-android.zip** into **app/src/main/jni** and change the **OpenCV_DIR** path to yours in **app/src/main/jni/CMakeLists.txt**.

> For example:`opencv-mobile-4.6.0-android`

### 1.3 Build and Install ncnn-yolov8-seg app

* Open this project with Android Studio, build it and enjoy!

## 2 Some notes

* Android ndk camera is used for best efficiency.
* Crash may happen on very old devices for lacking HAL3 camera interface.
* All models are manually modified to accept dynamic input shape.
* Most small models run slower on GPU than on CPU, this is common.
* FPS may be lower in dark environment because of longer camera exposure time.

## 3 Screenshot

![](./doc/20230209114529.jpg)

## 📊 GitHub Stats

![Alt](https://repobeats.axiom.co/api/embed/2f94ce240c907726c07fcf1cf97263edbf003997.svg "Repobeats analytics image")

## 🔗 Reference

- https://github.com/ultralytics/ultralytics 
- https://github.com/Tencent/ncnn
- https://github.com/nihui/opencv-mobile
- https://github.com/nihui/ncnn-android-nanodet 
- https://github.com/FeiGeChuanShu/ncnn-android-yolov8
