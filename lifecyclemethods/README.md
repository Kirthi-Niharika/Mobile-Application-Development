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
Developed by: T . Kirthi Niharika
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
![image](https://github.com/Kirthi-Niharika/Mobile-Application-Development/assets/114135005/db18267e-121d-4281-b5b5-b22c37bb3ff7)
![image](https://github.com/Kirthi-Niharika/Mobile-Application-Development/assets/114135005/1156770f-2c5d-4dff-9577-88c96df65eec)
![image](https://github.com/Kirthi-Niharika/Mobile-Application-Development/assets/114135005/51ee0973-aa19-4000-8229-045e0e422b34)
![image](https://github.com/Kirthi-Niharika/Mobile-Application-Development/assets/114135005/a121dccb-f5a6-4cb2-9429-fae16799da6f)
![image](https://github.com/Kirthi-Niharika/Mobile-Application-Development/assets/114135005/d39bf0a9-c578-45b3-8ac9-c63cfb0ba5b7)
![image](https://github.com/Kirthi-Niharika/Mobile-Application-Development/assets/114135005/ab9589c8-76bf-498f-a59f-d78c79464c2b)




## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
