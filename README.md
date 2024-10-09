# Bottom-Navigation-Fab-Button-




make menu


```bash

<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto">



    <item android:id="@+id/home_btm"
        android:icon="@drawable/home"
        android:title="Home"

        />


    <item android:id="@+id/search_btm"
        android:icon="@drawable/search"
        android:title="search"

        />

    <item android:id="@+id/gas_btm"
        android:icon="@drawable/gas"
        android:title="Gas"

        />


    <item android:id="@+id/add_btm"
        android:icon="@drawable/add"
        android:title="Add"

        />

</menu>

```

xml 

```bash


<?xml version="1.0" encoding="utf-8"?>
<androidx.coordinatorlayout.widget.CoordinatorLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"
    android:background="#01579B">




    <com.google.android.material.bottomappbar.BottomAppBar
        android:id="@+id/bottomAppBar"
        android:layout_width="match_parent"
        android:layout_height="?attr/actionBarSize"
        android:layout_gravity="bottom"
        android:background="@color/white"
        app:fabAlignmentMode="center"
        app:fabAnchorMode="cradle"
        app:fabCradleRoundedCornerRadius="@dimen/_30sdp"
        app:menu="@menu/botton_item"

        >

    </com.google.android.material.bottomappbar.BottomAppBar>


    <com.google.android.material.floatingactionbutton.FloatingActionButton
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:background="@color/white"
        app:layout_anchor="@id/bottomAppBar"
        android:src="@drawable/add"
        app:fabSize="normal"
        android:layout_margin="16dp"
        />


</androidx.coordinatorlayout.widget.CoordinatorLayout>


```



