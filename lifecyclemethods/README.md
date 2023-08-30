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
Developed by: S.PRADEEPASRI
Registeration Number : 212221220038
*/
```
## activity_main.xml:

```
   <?xml version="1.0" encoding="utf-8"?>
    <androidx.constraintlayout.widget.ConstraintLayoutxmlns:
android="http://schemas.android.com/apk/res/android"
        xmlns:app="http://schemas.android.com/apk/res-auto"
        xmlns:tools="http://schemas.android.com/tools"
        android:layout_width="match_parent"
        android:layout_height="match_parent"
        tools:context=".MainActivity">

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="HELLO WORLD!"
        android:textSize="40sp"
        android:textStyle="bold"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
    </androidx.constraintlayout.widget.ConstraintLayout>
```

 ## MainActivity.java:
 ```

 package com.example.helloworld;

import androidx.appcompat.app.AppCompatActivity;

import android.os.Bundle;
import android.util.Log;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

@Override
protected void onCreate(Bundle savedInstanceState) {
    super.onCreate(savedInstanceState);
    setContentView(R.layout.activity_main);

    // Display toast message when the activity is created
    Toast.makeText(getApplicationContext(), "onCreate Invoked", Toast.LENGTH_LONG).show();
}

@Override
protected void onStart(){
    super.onStart();
    Toast.makeText(getApplicationContext(), "onStart Invoked", Toast.LENGTH_LONG).show();
}

@Override
protected void onPause(){
    super.onPause();
    Toast.makeText(getApplicationContext(), "onPause Invoked", Toast.LENGTH_LONG).show();
}

@Override
protected void onResume(){
    super.onResume();
    Toast.makeText(getApplicationContext(), "onResume Invoked", Toast.LENGTH_LONG).show();
}

@Override
protected void onStop(){
    super.onStop();
    Toast.makeText(getApplicationContext(), "onStop Invoked", Toast.LENGTH_LONG).show();
}

@Override
protected void onRestart(){
    super.onRestart();
    Toast.makeText(getApplicationContext(), "onRestart Invoked", Toast.LENGTH_LONG).show();
}

@Override
protected void onDestroy(){
    super.onDestroy();
    Toast.makeText(getApplicationContext(), "onDestroy Invoked", Toast.LENGTH_LONG).show();
}
```

## OUTPUT
![Screenshot (16)](https://github.com/suryacse05/Mobile-Application-Development/assets/131433142/18b6648e-69c8-4809-a961-8709726e3558)


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
