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
