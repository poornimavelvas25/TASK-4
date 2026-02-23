# STEPS
1.Used kali linux as target
2.Used Windows instead of another machine.
3.telnet

## STEP 1:-Open Terminal in Kali
## STEP 2:-Check if ufw is installed
         sudo ufw status
If not,
        sudo apt update
        sudo apt install ufw -y
## STEP 3:-Enable 
        sudo ufw enable
## STEP 4:-List Current Firewall Rules
        sudo ufw status numbered
## STEP 5:-Block Inbound Traffic on Port 23 (Telnet)
        sudo ufw deny 23/tcp
## STEP 6:-Allow SSH (Port 22)
        sudo ufw allow 22/tcp
## STEP 7:-Test in Windows
        telnet 192.168.56.101 23
If telnet not installed,
     Open cmd and run as adminstrator,
     dism /online /Enable-Feature /FeatureName:TelnetClient
## STEP 8:-Test SSH (Port 22)
        ssh kali@192.168.56.101(UR KAIL USERNAME AND IP)
## STEP 9:-RESULTS
If allowed → it connects.

If blocked → firewall issue.


## NOTE:-
If ssh didnot connect go to kali and enable ssh.
