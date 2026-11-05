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

### Program to print the text “Hello World”.
### Developed by: DIVYA PRIYA S
### Registeration Number : 212225240037


### MainActivity.java
```
package com.example.lifecycleactivity;

import android.os.Bundle;
import android.widget.Toast;

import androidx.appcompat.app.AppCompatActivity;

public class MainActivity extends AppCompatActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        Toast toast=Toast.makeText(getApplicationContext(),"onCreate Called", Toast.LENGTH_LONG)
        toast.show();
    }

    @Override
    protected void onStart() {
        super.onStart();
        Toast toast=Toast.makeText(getApplicationContext(), "onStart Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onRestart() {
        super.onRestart();
        Toast toast=Toast.makeText(getApplicationContext(), "onRestart Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onResume() {
        super.onResume();
        Toast toast=Toast.makeText(getApplicationContext(), "onResume Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onPause() {
        super.onPause();
        Toast toast=Toast.makeText(getApplicationContext(), "onPause Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onStop() {
        super.onStop();
        Toast toast=Toast.makeText(getApplicationContext(), "onStop Called", Toast.LENGTH_LONG)
        toast.show();
    }
    protected void onDestroy() {
        super.onDestroy();
        Toast toast=Toast.makeText(getApplicationContext(), "onDestroy Called", Toast.LENGTH_LONG)
        toast.show();
    }

}

 
```
### activity_main_xml

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/main"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:layout_width="199dp"
        android:layout_height="25dp"
        android:autoSizeTextType="none"
        android:fontFamily="sans-serif-black"
        android:text="Hello Everyone"
        android:textAlignment="center"
        android:textColor="#1131D9"
        android:textSize="20sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.473" />

    <TextView
        android:id="@+id/textView"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:fontFamily="sans-serif-black"
        android:text="Welcome to Life Cycle Activity"
        android:textAlignment="center"
        android:textColor="#CE1313"
        android:textSize="20sp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:layout_constraintVertical_bias="0.321" />

    <Button
        android:id="@+id/button2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:text="Start your Activity"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        tools:layout_editor_absoluteY="429dp" />

    <ImageView
        android:id="@+id/imageView2"
        android:layout_width="124dp"
        android:layout_height="80dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.498"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button2"
        app:layout_constraintVertical_bias="0.132"
        app:srcCompat="@android:drawable/ic_media_play" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

## OUTPUT

<img width="1873" height="1006" alt="Screenshot 2026-10-22 113618" src="https://github.com/user-attachments/assets/9d15fe22-9f85-41b3-ab0e-ee4e81e7a246" />

<img width="1917" height="1015" alt="Screenshot 2026-11-02 085103" src="https://github.com/user-attachments/assets/50082d88-c232-45ab-990f-b41314356675" />
<img width="1917" height="1020" alt="Screenshot 2026-11-02 084935" src="https://github.com/user-attachments/assets/0014f532-6870-494d-aad7-5c15724d758f" />

## RESULT
Thus a Simple Android Application create a HelloWorld Activity using all lifecycles methods to display messages using Android Studio is developed and executed successfully.


