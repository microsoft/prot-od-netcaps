# Latest news
November 25 2019 - Microsoft Message Analyzer (MMA) has been retired and removed from public-facing sites on microsoft.com. A private MMA build is available for testing purposes; to request it, send an email to getmma@microsoft.com.

# Archived news
May 30 2019 - Windows 10/Windows Server 2019 (19H1) network captures in WireShark format (.pcapng) and Microsoft Message Analyzer format (.matp) added for MS-ADOD and MS-FASOD and network captures in Microsoft Message Analyzer format (.matp) added for MS-CERSOD and MS-RDSOD.November 5 2018 - Windows RS5 network captures in Microsoft Message Analyzer format (.matp) added for MS-CERSOD and MS-RDSOD,
network captures in WireShark format (.pcapng) added for MS-ADFSOD
June 29 2018 - Windows RS4 network captures in Microsoft Message Analyzer format (.matp) added for 7 ODs: MS-ADOD, MS-AUTHSOD, 
MS-AZOD, MS-FASOD, MS-CERSOD, MS-RDSOD, and MS-VSOD.

# prot-od-netCaps
This project contains annotated network captures for examples in Windows protocols overview documents. 
Overview Documents describe how related protocols work together to support common scenarios and are published at MSDN under 
Windows Protocols/Overview Documents at http://msdn.microsoft.com/en-us/library/hh128055(v=prot.13). 
Use either Network Monitor (NetMon) or Message Analyzer to open and examine the network capture files. 
For more information on setting up and using Netmon with these captures, see  UsingTheEUODCaptures.docx. 
For information on viewing these captures in Message Analyzer, see http://technet.microsoft.com/en-us/library/jj673503.aspx.

## Details on folders
Network captures for the scenarios covered in a particular Overview Document are released together in a single folder with a 
file name composed of the "short name" of the Overview Document, for example [MS-ADFSOD]-captureALL. 
In the .matp capture files included in the folders, the Windows product version used to generate the captures is included in the name, 
for example MS-ADFSOD_Example1_WIN2016_X64_WIN10_X64_Domain.matp. 
In addition, the annotations in each network capture file include the published date (in the footer) of the Overview Document used to 
generate the captures.
