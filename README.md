# cf

pract 1} Creating a Forensic Image using FTK Image/Encase Image 
i)open ftk imager and go to file then create disk image
ii)select content of folder browse an file then give evidence item info and next 
iii)give destination folder and name also -->finish
iv) then in create image--click on start--> we get op
v) then again go to file --> add evidence item --image file --
browse ad1 file from destination folder-->finish
vi) click on evidence tree and checkout file (inside details)

pract 2} Data Acquisition - Perform data acquisition using:
 USB Write Blocker + FTK Imager.    
i) connect pd then open cmd and write commands 
diskpart , listdisk, select disk 1 , attributes disk set readonly
,attributes disk , attributes disk clear readonly, attributes disk
ii) open fkt imager and go to file-->create disk image-->select physical drive
iii)then browse--  finish --> click on add button and add destination folder
-->image type SMART and next then give evidence information-->next
iv) browse  destination folder  and give filename --> finish
v) click on start (it will take time) then u get op

 
pract3}  Forensics Case Study: -Solve the Case study (image file) provided
 in lab using Encase Investigator or Autopsy. 
i) cfreds.nist.gov then download rhinousb zip file
i)open auotspy --> fill case info then option info selct disk image (type of data source type)
ii) and select data source rhinousb.dd and browse this file --> next then
iii)in configure invest click on next --> finish
iv) search keyword and then generate report(html report)-- next--all result--finish
v) go to wireshark  open file--> select  rhino(text file)
then in searchbar-- search ftp , ftp-data, http.

pract4}  Capturing and analyzing network packets using Wireshark (Fundamentals): 
Identification the live network, Capture Packets,Analyze the captured packets
i)open wireshark -->click on snoops -- insearch bar
ip.addr==192.168.1.71, ip.src==192.168.1.71 , ip.dst==40.100.138.2 ,
http, http.request, http.response.code==200 , tcp.port==80 || udp.port==80
tcp contains facebook ,icmp , udp,ftp

pract 5} aim:- Analyse the packets provided in lab and solve the questions using Wireshark: 
What web server software is used by www.snopes.com?
About what cell phone problem is the client concerned? 
According to Zillow, what instrument will Ryan learn to play? 
How many web servers are running Apache? 
What hosts (IP addresses) think that jokes are more entertaining when they are explained? 

steps:-i)wireshark--search http --> right click on hypertext transfer protocol
-- the we get snopes.com in green color -- right click on that-- 
select follow-- tcp stream
ii) frame matches "(?i)cell"
iii)frame matches "(?i)zillow" 
then go to file --> export object-- http and save all
iv)http.response right click -- apply as column 
go to statistics-- endpoints--op
v) frame contains "joke"

pract6} aim:Using Sysinternals tools for Network Tracking and Process Monitoring: 
i)Check Sysinternals tools 
ii)Monitor Live Processes 
iii)Capture RAM 
iv)Capture TCP/UDP packets
v)Monitor Hard Disk
vi) Monitor Virtual Memory
vii)Monitor Cache Memory

stpes:i)sysinternals tools extract file and check the tools
ii) MLP -->procmon.exe open app then filter --filter-->select 1st and ok
then right click --> properties then get op
iii)rammap.exe open this app (khatam)
iv) tcpview.exe open and save menu item
v)diskmon.exe just open this
vi) vmmap.exe  open this also
vii)cacheset.exe open this 

pract7} aim:Recovering and Inspecting deleted files
Check for Deleted Files ,Recover the Deleted Files , Analyzing and Inspecting the recovered files
steps:-i)open fkt imager --file-- add evidence item--select logical drive
finish--then go to orphan folder and right click --export files--browse location u want to export and open that file...


pract9} aim:- Email Forensics 
- Mail Service Providers 
- Email protocols 
- Recovering emails 
- Analyzing email header
steps:- i)create new case,-->next next-->next --> then add evidence item-->select individual file-->select ‘Jim_shu’s.pst’ this file from cf folder
-->ok-->next-->next-->select any email-->then we get output in bottom of screen -->in op copy standard header information.
ii) then open browser and search message header analyzer and paste that one & click on analyze headers 
iii)go to fkt --> file->report wizard -->fill case info-> next-->next next --> click on yes we get html file
iv)again go to ftk --> file--> export files--> click on html view and next and ok

pract 10} Aim: Web Browser Forensics 
- Web Browser working 
- Forensics activities on browser 
- Cache / Cookies analysis 
- Last Internet activity

i)install browser history examiner click on continue trial
ii)go to file -- capture history--click on capture history
 form this computer --next -- give destination folder and next then capture --> load 
iii) now file--> load history-- click on load history from windows user profile and next
browse mail user folder in windows and next -- 
iv) file --export -- export to html and pdf u will get output

