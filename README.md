# UnfoldAndZoomScrollView

## 此项目已经更新，采取更优的方式实现，请移步
HeadZoomLayout(https://github.com/old-traveler/HeadZoomLayout)

~~仿QQ个人信息详情界面中背景图的下拉扩展放大功能，仅供学习使用。

![img](https://github.com/old-traveler/HeadZoomScrollView-master/blob/master/img/20170503173531271.gif)

可直接用于你的项目

Add it in your root build.gradle at the end of repositories:

Step 1.

	allprojects {
		repositories {
			...
			maven { url 'https://jitpack.io' }
		}
	}

Step 2.

	dependencies {
		 compile 'com.github.old-traveler:HeadZoomScrollView-master:1.0.0'
	}


使用方法：



<com.mrw.headzoomscrollview.UnfoldAndZoomScrollView

    android:layout_width="match_parent"
    android:layout_height="match_parent">

    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        android:orientation="vertical"
        android:fitsSystemWindows="true">
         //扩展放大的控件可为ImageView或其他布局、控件
        <ImageView
            android:fitsSystemWindows="true"
            android:id="@+id/iv"
            android:layout_width="match_parent"
            android:layout_height="400dp"
            android:scaleType="centerCrop"
            />

        <LinearLayout
            android:background="?android:attr/selectableItemBackground"
            android:clickable="true"
            android:focusable="true"
            android:layout_width="match_parent"
            android:layout_height="50dp">
            <TextView
                android:background="#ffffff"
                android:layout_width="match_parent"
                android:layout_height="match_parent" />

        </LinearLayout>

    </LinearLayout>

</com.mrw.headzoomscrollview.UnfoldAndZoomScrollView>


博客地址:http://blog.csdn.net/qq_34379015/article/details/71124450
