#SPDX-License-Identifier: GPL-3.0-only
#
#     Copyright (C) 2020  Haruki Shimotori and Ryuichi Ueda. All right reserved.
#

obj-m := myled.o
FLAGS_myled.o := -O0 

myled.ko: myled.c
	make -C /usr/src/linux-headers-`uname -r` M=`pwd` V=1 modules

clean:
	make -C /usr/src/linux-headers-`uname -r` M=`pwd` V=1 clean
