# layout-test
## 表格布局实现以下界面：
![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E8%A1%A8%E6%A0%BC%E5%B8%83%E5%B1%80%E5%9B%BE1.png)

![image](https://github.com/choujvzi/layout-test/blob/master/screenshots/%E8%A1%A8%E6%A0%BC%E5%B8%83%E5%B1%80%E5%9B%BE2.png)
### 表格布局部分重要代码如下：
'''<?xml version="1.0" encoding="utf-8"?>
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
