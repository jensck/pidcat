PID Cat
=======

An update to Jake Wharton's PID-filtering logcat script, which is based off
Jeff Sharkey's excellent [logcat color script][1], with two changes:
1. No color-coding (friendly for redirecting to files and viewing in a plan text editor) and
2. Add timestamps

During application development you often want to only display log messages
coming from your app. Unfortunately, because the process ID changes every time
you deploy to the phone it becomes a challenge to grep for the right thing.

This script solves that problem by filtering by application package. Supply the
target package as the sole argument to the python script and enjoy a more
convenient development process.

    ./pidcat.py com.oprah.bees.android

 [1]: http://jsharkey.org/blog/2009/04/22/modifying-the-android-logcat-stream-for-full-color-debugging/
