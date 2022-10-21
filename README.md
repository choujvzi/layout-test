# layout-test
## 表格布局实现以下界面：
![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E8%A1%A8%E6%A0%BC%E5%B8%83%E5%B1%80%E5%9B%BE1.png)

![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E8%A1%A8%E6%A0%BC%E5%B8%83%E5%B1%80%E5%9B%BE2.png)

### 表格布局部分重要代码如下：
```java
<?xml version="1.0" encoding="utf-8"?>
<TableLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <TableRow
        android:layout_width="419dp"
        android:layout_height="30dp" >
        <TextView
            android:id="@+id/textView"
            android:layout_width="412dp"
            android:layout_height="30dp"
            android:background="#545454"
            android:gravity="center_vertical|start"
            android:text="Hello TableLayout"
            android:textColor="@color/white" />
    </TableRow>
</TableLayout>
```

## 线性布局实现以下界面：
![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E7%BA%BF%E6%80%A7%E5%B8%83%E5%B1%80%E5%9B%BE1.png)

![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E7%BA%BF%E6%80%A7%E5%B8%83%E5%B1%80%E5%9B%BE2.png)

### 线性布局部分重要代码如下：
```java
<?xml version="1.0" encoding="utf-8"?>
<LinearLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity"
    android:orientation="vertical">
    <LinearLayout
        android:layout_width="match_parent"
        android:layout_height="40dp"
        android:orientation="horizontal"
        >
        <TextView
            android:layout_width="0dp"
            android:layout_height="40dp"
            android:layout_weight="1"
            android:text="One,One"
            android:background="@color/black"
            android:textColor="@color/white"
            android:textSize="12sp"
            android:gravity="center"
            />
        <TextView
            android:layout_width="0dp"
            android:layout_height="40dp"
            android:layout_weight="1.4"
            android:layout_marginStart="3dp"
            android:text="One,Two"
            android:background="@color/black"
            android:textColor="@color/white"
            android:textSize="12sp"
            android:gravity="center"/>
        <TextView
            android:layout_width="0dp"
            android:layout_height="40dp"
            android:layout_marginStart="3dp"
            android:layout_weight="1"
            android:text="One,Three"
            android:background="@color/black"
            android:textColor="@color/white"
            android:textSize="12sp"
            android:gravity="center"/>
        <TextView
            android:layout_width="0dp"
            android:layout_height="40dp"
            android:layout_weight="1"
            android:layout_marginStart="3dp"
            android:text="One,Four"
            android:background="@color/black"
            android:textColor="@color/white"
            android:textSize="12sp"
            android:gravity="center"/>
    </LinearLayout>
</LinearLayout>
```

## 约束布局1实现以下界面：
![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E7%BA%A6%E6%9D%9F%E5%B8%83%E5%B1%801%E5%9B%BE1.png)

![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E7%BA%A6%E6%9D%9F%E5%B8%83%E5%B1%801%E5%9B%BE2.png)

