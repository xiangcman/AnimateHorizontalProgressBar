# AnimateHorizontalProgressBar
[![Platform](https://img.shields.io/badge/platform-android-green.svg)](http://developer.android.com/index.html)

A tiny Android library makes very easier ProgressBar anitmation horizontal. 

# Usage

Include the AnimateHorizontalProgressBar widget in your layout.

```xml

    <com.daasuu.library.AnimateHorizontalProgressBar
        android:id="@+id/animate_progress_bar"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        app:ahp_backgroundColor="@color/colorPrimaryDark"
        app:ahp_progressColor="@color/colorAccent" />

```
In your onCreate method (or onCreateView for a fragment), bind the widget and set default value.
```JAVA

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        
        AnimateHorizontalProgressBar progressBar = (AnimateHorizontalProgressBar) findViewById(R.id.animate_progress_bar);
        progressBar.setMax(1000);
        progressBar.setProgress(400);
    }

```
Animate ProgressBar with setProgress
```JAVA
    progressBar.setProgressWithAnim(800);
```
Animate ProgressBar with setMax
```JAVA
    progressBar.setMaxWithAnim(2000);
```

# Gradle

Add the dependency to your build.gradle.

```
dependencies {
    compile 'com.daasuu:animateHorizontalProgressBar:0.1.3'
}
```

## License

Copyright 2015 MasayukiSuda

MIT License

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

