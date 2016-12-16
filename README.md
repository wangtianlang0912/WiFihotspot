# WiFihotspot
A demonstration of how to develop an example of WiFi.

该demo是基于https://github.com/AndroidKun/WiFihotspot 改造的，首先感谢AndroidKun提供的源码共享，我将其导入到了Android Studio中，主要修改了以下几个地方。

1. 增加    <uses-permission android:name="android.permission.WRITE_SETTINGS"/> 支持Android 6.0系统
2. 修改了 MainActiivity.java的216行 config.hiddenSSID = false; 让创建的AP能够别其他设备发现；

3. 修改了 MainActiivity.java的221行 因为WPA2_PSK被系统隐藏了，所以只能看到WPA_PSK，经查询WPA2_PSK = 4。修改可行；
 