# serial/rs485 tools | linux

bootdisc of a barebones rs485/serial debugging system based on linux. Nothing other than what is needed, no X, no fluff, < 80 mb, just serial/rs485 communication tools that should run on any potato with a focus on serial and modbus communication.

## rs485/rs232 tools
```
minicom................serial client with special support for rs485 (Setup half-duplex rs485 adapter like the CC-USB-RS485-150U)
picocom................serial client for hexadecimal communication (RX/TX Hexadecimal messages)
mbpoll.................tool for constructing modbus messages for reading or writing
hexcurse...............large format hexadecimal editor (for a captured data steam)
hexdump................data convertion (hex2dec, dec2hex)
socat..................connect to virtual ports (usr-w610 RS485 to Wifi)
```
## other tools
```
tcpdump.................tcp capture utility used to decode/reverse-engineer the manufactures softwares functionality 
arping, arp-san, nmap...utilities needed for network device identification
nbtscan, smbclient......for find network shares (to save files remotely, since the bootdisk is likely read-only
mdns....................for listing all the mdns device found on the network without using avahi
nano....................text editor
bc......................calculator
```

## helpers
```
usr-w610.sh.............script to find and help connect to a usr-w610 device on a local network
parse-modbus-msg.sh.....script parses either tx or rx modbus comands for valilidity
```
