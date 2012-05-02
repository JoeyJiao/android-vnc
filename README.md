android-vnc
===========

My C8600 screen broken at least some mbn partition broken due to flash wrong C8500S updata.app. So android-vnc is the tool I can see screen and to operate from PC.
But seeing screen function works while operate not.

Based on http://code.google.com/p/android-vnc-server
and 	https://github.com/eachscape/tryout-androidvncserver

Procedures:
1. Compile or use executable androidvncserver and put under /system/bin/
2. adb shell androidvncserver -k /dev/input/event2 -t /dev/input/event0
3. Install any VNC viewer like Remmina on Ubuntu
4. adb forward tcp:5901 tcp:5901, then vnc to 127.0.0.1:5901
5. optional to step 4, using wifi, like 192.168.1.104:5901
6. optional to step 4, using usb0, like 192.168.1.105:5901
7. If want quit, adb shell ps|grep androidvncserver and then kill pid

Build Note:
1. Not capable with distcc so 'unset CCACHE_PREFIX' and then make androidvncserver under android src enviroment
