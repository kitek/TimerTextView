# TimerTextView
Simple self updated timer TextView

[ ![Download](https://api.bintray.com/packages/kitek/maven/TimerTextView/images/download.svg) ](https://bintray.com/kitek/maven/TimerTextView/_latestVersion)

## How to install

```
repositories {
  jcenter()
}
dependencies {
  compile 'pl.kitek:timertextview:0.0.2'
}
```

## How to use

your_layout.xml
```
<pl.kitek.timertextview.TimerTextView
        android:id="@+id/timerText"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_centerInParent="true"
        android:drawableLeft="@drawable/ic_timer"
        android:drawablePadding="4dp"
        android:gravity="center"
        android:textSize="24sp"/>
```

YourActivity.java
```java
long futureTimestamp = System.currentTimeMillis() + (10 * 60 * 60 * 1000);
TimerTextView timerText = (TimerTextView) findViewById(R.id.timerText);
timerText.setEndTime(futureTimestamp);
```

## Example

<img src="https://raw.githubusercontent.com/kitek/TimerTextView/master/example.gif" width="256">
