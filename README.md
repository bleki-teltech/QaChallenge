# QaChallenge
This repository contains solution for QaChallenge#2 - requirement file attached (Teltech QA Tech Challenge #2.pdf).

To summarize - kamailio was brought up on uBuntu linux OS, same platform is hosting SIPp instances, scripts for A and B party are communicating via kamailio.
Kamailio is listening on port 5060, SIPp script for AParty uses port 5062, SIPp script for BParty uses port 5061.

Versions;
OS - Linux 5.4.0-58-generic #64-Ubuntu 
Kamailio - version: kamailio 5.4.3 (x86_64/linux)
SIPPp - sipp-3.6.0

4 test cases were prepared;
- 01_Busy - scenario: A call B, B is busy, call released
- 02_Abandon - scenario: A call B, A abandons the call during ringing, call released
- 03_Reject - scenario: A call B, B rejects the call during ringing, call released
- 04_Connect - scenario: A call B, call connected

Each test case contains following;
- SIPp scripts for A and B party
- pcap trace for single call and multiple calls
- SIPp messages and screen logs for single call and multiple calls
- screenshot of SIPp from putty
