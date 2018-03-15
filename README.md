# RedTeam
                                                            Nmap
=========================================================================

nmap -sS -sV -A -O --script="*-vuln-*" --script-args=unsafe=1 <[IP]>

nmap -sC -sV -A -p- --open -v -T5 --script vuln 

nmap -sn -n --disable-arp-ping --max-retries=1 -vvv ipRange

nmap -sC -sV -A -p- --open -v -T5 --script vuln 192.168.1.210

nmap -T4 -A -sV --script=vuln -Pn

nmap -sV --script=default --script=vulscan/vulscan.nse IP

nmap -Pn -sV -oX a.xml site.com; searchsploit --nmap a.xml



                                                        Nikto

nikto -h http://yourdomain.com -C all

nikto -Tuning x 6 -h http://targetsite.com