### 约束布局1部分重要代码如下：
```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <TextView
        android:id="@+id/textView14"
        android:layout_width="412dp"
        android:layout_height="21dp"
        android:text="ConStrainLayout"
        android:background="#32CD32"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent" />
    <TextView
        android:id="@+id/textView15"
        android:layout_width="411dp"
        android:layout_height="62dp"
        android:text="Input"
        android:textSize="40sp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView14" />
    <TextView
        android:id="@+id/textView16"
        android:layout_width="363dp"
        android:layout_height="31dp"
        android:layout_marginTop="24dp"
        android:background="#B5A642"
        android:gravity="center_vertical|end"
        android:text="0.0"
        android:textSize="30sp"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView15" />
    <Button
        android:id="@+id/button"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="16dp"
        android:text="7"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/textView16"
        app:layout_constraintVertical_bias="0.064" />
    <Button
        android:id="@+id/button2"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="8"
        app:layout_constraintStart_toEndOf="@+id/button"
        app:layout_constraintTop_toBottomOf="@+id/textView16" />
    <Button
        android:id="@+id/button3"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="9"
        app:layout_constraintStart_toEndOf="@+id/button2"
        app:layout_constraintTop_toBottomOf="@+id/textView16" />
    <Button
        android:id="@+id/button4"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="/"
        app:layout_constraintStart_toEndOf="@+id/button3"
        app:layout_constraintTop_toBottomOf="@+id/textView16" />
    <Button
        android:id="@+id/button6"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="16dp"
        android:layout_marginTop="35dp"
        android:text="4"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button" />
    <Button
        android:id="@+id/button7"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="5"
        app:layout_constraintStart_toEndOf="@+id/button6"
        app:layout_constraintTop_toBottomOf="@+id/button2" />
    <Button
        android:id="@+id/button8"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="6"
        app:layout_constraintStart_toEndOf="@+id/button7"
        app:layout_constraintTop_toBottomOf="@+id/button3" />
    <Button
        android:id="@+id/button9"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="x"
        app:layout_constraintStart_toEndOf="@+id/button8"
        app:layout_constraintTop_toBottomOf="@+id/button4" />
    <Button
        android:id="@+id/button10"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="16dp"
        android:layout_marginTop="35dp"
        android:text="1"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button6" />
    <Button
        android:id="@+id/button11"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="2"
        app:layout_constraintStart_toEndOf="@+id/button10"
        app:layout_constraintTop_toBottomOf="@+id/button7" />
    <Button
        android:id="@+id/button12"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="3"
        app:layout_constraintStart_toEndOf="@+id/button11"
        app:layout_constraintTop_toBottomOf="@+id/button8" />
    <Button
        android:id="@+id/button13"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="+"
        app:layout_constraintStart_toEndOf="@+id/button12"
        app:layout_constraintTop_toBottomOf="@+id/button9" />
    <Button
        android:id="@+id/button14"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="16dp"
        android:layout_marginTop="35dp"
        android:text="."
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toBottomOf="@+id/button10" />
    <Button
        android:id="@+id/button15"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="0"
        app:layout_constraintStart_toEndOf="@+id/button14"
        app:layout_constraintTop_toBottomOf="@+id/button11" />
    <Button
        android:id="@+id/button16"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="="
        app:layout_constraintStart_toEndOf="@+id/button15"
        app:layout_constraintTop_toBottomOf="@+id/button12" />
    <Button
        android:id="@+id/button17"
        android:layout_width="65dp"
        android:layout_height="50dp"
        android:layout_marginStart="35dp"
        android:layout_marginTop="35dp"
        android:text="-"
        app:layout_constraintStart_toEndOf="@+id/button16"
        app:layout_constraintTop_toBottomOf="@+id/button13" />
</androidx.constraintlayout.widget.ConstraintLayout>
```

## 约束布局2实现以下界面：
![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E7%BA%A6%E6%9D%9F%E5%B8%83%E5%B1%802%E5%9B%BE1.png)

![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E7%BA%A6%E6%9D%9F%E5%B8%83%E5%B1%802%E5%9B%BE2.png)

