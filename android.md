# Appium 环境搭建 Mac

## appium
~~~ shell
npm install appium
npm install appium-doctor

# 下载Android Studio 可以配置安卓环境
export JAVA_HOME=$(/usr/libexec/java_home)
export PATH=$PATH:${JAVA_HOME}/bin
export ANDROID_HOME=/Users/bzy/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/tools:$ANDROID_HOME/platform-tools
~~~
