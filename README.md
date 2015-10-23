# PlainDAC
Controlling PlainDAC+ and PlainDSP from userspace.

#INSTALLATION
git clone https://github.com/PolyVection/PlainDAC.git

cd PlainDAC

*only for Banana Pi users*: 
edit plaindac.c and replace “/dev/i2c-1” with “/dev/i2c-2”

gcc -o plaindac plaindac.c

#USAGE
./plaindac -u = startup command:    

./plaindac -p = mute command:       

./plaindac -m = volume + 0.5dB:     

./plaindac -l = volume - 0.5dB:     

./plaindac -d = status/debug:       

./plaindac -v 01 (where 01 is the volume in percent from 0 to 124) 