### 约束布局2部分重要代码如下：
```java
<?xml version="1.0" encoding="utf-8"?>
<androidx.constraintlayout.widget.ConstraintLayout xmlns:android="http://schemas.android.com/apk/res/android"
    xmlns:app="http://schemas.android.com/apk/res-auto"
    xmlns:tools="http://schemas.android.com/tools"
    android:layout_width="match_parent"
    android:layout_height="match_parent"
    tools:context=".MainActivity">
    <ImageView
        android:id="@+id/imageView"
        android:layout_width="30dp"
        android:layout_height="30dp"
        android:layout_marginTop="15dp"
        app:layout_constraintEnd_toStartOf="@+id/imageView2"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="parent"
        app:srcCompat="@drawable/space_station_icon" />
    <ImageView
        android:id="@+id/imageView2"
        android:layout_width="30dp"
        android:layout_height="30dp"
        app:layout_constraintBottom_toBottomOf="@+id/imageView"
        app:layout_constraintEnd_toStartOf="@+id/imageView3"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/imageView"
        app:layout_constraintTop_toTopOf="@+id/imageView"
        app:srcCompat="@drawable/rocket_icon" />
    <ImageView
        android:id="@+id/imageView3"
        android:layout_width="30dp"
        android:layout_height="30dp"
        app:layout_constraintBottom_toBottomOf="@+id/imageView2"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toEndOf="@+id/imageView2"
        app:layout_constraintTop_toTopOf="@+id/imageView2"
        app:srcCompat="@drawable/rover_icon" />
    <TextView
        android:id="@+id/textView18"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="15dp"
        android:text="Space Stations"
        app:layout_constraintEnd_toEndOf="@+id/imageView"
        app:layout_constraintHorizontal_bias="0.607"
        app:layout_constraintStart_toStartOf="@+id/imageView"
        app:layout_constraintTop_toBottomOf="@+id/imageView" />
    <TextView
        android:id="@+id/textView19"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="15dp"
        android:text="Flights"
        app:layout_constraintEnd_toEndOf="@+id/imageView2"
        app:layout_constraintStart_toStartOf="@+id/imageView2"
        app:layout_constraintTop_toBottomOf="@+id/imageView2" />
    <TextView
        android:id="@+id/textView20"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:layout_marginTop="15dp"
        android:text="Rovers"
        app:layout_constraintEnd_toEndOf="@+id/imageView3"
        app:layout_constraintStart_toStartOf="@+id/imageView3"
        app:layout_constraintTop_toBottomOf="@+id/imageView3" />
    <TextView
        android:id="@+id/textView21"
        android:layout_width="124dp"
        android:layout_height="98dp"
        android:layout_marginEnd="40dp"
        android:background="#339900"
        android:gravity="center"
        android:text="DCA"
        app:layout_constraintBottom_toBottomOf="@+id/imageView4"
        app:layout_constraintEnd_toEndOf="@+id/imageView4"
        app:layout_constraintTop_toTopOf="@+id/imageView4" />
    <TextView
        android:id="@+id/textView22"
        android:layout_width="124dp"
        android:layout_height="98dp"
        android:layout_marginStart="40dp"
        android:background="#339900"
        android:gravity="center"
        android:text="MARS"
        app:layout_constraintBottom_toBottomOf="@+id/imageView4"
        app:layout_constraintStart_toStartOf="@+id/imageView4"
        app:layout_constraintTop_toTopOf="@+id/imageView4" />
  <ImageView
        android:id="@+id/imageView4"
        android:layout_width="60dp"
        android:layout_height="60dp"
        android:layout_marginBottom="36dp"
        app:layout_constraintBottom_toTopOf="@+id/guideline2"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.498"
        app:layout_constraintStart_toStartOf="parent"
        app:srcCompat="@drawable/double_arrows" />
    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline2"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="horizontal"
        app:layout_constraintGuide_begin="200dp" />
    <androidx.constraintlayout.widget.Guideline
        android:id="@+id/guideline3"
        android:layout_width="wrap_content"
        android:layout_height="wrap_content"
        android:orientation="vertical"
        app:layout_constraintGuide_percent="0.05" />
    <Switch
        android:id="@+id/switch1"
        android:layout_width="160dp"
        android:layout_height="wrap_content"
        android:layout_marginStart="8dp"
        android:layout_marginTop="200dp"
        android:background="#FF7F00"
        android:minHeight="48dp"
        android:text="One Way"
        app:layout_constraintStart_toStartOf="@+id/guideline3"
        app:layout_constraintTop_toTopOf="parent" />
    <TextView
        android:id="@+id/textView23"
        android:layout_width="wrap_content"
        android:layout_height="45dp"
        android:layout_marginStart="8dp"
        android:layout_marginTop="8dp"
        android:background="#FF7F00"
        android:gravity="center_vertical|start"
        android:text="1 Traveller"
        app:layout_constraintStart_toStartOf="@+id/guideline3"
        app:layout_constraintTop_toBottomOf="@+id/switch1" />
    <ImageView
        android:id="@+id/imageView5"
        android:layout_width="90dp"
        android:layout_height="90dp"
        app:layout_constraintBottom_toBottomOf="parent"
        app:layout_constraintEnd_toEndOf="parent"
        app:layout_constraintHorizontal_bias="0.5"
        app:layout_constraintStart_toStartOf="parent"
        app:layout_constraintTop_toTopOf="@+id/guideline2"
        app:srcCompat="@drawable/galaxy" />
           <ImageView
        android:id="@+id/imageView6"
        android:layout_width="30dp"
        android:layout_height="30dp"
        app:layout_constraintBottom_toBottomOf="@+id/imageView5"
        app:layout_constraintEnd_toStartOf="@+id/imageView5"
        app:layout_constraintTop_toTopOf="@+id/imageView5"
        app:srcCompat="@drawable/rocket_icon" />
    <Button
        android:id="@+id/button5"
        android:layout_width="match_parent"
        android:layout_height="wrap_content"
        android:text="DEPART"
        app:layout_constraintBottom_toBottomOf="parent"
        tools:layout_editor_absoluteX="65dp" />
</androidx.constraintlayout.widget.ConstraintLayout>
```
