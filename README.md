DallasTemperature_SparkCore
===========================

Quick port of exiting DallasTemperature and Onewire libraries to Spark Core platform

Put DallasTemperature.h, OneWire.h in the inc directroy under core-firmware

Put DallasTemperature.cpp, OneWire.cpp and example application application.cpp in the scr directory under core-firmware

add 
```
>CPPSRC += $(TARGET_SRC_PATH)/DallasTemperature.cpp
>CPPSRC += $(TARGET_SRC_PATH)/OneWire.cpp
```
to your build.mk file the scr directory under core-firmware

make and enjoy.



DallasTemperature Libary from 
http://milesburton.com/Dallas_Temperature_Control_Library
OneWire Libary from.
http://www.pjrc.com/teensy/td_libs_OneWire.html

SparkCore Verison of OneWire Libary 

I've taken the code that Spark Forum user tidwelltimj posted 
split it back into separte code and header files and put back in the 
credits and comments and got it compiling on the command line within SparkCore core-firmware
