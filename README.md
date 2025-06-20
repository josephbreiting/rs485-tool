# serial/rs485 tools | linux

bootdisc of my barebones rs485/serial debugging system based on linux. Nothing other than what is needed, no X, no fluff just serial/rs485 communication tools that should run on any potato.

## rs485/rs232 tools
minicom................serial client with special support for rs485 (Setup half-duplex rs485 adapter like the CC-USB-RS485-150U)
picocom................serial client for hexadecimal communication (RX/TX Hexadecimal messages)
mbpoll.................tool for constructing modbus messages for reading or writing
hexcurse...............large format hexadecimal editor (for a captured data steam)
xxd....................data convertion (hex2dec, dec2hex)
socat..................connect to virtual ports (usr-w610 RS485 to Wifi)

## other tools
tcpdump.................tcp capture utility used to decode/reverse-engineer the manufactures softwares functionality (finding how the software finds the rs485 to wifi converter) 
arping, arp-san, nmap...utilities needed for network device identification (reproduces the functions need to find the rs485 to wifi converter on the network)
nbtscan, smbclient......for find network shares (to save files remotely, since the bootdisk is likely read-only
mdns....................for listing all the mdns device found on the network without using avahi
nano....................text editor
bc......................calculator

# helpers
usr-w610.sh.............script to find and help connect to a usr-w610 device on a local network
parse-modbus-msg.sh.....script parses either tx or rx modbus comands for valilidity
modbus-scan.sh..........script to scan for either serial setup parameters and modbus device details 
