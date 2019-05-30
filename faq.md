 # Network Captures & Protocol Overview Documents - Frequently Asked Questions

## What do these network captures represent?
The network captures map to the examples of common usage scenarios described in Windows Protocols Overview Documents. For example, in MS-FASOD File Access Services Protocols Overview at https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-fasod/a8df7cf6-4f73-4441-8319-653618a50da0, Example 2 at https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-fasod/ea5c54be-710c-4267-a2a2-f7e56cba0d13 describes the sequence of events when a client accesses a file in a domain. The corresponding network capture file MS-FASOD_Example2_Win2016_X64_Win10_X64_Domain.matp -- which is included in the [MS-FASOD]-160926-captureALL.zip file at https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-FASOD/[MS-FASOD]-160926-captureALL.zip -- contains all the network traffic for that example.

## Where can I find the latest network capture zips?
Zip files of all the latest network captures (for Windows 10 and Windows Server 2019, generated in May 2019) can be found on the individual title pages for each Overview Document. For example, the network captures for MS-FASOD can be found under the CAPTURE links at https://docs.microsoft.com/en-us/openspecs/windows_protocols/ms-fasod/a8df7cf6-4f73-4441-8319-653618a50da0.

## Where can I find the Overview Documents associated with these captures?
The Windows Protocols Overview Documents are available on Docs.Microsoft.Com (in HTML, DOCX, and PDF formats) at https://docs.microsoft.com/en-us/openspecs/windows_protocols/MS-WINPROTLP/4a1806f9-2979-491d-af3c-f82ed0a4c1ba.

## What's the file format of the capture files?
Newer individual network capture files for Windows 10 are in WireShark .pcapng format and Microsoft Message Analyzer .matp format; older ones are in Network Monitor .cap format. All capture files associated with a particular Overview Document are then collected together into a single .ZIP file and published.

## Are .pcapng format versions of the latest network captures available?
Yes. This GitHub project also contains .pcapng format versions of the .matp format network captures, including the annotations.

## What tool can I use to view and analyze these captures?
You'll first need to install the required parsers from https://github.com/Microsoft/WindowsProtocolTestSuites. You can then use Network Monitor (3.4 download at http://www.microsoft.com/en-us/download/details.aspx?id=4865) or Message Analyzer (latest version download at http://www.microsoft.com/en-us/download/details.aspx?id=44226), WireShark, or any other network analysis tool to view and analyze the capture files.
NOTE: If using Microsoft Message Analyzer or Network Monitor to view the captures, do not reparse the files or else you may lose some or all of the annotations/comments.

## What do the comments in the capture files mean?
Selected frames in each capture file are annotated to match the numbered steps described for the corresponding scenario in the overview documents. They help you better understand the message sequencing and the examples themselves. 

## Where can I find more information about how to install the parsers?
See https://www.codeplex.com/Download?ProjectName=euodcap&DownloadId=463012.

## Where can I find more I information about how to analyze the capture files?
For Network Monitor, see https://www.codeplex.com/Download?ProjectName=euodcap&DownloadId=463012 and for Message Analyzer, see http://technet.microsoft.com/en-us/library/jj673503.aspx.

## Can I contribute new captures or modify existing ones?
Yes! The files in this repository are the same files that were uploaded to Azure. You can tell us about issues you find or suggest a change at https://github.com/Microsoft/prot-od-netcaps/issues, or fork a branch and annotate, modify, and add new captures - we welcome all contributors.
