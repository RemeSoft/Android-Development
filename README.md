# Android-Development
This repository is all about andoid development. There I will try to solve all common andoid development probelm.

## How to remove Titlebar
First go to res > themes > themes.xml than set style NoActionBar.
```XML
<style name="Theme.RannaGhor" parent="Theme.MaterialComponents.DayNight.NoActionBar">
```
## How to change statusbar color and it's text color.
First go to themes.xml and add this line.
```XML
<item name="android:statusBarColor">@color/white</item>
```
Then go to it's java file and add those line.
```java
if (Build.VERSION.SDK_INT >= Build.VERSION_CODES.M) {
    getWindow().getDecorView().setSystemUiVisibility(View.SYSTEM_UI_FLAG_LIGHT_STATUS_BAR);
}
getWindow().setStatusBarColor(ContextCompat.getColor(this,R.color.white));
```

## How To create round buttons.
In XML file add those lines.
```XML
<com.google.android.material.button.MaterialButton
    app:cornerRadius="10dp"
 ```

