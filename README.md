# openwrt_tmp
# Thanks to Ronaldo Nunez and OpenWRT community for supporting
# https://www.youtube.com/watch?v=iJqMEjVXKZU&ab_channel=EmbeddedMeetup

Install dependency packages if compilation fails, example: gawk, python2 etc. 

openwrt compilation process as below step by step,

$git clone https://github.com/openwrt/openwrt.git -b openwrt-19.07
$cd openwrt/
$scripts/feeds update
$sudo scripts/feeds install -a
$sudo make menuconfig
$sudo make download
$sudo su
$export FORCE_UNSAFE_CONFIGURE=1
$make -j16 V=s

