# Usage

## 1. 环境准备

### 开发工具
- `Android Studio`
- `NDK`

### 拷贝头文件
下载或clone[MNN](https://github.com/alibaba/MNN)代码，拷贝头文件到`app/include`目录下；

示例：
```
git clone https://github.com/alibaba/MNN
cp MNN/include /path/to/MNNExample/mobilenet/android/app/
```

### 拷贝库文件
从[MNN Release](https://github.com/alibaba/MNN/releases)中下载最新的`mnn_xxx_android_armv7_armv8_cpu_opencl_vulkan.zip`并解压，将文件夹下的库文件拷贝到`app/libs`目录下；

示例：
```
wget https://github.com/alibaba/MNN/releases/download/2.4.0/mnn_2.4.0_android_armv7_armv8_cpu_opencl_vulkan.zip
unzip mnn_2.4.0_android_armv7_armv8_cpu_opencl_vulkan.zip
cp mnn_2.4.0_android_armv7_armv8_cpu_opencl_vulkan/arm* /path/to/MNNExample/mobilenet/android/app/libs
```


### 模型下载：
从[Release](https://github.com/wangzhaode/mobilenet-mnn/releases/tag/v1.0)下载模型文件，并放在工程中的assets文件夹（Android视图）或者resources文件夹（Project视图）中

## 2. 编译运行

使用`Android Studio`打开`demo`目录，在`local.properties`中指定`sdk.dir`与`ndk.dir`，即可编译执行。
