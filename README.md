# Email based incident tracking

Automate the process of email based incident tracking.

## Greeting

Hi Every one
Welcome to challenge 2 of SRE Hack '21.

I'm Sugunan and am here to give you a heads up about this challenge.

Challenge 2 focuses on automate the process of email based incident tracking or ticketing.

## Problem

A support team working on customer issues & requests to provide solutions.

Most of the time customer contact the support team via emails.

Customer expecting to have proactive follow-up on their complains and requests.

The company committed for certain SLA on handling customer requests.

If the SLA violated the company subjected to penalty.

It is the responsibility of team leads to prevent the SLA violations.

Currently each team leads have to go through individual mail box and consolidate reports on customer queries.

This is very resource intense task, and frequently it leads to human errors.

## Details of SLA

SLA means "Service Level Agreement"

The company committed, that each and every customer complain or request will have response and resolution SLA.

And each complain will be given priority as well.

Additionally those complains will be categorized as Incident or Service request (SR).

Find the SLA Matrix on the table as (hh:mm).

###### Matrix for Response

| Priority  | Incident | SR |
| :----- |:-----:| :-----:|
| high   | 00:15 | 01:00  |
| medium | 00:30 | 02:00  |
| low    | 01:15 | 04:00  |

###### Matrix for Resolution

| Priority  | Incident | SR |
| :----- |:-----:| :-----:|
| high   | 02:15 | 04:00  |
| medium | 04:30 | 08:00  |
| low    | 08:15 | 18:00  |

## SR vs Incident

SR is service request which mean customer need some information or help to complete certain task.

Incident is some issue which is blocking the customer from BAU activities.

Incident should be given faster resolution than SR as it is blocking or limiting the operation.

## Priority

Priority or wee can call it as urgency based on how fast the ticket should be handled.
The priority can be number as "1, 2, 3 . . ." where 1 is most serious. Or it can be "High, Medium, Low"

## Expected solution

* Build a system to automatically identify and categorize inbound emails into issues or requests.
* Also the system should be able to track and manage inbound, outbound emails as well as associated conversations visually.
* Build functionality to track the time taken for each received email ticket and warn or alert operators of the system of possible service level or threshold breach.

## Conclution

If you have any further queries, <please join the expert team>



