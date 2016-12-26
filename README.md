Android-ExpandIcon
================

Nice and simple customizable implementation of Google style up/down arrow.

![image](https://github.com/zagum/Android-ExpandIcon/blob/master/art/expand_icon_demo.gif)

Compatibility
-------------

This library is compatible from API 15 (Android 4.0.3).

Download
--------

Add it in your root build.gradle at the end of repositories:

```groovy
allprojects {
    repositories {
        ...
        maven { url "https://jitpack.io" }
    }
}
```

Add the dependency

```groovy
dependencies {
    compile ''
}
```

Usage
-----

Default implementation:

```xml
    <com.github.zagum.expandicon.ExpandIconView
        android:layout_width="24dp"
        android:layout_height="24dp"/>
```

Fully customized implementation:

```xml
    <com.github.zagum.expandicon.ExpandIconView
        android:layout_width="24dp"
        android:layout_height="24dp"
        app:animationDuration="300"
        app:color="#000"
        app:colorLess="@color/colorPrimary"
        app:colorMore="@color/colorAccent"
        app:roundedCorners="false"
        app:switchColor="true"/>
```

Public methods: 

```java
    expandIconView.switchState();
    
    expandIconView.setState(ExpandIconView.LESS, true);
    
    expandIconView.setFraction(.3f, true);
```

See sample project for more information

License
-------

    Copyright 2016 Evgenii Zagumennyi
    
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
    
    http://www.apache.org/licenses/LICENSE-2.0
    
    Unless required by applicable law or agreed to in writing, software
    distributed under the License is distributed on an "AS IS" BASIS,
    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
    See the License for the specific language governing permissions and
    limitations under the License.