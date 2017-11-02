all:
	verilator -O3 --x-assign fast --noassert -Wall -Wno-DECLFILENAME --cc harris.v --exe sim_DesignTop_main.cpp --top-module DesignTop
	make OPT_FAST="-O3" -C obj_dir -j -f VDesignTop.mk VDesignTop
	./obj_dir/VDesignTop
