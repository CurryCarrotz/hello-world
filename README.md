<?xml version="1.0" encoding="utf-8"?>
<RelativeLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="@drawable/image_background"
    tools:context=".EditProfileActivity">

    <android.support.design.widget.AppBarLayout
        android:id="@+id/app_bar_layout"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        app:elevation="0dp">

        <android.support.v7.widget.Toolbar
            android:id="@+id/edit_profile_toolbar"
            android:layout_width="match_parent"
            android:layout_height="wrap_content"
            android:theme="@style/ThemeOverlay.AppCompat.Dark.ActionBar">

            <TextView
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:layout_marginEnd="50dp"
                android:layout_marginRight="50dp"
                android:gravity="center"
                android:text="Edit Profile"
                android:textAlignment="center"
                android:textColor="@color/colorGeneralText"
                android:textSize="25sp" />
        </android.support.v7.widget.Toolbar>
    </android.support.design.widget.AppBarLayout>

    <ScrollView
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:layout_below="@+id/app_bar_layout">

        <RelativeLayout
            android:layout_width="match_parent"
            android:layout_height="wrap_content">

        <RelativeLayout
            android:id="@+id/profile_banner"
            android:layout_width="411dp"
            android:layout_height="239dp"
            android:background="@drawable/profile_picblur">

            <RelativeLayout
                android:id="@+id/image_wrapper"
                android:layout_width="wrap_content"
                android:layout_height="wrap_content"
                android:layout_centerHorizontal="true"
                android:layout_marginTop="100dp">

                <ImageView
                    android:id="@+id/profile_Pic"
                    android:layout_width="150dp"
                    android:layout_height="150dp"
                    android:scaleType="centerInside"
                    android:src="@drawable/profile_pic" />

                <ImageButton
                    android:id="@+id/button_ProfilePic"
                    android:layout_width="wrap_content"
                    android:layout_height="wrap_content"
                    android:layout_marginLeft="110dp"
                    android:layout_marginTop="100dp"
                    android:background="@color/colorTransparent"
                    android:src="@drawable/camera" />

            </RelativeLayout>
        </RelativeLayout>


        <LinearLayout
            android:layout_width="fill_parent"
            android:layout_height="match_parent"
            android:layout_below="@+id/profile_banner"
            android:orientation="vertical"
            android:padding="8dp">

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content"
                android:orientation="horizontal">

                <TextView
                    android:id="@+id/user_label"
                    android:layout_width="fill_parent"
                    android:layout_height="wrap_content"
                    android:layout_gravity="center"
                    android:layout_marginLeft="10dp"
                    android:layout_weight="50"
                    android:text="User Name"
                    android:textSize="20sp" />

                <TextView
                    android:id="@+id/user_name"
                    android:layout_width="fill_parent"
                    android:layout_height="wrap_content"
                    android:layout_marginRight="10dp"
                    android:layout_weight="50"
                    android:gravity="right"
                    android:text="Marko01"
                    android:textAlignment="gravity"
                    android:textSize="20sp" />
            </LinearLayout>

            <View
                android:id="@+id/profile_list_bottom_border"
                android:layout_width="match_parent"
                android:layout_height="2dp"
                android:background="#B9B9B9"
                />

            <LinearLayout
                android:layout_width="match_parent"
                android:layout_height="wrap_content">

                <TextView
                    android:id="@+id/firstName_label"
                    android:layout_width="fill_parent"
                    android:layout_height="wrap_content"
                    android:layout_gravity="center"
                    android:layout_marginLeft="10dp"
                    android:layout_weight="50"
                    android:text="User Name"
                    android:textSize="20sp" />

                <TextView
                    android:id="@+id/firstName_value"
                    android:layout_width="fill_parent"
                    android:layout_height="wrap_content"
                    android:layout_marginRight="10dp"
                    android:layout_weight="50"
                    android:gravity="right"
                    android:text="Marko01"
                    android:textAlignment="gravity"
                    android:textSize="20sp" />

            </LinearLayout>
        </LinearLayout>
        </RelativeLayout>
    </ScrollView>
</RelativeLayout>
