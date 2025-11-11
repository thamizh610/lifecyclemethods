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
Developed by: THAMIZARASAN S
Registeration Number : 212223220116
*/
```
# activity_main.xml
```
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
        android:text="Hello World"
        android:textColor="#673AB7"
        android:textColorHighlight="#0A1013"
        android:textColorHint="#4A3F3F"
        android:textColorLink="#2F3D43"
        android:textSize="34sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.179" />

```
# Mainactivity.java
```
package com.example.exp1;
import android.os.Bundle;
import android.widget.Toast;
import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast = Toast.makeText(getApplicationContext(), "onCreate Called", Toast.LENGTH_LONG);
        toast.show();
    }
    protected void onStart() {
        super.onStart();
        Toast toast = Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG);
        toast.show();
    }
    @Override

    protected void onRestart() {
        super.onRestart();
        Toast toast = Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onPause() {
        super.onPause();
        Toast toast = Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onResume(){
        super.onResume();
        Toast toast = Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onStop() {
        super.onStop();
        Toast toast = Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG);
        toast.show();

    }
    protected void onDestroy() {
        super.onDestroy();
        Toast toast = Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG);
        toast.show();

    }
}
```

## OUTPUT
<img width="397" height="735" alt="image" src="https://github.com/user-attachments/assets/929ada25-4214-482e-aa96-c2fe2341b856" />
<img width="422" height="730" alt="image" src="https://github.com/user-attachments/assets/dadef7c5-2ab9-4194-b7d9-4456929eaaba" />
<img width="409" height="739" alt="image" src="https://github.com/user-attachments/assets/3889aa34-442b-4e39-8179-c9010ed476d2" />
<img width="383" height="742" alt="image" src="https://github.com/user-attachments/assets/ed3497e9-2743-4dcf-bdd5-7aa072cceb7d" />
<img width="397" height="736" alt="image" src="https://github.com/user-attachments/assets/9d9f3000-1ab7-4bf1-9688-b5bf47c1d0d0" />
<img width="384" height="736" alt="image" src="https://github.com/user-attachments/assets/c14f6dca-e559-4c01-9bf2-a6cc0c0ab278" />
<img width="381" height="717" alt="image" src="https://github.com/user-attachments/assets/2f606ce5-1087-44d9-9a49-9d818a962b75" />


## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.
