CircleIndicator
===============
a lightweight viewpager indicator! 

![inside mode]( https://github.com/ky0615/CircleIndicator/blob/master/demo/inside.gif)    

![outside mode]( https://github.com/ky0615/CircleIndicator/blob/master/demo/outside.gif)    

![solo mode]( https://github.com/ky0615/CircleIndicator/blob/master/demo/solo.gif)    

Usage
--------

import on gladle:


in default build.gradle

```gradle
allprojects {
    repositories {
        mavenCentral()
        maven { url "https://ky0615.github.io/maven/" }
    }
}
```

in added app's gradle:
```gradle

dependencies {
    compile 'ky0615:android-circle-indicator:1.1.0'
}

```


xml:

```xml
	<ws.temp.circleindicator.widget.CircleIndicator
        android:layout_width="match_parent"
        android:layout_height="40dp"
        android:layout_centerVertical="true"
        android:id="@+id/indicator"
        CircleIndicator:ci_background="@android:color/white"
        CircleIndicator:ci_selected_background="@android:color/black"
        CircleIndicator:ci_mode="outside"
        CircleIndicator:ci_gravity="center"
        CircleIndicator:ci_radius="10dp"
        CircleIndicator:ci_margin="5dp"
        />
```

java:

```java
        circleIndicator.setViewPager(viewPager);
```

--------
Notice:the method should be called after ViewPager.setAdapter().    

#####Properties:

* `app: ci_radius` :indicator's radius
* `app: ci_margin` :margin between two indicators
* `app: ci_background`:indicator's background
* `app: ci_selected_background`:selected indicator's background
* `app: ci_gravity`:indicator's layout gravity,support left,center and right.
* `app: ci_mode`:indicator's change mode when viewpager scrolled


License
--------
```
Copyright (C) 2016 Koutarou Yabe
Copyright (C) 2014 relex

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
