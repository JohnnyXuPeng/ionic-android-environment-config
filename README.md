
配置ionic安卓打包环境

1.安装Node.js:https://nodejs.org/en/
安装后测试当前版本
node -v
npm -v

2.安装ionic
npm install -g ionic
安装后测试当前版本
ionic -version

3.安装cordova
npm install -g cordova
安装后测试当前版本
cordova -version

4.安装java JDK
下载地址:http://www.oracle.com/technetwork/java/javase/downloads/index.html
安装到C:\Java路径下
右键我的电脑-属性-高级-环境变量-系统变量-Path-编辑-新建
C:\Java\jre1.8.0_131\bin
安装后测试当前版本
java -version

5.创建ionic项目
创建ionic1：ionic start MyApp --type=ionic1(不需要运行该命令)
创建ionic2：ionic start MyApp

6.在浏览器中运行
ionic serve

7.安装android SDK
https://developer.android.com/studio/index.html?hl=zh-cn(安装组件时需要开代理)
右键我的电脑-属性-高级-环境变量-系统变量-新建
系统变量名:ANDROID_HOME
系统变量值:D:\Android_SDK
右键我的电脑-属性-高级-环境变量-系统变量-Path-编辑-新建
D:\Android_SDK\platform-tools
D:\Android_SDK\tools
D:\Android Studio\gradle\gradle-3.2\bin

8.添加android平台
cordova platform add android

9.打包成app
cordova build android
