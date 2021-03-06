---
title: Call Statuses
---

# Call Statuses 

This guide explains call statuses like started, ringing, answered, rejected, busy, unanswered, timeout, failed, complete and machine. Since everyone is familiar with the phone, these concepts are pretty straightforward. 


## Lifecycle

Each call goes through a sequence of statuses in its lifecycle:

A call may pass from Started to Ringing to Answered to Complete but there are many different sets of sequences for statuses in a call's lifecycle. Below is a schematic diagram outlining all possible paths. 

![Visual diagram of Call statuses. A description of the text is given in the next section.](/assets/images/call-statuses-rtc-diagram.png)

## Statuses

Here is list of of all call statuses: 

- **started** : The call is created on the Nexmo platform
- **ringing** : The destination has confirmed that the call is ringing
- **answered** : The destination has answered the call
- **rejected** : The call attempt was rejected by the destination
- **busy**: The destination is on the line with another caller
- **unanswered**: The call was canceled by the caller
- **timeout**: The call timed out before it was answered
- **failed**: The call failed before reaching the destination
- **complete**: The call is completed successfully
- **macine**: The call is answered by a machine

These statuses are valid for all 1:1 call combinations such as IP to IP, IP to PSTN, PSTN to IP. 

## Disclaimer 

While Nexmo, the Vonage API Platform strives to provide the most accurate status, we have little to no control over statuses like busy, rejected, unanaswered and failed, most of which depend in the largest part upon the carriers themselves. More specifically, a call might not be completed because the callee was on another line(busy) but it is relayed as rejected by the carrier. 
