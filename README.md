
# Rapport

I filen "activity_main.xml" i design fliken används en constraintLayout och sedan lades olika wigetar till i layouten.

Det som lades till var "EditText" , "ImageView" samt "Button". Sedan constraintade olika widgetar och med hjälp av margin för att placera de widgetarna på skärmen snyggt. 

Två ImageView lades till som kallar på bilderna "pic1" och "pic2".  

koden av detta kan man se i kod fliken och det blev som följande: 

```
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">

    <TextView
        android:id="@+id/titleTv"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="32dp"
        android:text="Hello World!"
        app:layout_constraintLeft_toLeftOf="parent"
        app:layout_constraintRight_toRightOf="parent"
        app:layout_constraintTop_toTopOf="parent" />

    <Button
        android:id="@+id/submitButton"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginBottom="360dp"
        android:text="Button"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="@+id/inputEt"
        app:layout_constraintHorizontal_bias="0.508"
        app:layout_constraintStart_toStartOf="@+id/inputEt" />

    <EditText
        android:id="@+id/inputEt"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="24dp"
        android:layout_marginBottom="32dp"
        android:ems="10"
        android:gravity="center"
        android:hint="@string/name_helper"
        android:inputType="text"
        app:layout_constraintBottom_toTopOf="@+id/submitButton"
        app:layout_constraintEnd_toEndOf="@+id/imageView3"
        app:layout_constraintStart_toStartOf="@+id/imageView2"
        app:layout_constraintTop_toBottomOf="@+id/imageView3"
        android:autofillHints="" />

    <ImageView
        android:id="@+id/imageView2"
        android:layout_width="150dp"
        android:layout_height="140dp"
        android:layout_marginTop="32dp"
        android:contentDescription="@string/placeholder_1"
        app:layout_constraintEnd_toStartOf="@+id/imageView3"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/titleTv"
        android:src="@drawable/pic1" />

    <ImageView
        android:id="@+id/imageView3"
        android:layout_width="150dp"
        android:layout_height="140dp"
        android:layout_marginTop="32dp"
        android:contentDescription="@string/placeholder_2"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/imageView2"
        app:layout_constraintTop_toBottomOf="@+id/titleTv"
        android:src="@drawable/pic2" />

</androidx.constraintlayout.widget.ConstraintLayout>
```

Skärmbild av appen: 
![](screenshot.png)

