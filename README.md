check_bw
========

Bandwidth check for use with nagios or similar


Usage:

./check_bw (-t|-p) -i (interface) -w (in,out) -c (in,out)

-t: transfer mode, measure in Mbit/s

-p: packets mode, measure in packages/s

-i: interface name

-w: warning level written as in,out - only integers

-c: critical level written as in,out - only integers


Sample:

./check_bw -t -i eth0 -w 8,4 -c 10,5

output: BANDWIDTH OK - rx 1.20 Mbit/s tx 1.86 Mbit/s
