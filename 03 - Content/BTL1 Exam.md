---
creation date: July 7th 2023
last modified date: July 7th 2023
aliases: []
tags: #📖
---

Primary Categories: [[]] 
Secondary Categories: [[]] 
Links: [[]] 
Search Tag: #📖  

# [[BTL1 Exam]]  
---

# eM Client containing hosts
- Florence Nightingale
	- [x] Extracted
	- [ ] Explored
- Administrator 
	- [ ] Extracted
	- [ ] Explored


## Phishing email 
- invoicehome.uk
- 68.183.238.225

## Malware
- SHA256 - 9ACB79531CE18D940BF2259F0659E9B97DA5B562AD8B8B814C5030240B2BC4DF

## Wireshark
- TCP scan command 
```
ip.src == 172.16.0.2 && tcp.flags.syn == 1 && tcp.flags.ack == 0
```
46544

You have not successfully identified files that could be related to the attacker gaining further access into the target environment. File names and extensions can give away what their contents are.

You have not successfully identified the start time of a network scan. Provided with the type of scan and the source address, we can use these to filter traffic in Wireshark. You could also look in Statistics > Conversations to see the source IP communicate with a number of other IPs on a range of ports.

You have failed to identify the timestamp of a suspicious RDP connection, and the user that was logged in. With Windows Event logs we can look for 4624's that are related to successful logon, and then look for logon type 3 which shows a network logon. There is a log property called 'TargetUsername' that tells us which account is trying to be logged into.

You have unsuccessfully retrieved a port used in a bind shell for persistence. When investigating suspicious registry keys look at the data values held within, as these can disclose commands and file execution.

You have unsuccessfully provided the number of unique (non duplicate) sensitive files interacted with by the attacker. Looking in the staging location, you need to count the number of files that contain sensitive information.

            




















___

## Resources:

| Hyperlink | Info |
| --------- | ---- |


Created Date: July 7th 2023 (09:54 am) 
Last Modified Date: July 7th 2023 (09:54 am)
