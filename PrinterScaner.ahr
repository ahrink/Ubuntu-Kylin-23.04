Printer Driver install (as root, cd meaning: change directory)
example: mkdir /home/sananton/Printer 
note: # REM: sananton is a user name (case)
example: cd /home/sananton/Printer

# 1. apt-get install libgtk*

# 2. Download your Linux printer driver (case Canon)
note: [this is particular to printer or scanner as a device brand]

# 3. Download your Linux scanner driver (case Canon)
note: [this is particular to printer or scanner as a device brand]

# 4. once the downloaded package is in Printer-Directory
note: [extract the archive and cd to extracted archive]
example: cd /home/sananton/Printer/scangearmp2-4.30-1-deb/

# 5. execute install (scanner case)
example: ./install.sh
Screen outout example: Installation has been completed.

# 6. example
cd /home/sananton/Printer

note: download and extract archive in /home/sananton/Printer
note: [cd to where the extracted archive was executed]
example: cd /home/sananton/Printer/cnijfilter2-6.30-1-deb

# 7. the scanner driver only outputs on screen the result
# note: while the printer driver needs user input as follows:

#=========================================================#
#  Register Printer
#=========================================================#
Next, register the printer to the computer.
Connect the printer, and then turn on the power.
To use the printer on the network, connect the printer to the network.
When the printer is ready, press the Enter key.
> 

#=========================================================#
#  Connection Method
#=========================================================#
 1) USB
 2) Network
Select the connection method.[1]1

Searching for printers...


#=========================================================#
#  Select Printer
#=========================================================#
Select the printer.
If the printer you want to use is not listed, select Update [0] to search again.
To cancel the process, enter [Q].
-----------------------------------------------------------
 0) Update
-----------------------------------------------------------
Target printers detected
1) Canon TS3500 series (//Canon/?port=usb&serial=588C5D)
-----------------------------------------------------------
Currently selected:[1] Canon TS3500 series (//Canon/?port=usb&serial=588C5D)
Enter the value. [1]

#=========================================================#
#  Register Printer
#=========================================================#
Enter the printer name.[TS3500USB]
Command executed = sudo /usr/sbin/lpadmin -p TS3500USB -P /usr/share/cups/model/canonts3500.ppd -v cnijbe2://Canon/?port=usb&serial=588C5D -E
lpadmin: Printer drivers are deprecated and will stop working in a future version of CUPS.

#=========================================================#
#  Set as Default Printer
#=========================================================#
Do you want to set this printer as the default printer?
Enter [y] for Yes or [n] for No.[y]y

#=========================================================#
Installation has been completed.
Printer Name : TS3500USB
Select this printer name for printing.
#=========================================================#

