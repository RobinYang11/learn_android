# learn android
## 开发工具 android studio
## 模拟器 Genymotion 
# Activity
## 概念
	Activity 就是一个可视化的用户界面，负责创建一个屏幕窗口，放置组件，供用户交互。
## 用法
. 创建你的Activity类
. 在androidManifest.xml中注册该类
. 设置布局文件
## android 文件结构
### manifests 应用程序清单文件，
	AndroidManifest.xml
###  java  所有java 源代码文件
###  res 资源文件夹 
#### drawable 
#### mipmap 图标文件
#### values  键值对资源
#### 以及布局资源
# 创建Activity 
. 1 在java 文件夹下创建一个MyActivity 该类继承自android.app的activity
. 2 在manifest中注册activity 
	<activity android:name=".Myactivity">
		<action android:name="android.intent.MAIN"/>
		<catergory android:name="android.intent.catergory.LAUNCHER"/>
	</activity>
. 3.创建布局资源文件夹 layout 必须使用layout 这个名字 ，如果使用其他会报错
	 在该文件夹下创建布局文件 myLayout.xml
	 该文件有2个显示方式design 是视图界面，text 是 文件	
	 <textView 
	 	android:layout_width="warp_content"
		android:layout_height="warp_content"
		android:text="Hello RObin EDU/>
. 4 在java中的onCreate中调用setContentView(R.layout.myLayout);
# androidManiffest.xml的作用
## 概念
	 他是应用程序的清单文件，每个应用都必须包含，位于应用根目录下
##  作用：
. 1. 他描述了程序的基本属性
. 2. 他描述了应用程序需要使用的权限
. 3. 描述包含的应用组件的实现类

