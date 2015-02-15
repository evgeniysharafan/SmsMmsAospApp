# SmsMmsAospApp

It is the lollipop version of [AOSP Messaging app](https://android.googlesource.com/platform/packages/apps/Mms) which compiles without depending on internal Android classes and other libs which are listed in the [Android.mk](https://android.googlesource.com/platform/packages/apps/Mms/+/master/Android.mk) file.

Now it works without crashes only on lollipop because of using some new APIs, but it will be changed soon. I plan downgrade the minimum version to 15.

It doesn't contain the SoundRecorder module now, it will be changed soon.

-
This code will be useful if you write a sms/mms app. You will be surprized how difficult to create a mms app on Android. All such apps get inspire from AOSP Mms app and use internal com.google.android.mms.pdu package. Here you will find a working example of such app.

-
These links can be useful for you:

* [Mms app AOSP](https://android.googlesource.com/platform/packages/apps/Mms) sources.

* [New Mms service for lollipop](https://android.googlesource.com/platform/packages/services/Mms) and a lot of mms configs for countries in the res folder.

* [Chips](https://android.googlesource.com/platform/frameworks/opt/chips) library.
You can take a look at [this example](https://s-media-cache-ak0.pinimg.com/736x/19/e9/5a/19e95a6606b9fbc6251860831468f5cd.jpg) if you don't know what it is.

* A [library](https://github.com/klinker41/android-smsmms) for sending Sms and Mms messges, based on this AOSP code. Also it includes lollipop Mms service and Mms configs [from platform/packages/services/Mms](https://android.googlesource.com/platform/packages/services/Mms).
But this library doesn't contain code for receiving messages.
