LOCAL_PATH:= $(call my-dir)
include $(CLEAR_VARS)

LOCAL_SRC_FILES:= \
	fbvncserver.c \
	LibVNCServer-0.9.7/libvncserver/main.c \
	LibVNCServer-0.9.7/libvncserver/rfbserver.c \
	LibVNCServer-0.9.7/libvncserver/rfbregion.c \
	LibVNCServer-0.9.7/libvncserver/auth.c \
	LibVNCServer-0.9.7/libvncserver/sockets.c \
	LibVNCServer-0.9.7/libvncserver/stats.c \
	LibVNCServer-0.9.7/libvncserver/corre.c \
	LibVNCServer-0.9.7/libvncserver/hextile.c \
	LibVNCServer-0.9.7/libvncserver/rre.c \
	LibVNCServer-0.9.7/libvncserver/translate.c \
	LibVNCServer-0.9.7/libvncserver/cutpaste.c \
	LibVNCServer-0.9.7/libvncserver/httpd.c \
	LibVNCServer-0.9.7/libvncserver/cursor.c \
	LibVNCServer-0.9.7/libvncserver/font.c \
	LibVNCServer-0.9.7/libvncserver/draw.c \
	LibVNCServer-0.9.7/libvncserver/selbox.c \
	LibVNCServer-0.9.7/libvncserver/d3des.c \
	LibVNCServer-0.9.7/libvncserver/vncauth.c \
	LibVNCServer-0.9.7/libvncserver/cargs.c \
	LibVNCServer-0.9.7/libvncserver/minilzo.c \
	LibVNCServer-0.9.7/libvncserver/ultra.c \
	LibVNCServer-0.9.7/libvncserver/scale.c \
	LibVNCServer-0.9.7/libvncserver/zlib.c \
	LibVNCServer-0.9.7/libvncserver/zrle.c \
	LibVNCServer-0.9.7/libvncserver/zrleoutstream.c \
	LibVNCServer-0.9.7/libvncserver/zrlepalettehelper.c \
	LibVNCServer-0.9.7/libvncserver/zywrletemplate.c \
	LibVNCServer-0.9.7/libvncserver/tight.c

LOCAL_C_INCLUDES := \
	$(LOCAL_PATH) \
	$(LOCAL_PATH)/LibVNCServer-0.9.7/libvncserver \
	$(LOCAL_PATH)/LibVNCServer-0.9.7 \
	external/zlib \
	external/jpeg

LOCAL_SHARED_LIBRARIES := libz
LOCAL_STATIC_LIBRARIES := libjpeg

LOCAL_MODULE:= androidvncserver

include $(BUILD_EXECUTABLE)
