Settings -> Network -> Network Settings (button)
Select the Ethernet-item listed and click the setting button to edit.
...

Manually set network settings
https://help.ubuntu.com/stable/ubuntu-help/net-manual.html.en
...

Select the IPv4 only as a First Troubleshooting test:
- Add IP Address and Gateway, as well as the appropriate Netmask.
  [should correspond to LAN settings]

Skip DNS setting as it is set to auto. Save.

The above solved the problem noted in the README.MD with regards to Physical Network Interfaces (PNI) – OEM Install Ubuntu Kylin 23.04


…
20230805
Network troubleshooting where I reported a Kylin problem that is not actually the OS that causes such malfunction/error. 

The problem could be very well caused by “faulty wire” – that means the booting-device and OS is working but w/o replacing the “wire” we will never know. In this case the wire includes a dangle USB C network adapter. 

Particular such dangle is also overheating – had two one LG brand that is burned (not even recognized by OS) and a Gator brand that is overheating.
