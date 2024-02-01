# react-native-bluetooch-escpos-printer

See original at https://github.com/januslo/react-native-bluetooth-escpos-printer

# My update (fork from version 0.0.5)

> error: cannot find symbol import android.support.v4.app.ActivityCompat;

open `node_modules\react-native-bluetooth-escpos-printer\android\src\main\java\cn\jystudio\bluetooth\RNBluetoothManagerModule.java` and replace

    android.support.v4.app.ActivityCompat;
    android.support.v4.content.ContextCompat;

to

    import androidx.core.app.ActivityCompat;
    import androidx.core.content.ContextCompat;

visit [issues 188](https://github.com/januslo/react-native-bluetooth-escpos-printer/issues/188#issuecomment-1240682721)

> Could not resolve all dependencies for configuration ':react-native-bluetooth-escpos-printer:classpath

open `node_modules\react-native-bluetooth-escpos-printer\android\build.gradle` and replace as [Pull request](https://github.com/januslo/react-native-bluetooth-escpos-printer/blob/3ac15a7f9c44354b15395a2f4939c6c299425a15/android/build.gradle)

visit [issues 198](https://github.com/januslo/react-native-bluetooth-escpos-printer/issues/198)
