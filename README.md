# CustomImageView
Simply, we add **CircleImage** into layout.xml file.
```
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context="com.example.ongnau.customimageview.MainActivity">

    <com.example.ongnau.customimageview.CircleImage
        android:layout_width="@dimen/dp_300"
        android:layout_height="@dimen/dp_300"
        android:id="@+id/image_heart"
        app:border_color="@color/colorPrimary"
        android:layout_gravity="center_horizontal"
        android:src="@drawable/her"/>
</LinearLayout>
```
After that,in your activity, we just call **showImage()** to show circle image.
```
 @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        CircleImage image = findViewById(R.id.image_heart);
        image.showImage();
    }
```
