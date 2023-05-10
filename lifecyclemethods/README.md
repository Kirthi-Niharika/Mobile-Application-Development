# Ex.No:1 To create a HelloWorld Activity using all lifecycles methods to display messages.


## AIM:

To create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:

Step 1: Open Android Stdio and then click on File -> New -> New project.

Step 2: Then type the Application name as HelloWorld and click Next. 

Step 3: Then select the Minimum SDK as shown below and click Next.

Step 4: Then select the Empty Activity and click Next. Finally click Finish.

Step 5: Design layout in activity_main.xml.

Step 6: Display message give in MainActivity file.

Step 7: Save and run the application.

## PROGRAM:
```
/*
Program to print the text “Hello World”.
Developed by: T.Kirthi Niharika
Registeration Number : 212221040084
*/
```
activity_main.xml

<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Hello World!"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

</androidx.constraintlayout.widget.ConstraintLayout>

MainActivity.java
package com.example.appl1;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnCreate Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onStart() {
        super.onStart();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnStart Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onResume() {
        super.onResume();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnResume Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onPause() {
        super.onPause();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnPause Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onRestart() {
        super.onRestart();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnRestart Executed",Toast.LENGTH_LONG);
        t2.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        setContentView(R.layout.activity_main);
        Toast t2= Toast.makeText(getApplicationContext(),"OnDestroy Executed",Toast.LENGTH_LONG);
        t2.show();
    }
}



## OUTPUT
<img width="887" alt="Screenshot 2023-05-10 114520" src="https://github.com/suryacse05/Mobile-Application-Development/assets/114135005/106da0b0-6122-46a0-bd99-7db71af65e40">
<img width="897" alt="Screenshot 2023-05-10 114626" src="https://github.com/suryacse05/Mobile-Application-Development/assets/114135005/eda5069b-b5b8-4049-8f96-f55b7359475b">
<img width="903" alt="Screenshot 2023-05-10 115109" src="https://github.com/suryacse05/Mobile-Application-Development/assets/114135005/c99daa9b-eba1-4fe0-8254-155d8172aca9">
<img width="898" alt="Screenshot 2023-05-10 115209" src="https://github.com/suryacse05/Mobile-Application-Development/assets/114135005/54d32429-6d11-4aa2-b361-e31f990b10bf">
<img width="188" alt="Screenshot 2023-05-10 115209" src="https://github.com/suryacse05/Mobile-Application-Development/assets/114135005/25db7a33-93f6-48e9-a652-058d79c585db">

<img width="178" alt="Screenshot 2023-05-10 114626" src="https://github.com/suryacse05/Mobile-Application-Development/assets/114135005/43b94b0c-fed4-4478-9edf-afd1aef0ebc8">


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
