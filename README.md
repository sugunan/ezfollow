# Email based incident tracking

Automate the process of email based incident tracking.

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

## Goals of the challenge

* Build a system to automatically identify and categorize inbound emails into issues or requests.
* Also the system should be able to track and manage inbound, outbound emails as well as associated conversations visually.
* Build functionality to track the time taken for each received email ticket and warn or alert operators of the system of possible service level or threshold breach.

## Detail requirement

### Selection of technology

Make sure all tools and frame works selected are open source or custom build by the team. Avoid pirated softwares. Mention all the technologies used while doing presentation. 

### Expected end product

Following are expected feature on the end product. This can be an application which used by tech leads and managers.

* The solution should visualize mail threads as issue / request
  * This should be auto detected based on machine learning / rule engine or any other predefined words detection
  * Also there should be a way to change the category on UI by human
  * If the first mail on a thread from operation team then ignore that complete conversation
    * So maintain a list of mails to mark as operation team
    * Include "zugunan@gmail.com" also as operation team
* Apply priority or urgency to each mail as high, medium or low
  * High: If the mail talk about any urgency or if large group of people require the solution
  * Medium: If the mail doesn't talk about any time line or urgency, But if they still mention about a blocker (actionable item for operation team), then go for medium
  * Low: All the others mark as low
  * Also there should be a way to change the priority on UI by human
* In each email, all the reply and forward should be grouped as conversation
  * The conversation group can be done by utilizing the parameters in the mail object
  * If you want to choose other option then clearly mention how it is efficient then the previous point
* There should be a way to find SLA time lines of each mail thread
  * Refer the matrix provided above and indicate if any of the SLA breached
  * Good to have a way to alert about to breach SLA for each mail thread (before 10 min)
  * It is good to have working hours on SLA clock as Monday to Friday on week days and 8AM to 5PM as office hours

### Architecture and Implementation details

* Provide the complete ER diagram or if it is no SQL then provide the data model with example
* Provide the overall design of the application
* Follow UML standard on the diagrams
* Provide step by step deployment guide
* Provide user guide for the end product
* All the environment variable and SLA matrix should be configurable in single place
* Follow proper design patterns on implementation
* Follow proper coding standards and check for any vulnerabilities
