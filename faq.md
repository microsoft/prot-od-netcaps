# Network Captures & Protocol Overview Documents - Frequently Asked Questions

## What do these network captures represent?
The network captures map to the examples of common usage scenarios described in Windows Protocols Overview Documents. For example, in MS-FASOD File Access Services Protocols Overview at http://msdn.microsoft.com/en-us/library/jj216083.aspx, Example 2 at http://msdn.microsoft.com/en-us/library/jj216101.aspx describes the sequence of events when a client accesses a file in a domain. The corresponding network capture file MS-FASOD_Example2_Win2016_X64_Win10_X64_Domain.matp -- which is included in the [MS-FASOD]-160926-captureALL.zip file at https://winprotocoldoc.blob.core.windows.net/productionwindowsarchives/MS-FASOD/[MS-FASOD]-160926-captureALL.zip -- contains all the network traffic for that example.

## Where can I find the latest network capture zips?
Zip files of all the latest network captures (for Windows 10 and Windows Server 2016, generated in September 2016) can be found on the individual title pages for each Overview Document. For example, the network captures for MS-FASOD can be found under the CAPTURE links at https://msdn.microsoft.com/en-us/library/jj216083.aspx.

## Where can I find the Overview Documents associated with these captures?
The Windows Protocols Overview Documents are available on MSDN (in HTML, DOCX, and PDF formats) at http://msdn.microsoft.com/en-us/library/hh128055.aspx.

## What's the file format of the capture files?
Newer Individual network capture files for Windows 10 are in Microsoft Message Analyzer .matp format; older ones are in Network Monitor .cap format. All capture files associated with a particular Overview Document are then collected together into a single .ZIP file and published.

## Are .cap format versions of the latest network captures available?
Yes. This GitHub project also contains .cap format versions of the .matp format network captures, including the annotations.

## What tool can I use to view and analyze these captures?
You'll first need to install the required parsers from https://github.com/Microsoft/WindowsProtocolTestSuites. You can then use Network Monitor (3.4 download at http://www.microsoft.com/en-us/download/details.aspx?id=4865) or Message Analyzer (latest version download at http://www.microsoft.com/en-us/download/details.aspx?id=44226), WireShark, or any other network analysis tool to view and analyze the capture files.

## What do the comments in the capture files mean?
Selected frames in each capture file are annotated to match the numbered steps described for the corresponding scenario in the overview documents. They help you better understand the message sequencing and the examples themselves. 

## Where can I find more information about how to install the parsers?
See https://www.codeplex.com/Download?ProjectName=euodcap&DownloadId=463012.

## Where can I find more I information about how to analyze the capture files?
For Network Monitor, see https://www.codeplex.com/Download?ProjectName=euodcap&DownloadId=463012 and for Message Analyzer, see http://technet.microsoft.com/en-us/library/jj673503.aspx.

## Can I contribute new captures or modify existing ones?
Yes! The files in this repository are the same files that were uploaded to Azure. You can tell us about issues you find or suggest a change at https://github.com/Microsoft/prot-od-netcaps/issues, or fork a branch and annotate, modify, and add new captures - we welcome all contributors.
