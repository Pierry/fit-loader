fit-loader (forked - Loading)
================
Loading is a poject with kinds of Android loading view.

Yan can see the wiki for more detail.

[RotateLoading](https://github.com/yankai-victor/Loading/wiki/RotateLoading)

![RotateLoading](https://github.com/yankai-victor/Loading/blob/master/images/RotateLoading.gif)

Usage
=======

XML:

    <RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    	xmlns:tools="http://schemas.android.com/tools"
    	xmlns:app="http://schemas.android.com/tools"
    	android:layout_width="match_parent"
    	android:layout_height="match_parent"
    	>
    	<com.github.pierry.fitloader.RotateLoading
      		android:id="@+id/rotateloading"
      		android:layout_width="80dp"
      		android:visibility="gone"
      		android:layout_height="80dp"
      		app:loading_width="5dp"
      		android:background="@android:color/transparent"
      		android:layout_centerInParent="true"
      	/>
      	<LinearLayout
      		android:layout_width="match_parent"
      		android:layout_height="match_parent"
      		android:id="@+id/ll"
      		android:orientation="horizontal"
      	>

Activity

    void showLoader() {
    	rotateloading.start(false);
    	rotateloading.setVisibility(View.VISIBLE);
    	ll.setVisibility(View.INVISIBLE);
    }
    void hideLoader() {
    	rotateloading.stop();
    	rotateloading.setVisibility(View.INVISIBLE);
    	ll.setVisibility(View.VISIBLE);
    }

Gradle
=======
To get a GitHub project into your build:

Step 1. Add the JitPack repository to your build file
Add it in your build.gradle at the end of repositories:

        repositories {
          // ...
          maven { url "https://jitpack.io" }
        }

Step 2. Add the dependency in the form

        dependencies {
          compile 'com.github.Pierry:Loading:v1.0'
        }
	
License
=======
Copyright 2015 yankai-victor

Licensed under the Apache License, Version 2.0 (the "License"); you may not use this work except in compliance with the License.
You may obtain a copy of the License in the LICENSE file, or at:

http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software distributed under the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
