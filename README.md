# Watermark Library to Android 

<a href='https://bintray.com/duanniston/repository/watermarklib/_latestVersion'><img src='https://api.bintray.com/packages/duanniston/repository/watermarklib/images/download.svg'></a>


```gradle
 repositories {
    jcenter()
    //This repository is not necessary, but if  jcenter() not work, add the line below 
     maven {
         url  "http://dl.bintray.com/duanniston/repository" 
     }
 }
 ```

```gradle
compile 'br.com.duanniston:watermarklib:0.0.5'
```


> minSdkVersion 16

## Usage

#### Generating watermark from XML (view)

```java
private Bitmap generateWaterMark(Bitmap src) {

 //src is your original image
 WaterMark waterMark = new WaterMark(mContext);
 //return the your original image with watermark added
 return waterMark.getImageWaterMarkFromView(src, R.layout.watermark_all);
}
```

```xml
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:layout_gravity="center"
    android:gravity="center"
    android:orientation="vertical">

<TextView
        android:layout_width="match_parent"
        android:layout_gravity="center"
        android:gravity="center"
        android:layout_height="match_parent"
        android:text="watermark" />
</LinearLayout>
```

# Licence

```
Copyright 2016 Duanniston Cabral

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
```


