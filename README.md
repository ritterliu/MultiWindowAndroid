MultiWindowAndroid
==================

A multi window system basing on android KitKat 4.4 .

1. multi_window_android_v0.1.patch:

A patch you should apply in the root of AOSP, which has a WindowApps to let you select which APP shows in windowing state.


2. stack_box.patch:

After applying the multi_window_android_v0.1.patch, you can apply the stack_box.patch in AOSP/framework/base/, which will make the windowing APPs show in StackBox. 
More info about StackBox: http://blog.csdn.net/ritterliu/article/details/37560239

Toggle between old multi window solution and StackBox solution:
If you select no APP in WindowApps, all APPs will show in windowing state in StackBox. But If you select one or more APPs in WindowApps, the selected APPs will run in old multi window solution. You can tell the differences by watching the initial window size: StackBox is 600*800, old multi window is 540*960.

Special thanks to Tieto, by studying their multi window code, I write this stack_box patch.
