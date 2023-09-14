# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

## EQUIPMENTS REQUIRED:

Latest Version Android Studio

## ALGORITHM:


## PROGRAM:
```
/*
Program to print the text “GUIcomponent”.
Developed by: PRADEEPASRI S
Registeration Number : 212221220038
*/
```
## activitymain.xml
```
<?xml version="1.0" encoding="utf-8"?> 
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android" 
    xmlns:app="http://schemas.android.com/apk/res-auto" 
    xmlns:tools="http://schemas.android.com/tools" 
    android:layout_width="match_parent" 
    android:layout_height="match_parent" 
    tools:context=".MainActivity"> 
 
    <TextView 
        android:id="@+id/textView" 
        android:layout_width="339dp" 
        android:layout_height="124dp" 
        android:text="GOOGLE" 
        android:fontFamily="cursive" 
        android:textAlignment="center" 
        android:textSize="80sp" 
        app:layout_constraintBottom_toBottomOf="parent" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toTopOf="parent" 
        app:layout_constraintVertical_bias="0.36" />
 <Button 
        android:id="@+id/button" 
        android:layout_width="120dp" 
        android:layout_height="120dp" 
        android:text="COLOUR" 
        app:layout_constraintBottom_toBottomOf="parent" 
        app:layout_constraintEnd_toStartOf="@+id/button2" 
        app:layout_constraintHorizontal_bias="0.515" 
        app:layout_constraintStart_toStartOf="parent" 
        app:layout_constraintTop_toTopOf="parent" 
        app:layout_constraintVertical_bias="0.706" />
<Button 
        android:id="@+id/button2" 
        android:layout_width="120dp" 
        android:layout_height="120dp" 
        android:layout_marginEnd="56dp" 
        android:text="FONT" 
        app:layout_constraintBottom_toBottomOf="parent" 
        app:layout_constraintEnd_toEndOf="parent" 
        app:layout_constraintTop_toTopOf="parent" 
        app:layout_constraintVertical_bias="0.706" /> 
</androidx.constraintlayout.widget.ConstraintLayout>
```
## MainActivity.java
```
package com.example.guiapplication; 
 
import android.graphics.Color; 
import android.graphics.Typeface; 
import android.os.Bundle; 
import android.view.View;                                                                                                                               
import android.widget.Button; 
import android.widget.TextView; 
import androidx.appcompat.app.AppCompatActivity; 
 
public class MainActivity extends AppCompatActivity { 
 
    private TextView textView; 
    private Button colorButton; 
    private Button fontButton; 
 
    @Override 
    protected void onCreate(Bundle savedInstanceState) { 
        super.onCreate(savedInstanceState); 
        setContentView(R.layout.activity_main); 
 
        // Initialize UI elements 
        textView = findViewById(R.id.textView); 
        colorButton = findViewById(R.id.button); 
        fontButton = findViewById(R.id.button2); 
 
        // Set click listeners for buttons 
        colorButton.setOnClickListener(new View.OnClickListener() { 
            @Override 
            public void onClick(View view) { 
                // Change text color to a random color 
                int randomColor = Color.rgb( 
                        (int)(Math.random() * 256), 
                        (int)(Math.random() * 256), 
                        (int)(Math.random() * 256) 
                );                         
                textView.setTextColor(randomColor); 
            } 
        }); 
 
        fontButton.setOnClickListener(new View.OnClickListener() { 
            @Override 
            public void onClick(View view) { 
                // Change text font to a different typeface 
                Typeface newFont = Typeface.create("monospace", Typeface.BOLD); 
                textView.setTypeface(newFont); 
            } 
        }); 
    } 
} 
 
``` 
## OUTPUT
![Screenshot (81)](https://github.com/suryacse05/Mobile-Application-Development/assets/131433142/3fb92e57-8172-4e22-9101-5d2cac6a901e)
![Screenshot (82)](https://github.com/suryacse05/Mobile-Application-Development/assets/131433142/23b9fae3-3dee-4880-a304-85af6ed49ece)

## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.


