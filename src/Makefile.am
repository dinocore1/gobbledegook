# Build a static library (libggk.a)
lib_LIBRARIES = libggk.a
libggk_a_CXXFLAGS = $(GLIB_CFLAGS) $(GIO_CFLAGS) $(GOBJECT_CFLAGS)
libggk_a_SOURCES = DBusInterface.cpp \
                   DBusInterface.h \
                   DBusMethod.cpp \
                   DBusMethod.h \
                   DBusObject.cpp \
                   DBusObject.h \
                   DBusObjectPath.h \
                   GattCharacteristic.cpp \
                   GattCharacteristic.h \
                   GattDescriptor.cpp \
                   GattDescriptor.h \
                   GattInterface.cpp \
                   GattInterface.h \
                   GattProperty.cpp \
                   GattProperty.h \
                   GattService.cpp \
                   GattService.h \
                   GattUuid.h \
                   Globals.h \
                   Gobbledegook.cpp \
                   HciAdapter.cpp \
                   HciAdapter.h \
                   HciSocket.cpp \
                   HciSocket.h \
                   Init.cpp \
                   Init.h \
                   Logger.cpp \
                   Logger.h \
                   Mgmt.cpp \
                   Mgmt.h \
                   Server.cpp \
                   Server.h \
                   ServerUtils.cpp \
                   ServerUtils.h \
                   standalone.cpp \
                   TickEvent.h \
                   Utils.cpp \
                   Utils.h

include_HEADERS = ../include/Gobbledegook.h

# Build our standalone server (linking statically with libggk.a, linking dynamically with GLib)
standalone_CXXFLAGS =
noinst_PROGRAMS = standalone
standalone_SOURCES = standalone.cpp
standalone_LDADD = libggk.a
standalone_LDLIBS = $(GLIB_LIBS) $(GIO_LIBS) $(GOBJECT_LIBS)
