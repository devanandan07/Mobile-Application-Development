# Ex.No: 2 To develop an application that uses GUI Components with Fonts and Colors. 
Note: Create button for colors and fonts while clicking color or font button should change 


## AIM:

To create an application that uses GUI Components with Fonts and Colors using Android Studio.

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
Program to develop an application that uses GUI Components with Fonts and Colors.
Developed by: Devanandan K
Registeration Number :212221040036
```
MainActivity.java

**XML FILE:**
```xml
    
    <?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:id="@+id/bg"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    android:background="#D1B6B6"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/tv1"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="108dp"
        android:text="Color Change on button click"
        android:textColor="#FF1010"
        android:textSize="24sp"
        android:textStyle="bold"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.494"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/bt1"
        android:layout_width="158dp"
        android:layout_height="59dp"
        android:layout_marginStart="128dp"
        android:layout_marginTop="332dp"
        android:text="Color Changer"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
</androidx.constraintlayout.widget.ConstraintLayout>
```        
**MAINACTIVITY:**
```java    
    package com.example.exercise2;

import androidx.appcompat.app.AppCompatActivity;
import androidx.constraintlayout.widget.ConstraintLayout;

import android.graphics.Color;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;
import android.widget.TextView;
import android.widget.Toast;

public class MainActivity extends AppCompatActivity {

    Button Color_Changer;
    ConstraintLayout bg2;
    TextView tv1;
    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);

        Color_Changer = findViewById(R.id.bt1);
        bg2 = findViewById(R.id.bg);
        tv1= findViewById(R.id.tv1);

        Color_Changer.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View view) {
                Toast.makeText(MainActivity.this, "button worked", Toast.LENGTH_SHORT).show();

                bg2.setBackgroundColor(Color.BLACK);
                tv1.setTextColor(Color.MAGENTA);
                tv1.setText("color changed");

                tv1.setTextSize(30);
            }
        });


    }
}
```
## OUTPUT
 ![Screenshot (7)](https://github.com/devanandan07/Mobile-Application-Development/assets/145025017/30d045c5-1654-42d6-9987-bffe5892ed2e)
 ![Screenshot (8)](https://github.com/devanandan07/Mobile-Application-Development/assets/145025017/e2cd80f0-ad1d-4c7b-aae2-d1690371828b)






## RESULT
Thus a Simple Android Application that uses GUI Components with Fonts and Colors using Android Studio is developed and executed successfully.
