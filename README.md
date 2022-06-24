# Workshop-1
To Create a simple menu option in android refer sample output and design same design.
Procedure:

Step-1: Create an android application using MainActivity.java using package from com.example.w2 with an empty activity.

Step-2: Modify MainActivity.java to display the contents of an application. 

Step-3: Modify activity_main.xml to create a layout for the application.

Step-4: Launch an emulator and run the code.

Program:
## Activity_Main.xml
```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout 
xmlns:android="http://schemas.android.com/apk/res/android"
xmlns:app="http://schemas.android.com/apk/res-auto" 
xmlns:tools="http://schemas.android.com/tools" 
android:layout_width="match_parent" 
android:layout_height="match_parent" 
tools:context=".MainActivity">
</androidx.constraintlayout.widget.ConstraintLayout>
```
## MainActivity.java
```
package com.example.optionmenu;
import androidx.appcompat.app.AppCompatActivity; import androidx.appcompat.view.menu.MenuBuilder;
import android.annotation.SuppressLint; import android.os.Bundle;
import  android.view.Menu; import android.view.MenuInflater;
public class MainActivity extends AppCompatActivity {
@Override
protected void onCreate(Bundle savedInstanceState) { super.onCreate(savedInstanceState); setContentView(R.layout.activity_main);
}
@SuppressLint("RestrictedApi") @Override
public boolean onCreateOptionsMenu(Menu menu) { MenuInflater menuInflater = getMenuInflater(); menuInflater.inflate(R.menu.activity_menu, menu);
return true;
}
}
```
## Activity_menu.xml
```
<?xml version="1.0" encoding="utf-8"?>
<menu xmlns:android="http://schemas.android.com/apk/res/android">
<item android:title="Menu Item 1" />
<item android:title="Menu Item 2" >
<menu >
<item android:title="Menu Item 2.1" />
<item android:title="Menu Item 2.2" />
</menu>
</item>
<item android:title="Menu Item 3" />
</menu>
```
## Output



