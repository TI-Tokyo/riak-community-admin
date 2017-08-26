# Riak Community Proposal v0.1.1

## History

* 2017-08-24 - v0.1.0 - First version created from discussions on Slack.
* 2017-08-26 - v0.1.1 - Updated with feedback from Slack meeting on 2017-08-25.

## Authors

*Name (Slack handle) - Company - Email address*

* Mark Allen (mrallen1) - Alert Logic - 
* Russell Brown (russeldb) - Infinity Works - 
* Peter Clark (peterclark) - TI Tokyo - peter.clark@tiot.jp
* Heinz Gies (heinz) - Project-Fifo - 
* Pedram Nimreezi (deadzen) - Zen Enterprise Networks - 
* Azhar Nisar (azhar.nisar_nhs) - NHS Digital - 
* Gianluca Padovani (gpad) - Coders51 - 
* Steve Roberts (steve_erlang) - Erlang Solutions Limitied - 
* Bill Smargiassi (smarg) TI Tokyo - bill.smargiassi@tiot.jp
* Stuart Whitfield (sjmw) - Erlang Solutions Limited - 

## Introduction 

This is a proposal for the structure of a community-led open source project for the promotion and development of Riak and related software. 

This document is not intended to be final, and it is expected to go through considerable revision from discussion with end-users and developers. 

## Purpose 

The purpose of this document is to define a structure for the project and an outline of procedures that shall be implemented by the members of the groups defined in the document.  

## Scope 

The scope of this document is to: 
* define overall aims of the project 
* define the groups needed to make the project work 
* describe who should belong to each group 
* describe what each group does 
* describe how the groups interact 
* common methods and tools 
* timescales 
* funding 

## Naming conventions 

### Riak 

The open source version of Riak is licensed under the Apache license which means we are entitled to use the name Riak to describe the product (but not in a company name). The new owner of Riak (bet365) has announced they intend to make all Basho IPR open source, so I have assumed the same.  

Riak has commonly referred to Riak KV as well as the larger Riak family. In this document, it shall refer to the family of all Riak products. 

### Riak {Product Name} 

* Riak KV - the open source version of Riak KV, the key-value store. 
* Riak CS - the open source version of Riak CS, aka Riak S2. 
* Riak TS - the open source version of Riak TS, the time-series store. 

## Background 

Much has changed since May when Basho started to demonstrate issues at maintaining company stability. End-users have had their support services cut off, most without notice and with no plan in place by Basho to replace them.  

As the owner and primary developer of Riak has now gone, and the product has been made open source by both Basho (for the non-Enterprise Edition code) and bet365 (the new owners of the Enterprise Edition code and all other Basho IPR) the viability of the Riak platform has come into question. Some end-users have already made decisions to leave, and some have decided on a wait-and-see for a period of time. 

To stabilise this, we need a single canonical source for Riak and other Basho software to demonstrate to end-users that this platform is stable (won’t disappear), safe (bugfixes, security patches) and under development (new features and new OS support). 

## Aims 

The overarching ethos of this project is to produce a high-reliability light-weight key-value store that can be easily extended with end-user desired functionality.

The aim of this project is to provide: 

* A canonical open source version of source code for Riak. 
* Tested installation packages of Riak for supported OSs. 
* Canonical documentation on how to use Riak. 
* Product information on when and why to use Riak. 
* A public and easily understood minimalist structure.  

## Short-term objectives and time periods

* Initial Period (starting 2017-08-25)
    * By October 2017 (2017-10-01), this document should be finalised. 
    * By November 2017 (2017-11-01), all groups should have initial members. 
    * By December 2017 (2017-12-01), basic services should be up and running. 
    * By July 2018 (2018-07-01), set a date for the first set of elections and voting.
* Continuing Period (starting 2018-07-01)

## Groups and Teams list 

* Development Group 
    * Coding Standards Team 
    * Documentation Standards Team 
    * N x Riak {subproject} Team – for example: 
        * Riak Core Team 
        * Riak KV Team 
        * Riak CS Team 
        * Riak Client Tools for Java Team 
* Release Management Group 
    * Code Approval Team 
    * Testing Team 
    * Build Team 
    * Documentation Team 
* Project Direction Group 
* Admin Group 
    * Governance Team
    * Commercial Engagement Team (Riak promotion, public websites, etc...) 
    * Finance Team (Handling donations, payments, subscriptions, etc...) 
    * Services Team (running common services like FTP, web, CI/CD servers, email and mailing list provision, backups, etc...) 
    * Feedback Team (collate bug reports, proposal submissions, security notifications, etc...) 

## Governance

### Election Rules

Elections will happen at least once per year, but may also occur whenever a Team decides by majority vote to call an election. This allows for a Team to get more help if needed.  An Election can be called in one of three ways:
* By the majority (more than 50%) of the members of a Group or Team the Election is for. This allows for Groups or Teams to deal internally with issues.
* By the Governance Team. This allows for periodic elections, and emergency actions like when there are no Team members.
* By request of more than 30% of the members of all Groups. This allows for the general opinion to be heard.

Elections are run by the Governance Team, and will be done online.

Elections automatically happen if a Team has 0 members. 

Each election will be decided by a Candidate getting a majority vote (more than 50%) of the votes cast. 

The Election Process shall be:

1. Day 0: An election is called.
2. By day 7: All eligable voters are informed of the election details (what positions, why it was called, when the vote will be, who can vote), and are asked for candidate nominations to be submitted within 14 calendar days.
3. By day 21: All nominated people are contacted to confirm they wish to accept their nomination as a Candidate.
4. By day 28: All Candidates have written a short blurb (max 500 works) on why they should be elected and submitted it.
5. By day 35: All eligable voters are informed of all Candidates, their blubs, and the voting dates.
6. By day 49: The votes are cast and counted.

Assuming a win:

7. By day 56: The winners take their positions

Assuming a draw:

7. Between days 56-61: a run-off election with the top 3 Candidates will cast and counted.

Assuming a technical failure:

7. Between days 56-61, step 5 onwards will be repeated.

### Voting Elegibility

Development Group
* All members of the Development Group may vote.

Development Group Teams
* All members of the Development Group Team may vote.

Release Management Group and Teams
* All members of the Development Group may vote.

Project Direction Group
* All members of the Development Group may vote for the Developer positions.
* All companies supporting the project through resources or financing will get 1 vote for the End-User positions.
* All members of the Admin Group may vote for the Admin position.

Admin Group
* All members of the Admin Group may vote.

Admin Group Governance Team
* All members of the Project Direction Group may vote.

## Development Group

### Overview 
Members of this group actually write the code.

### Membership

Open to anyone actively developing Riak. 

In the Initial Period, this is anyone who registers. 

In the Continuing Period, this is anyone who has committed code in the last 6 months.

### Member removal 

A Development Group member can be removed from the Development Group by:
* a majority vote (more than 50%) of the other members of the Development Group. This should only happen in the case of serious misconduct, such as introducing flaws on purpose, or causing intentional damage to systems. 
* themselves at any time. 

### How they choose what to work on 

* Personal choice (i.e. independent developer). 
* Direction from their employer (i.e. corporate developer). 
* Prioritised list provided by Project Direction Group (anyone). 

### Type of work packets 

* Critical bug fixes. 
* Security patches. 
* Other bug fixes. 
* New features. 

### Source of work packets

* Feedback Team (bugs, security issues). 
* Project Direction Group (new features). 

### Common Process 

1. Pick a work packet. 
2. Read the current spec. 
3. If needed, update the spec and get feedback from others in the relevant Team until spec agreed. 
4. If needed, discuss with Team best implementation. 
5. Write solution, write test code for solution, document solution. Get feedback from CD/CI servers. 
6. When satisfied, commit to branch of relevant repo on GitHub. 
7. Send notification to Code Approval Team for them to look at it. 
8. Fix any issues that the Code Approval Team come back with. 
9. Fix any issues that the Testing Team come back with. 
10. Fix any issues that the Documentation Team come back with. 
11. Fix any issues that the Build Team come back with. 

### Teams 

In general:
* One team per GitHub repo/subproject. 
* Membership expected to overlap between teams. 
* Flat structure – everyone is equal. 

Other teams will include:
* The Coding Standards Team will produce one coding standard per programming language. All code must meet this standard to pass the Code Approval Team. 
* The Documentation Standards Team will produce one documentation standard. All documentation must meet this standard to pass the Documentation Team. 

## Release Management Group 

### Overview 

This Group does quality and sanity checks to make sure that only high-quality code, tests and documentation goes into official releases. 

### Membership 

In the Initial Period, members will be appoints by the Authors of this document. This gets us up-and-running quickly. 

In the Continuing Period, members of the Release Management Group will be elected by the members of the Development Group. The idea is to get people the developers trust approving their work. 

Each Team should have at maximum 10 members. 

A member is in the Release Management Group for 1 year, but can be re-elected. This stops automatic membership for life, and a healthy turnover of people. 

Anyone in the Development Group can be nominated for membership to any Release Management Group team by anyone at any time before an election is called. 

### Member removal 

A Release Management Group member can be removed from the Release Management Group by:
* a majority vote (more than 50%) of the members of the Release Management Group. This should only happen in the case of serious misconduct, such as introducing flaws on purpose, or causing intentional damage to systems. This is specifically not done at a team level to stop camps developing.
* themselves at any time.
* if a member loses an Election.

### Type of work packets 

* Notifications from the Development Group of features or fixes they believe are ready for release.

### Source of work packets 

* The Development Group. 

### How they choose what to work on 

Each team deals with work packets sent from the Development Group in this order: 
* Critical bug fixes. 
* Security patches. 
* Other bug fixes. 
* New Features from the prioritised list from the Project Direction Group. 
* Everything else on a first-come, first-served basis. 

### Code Approval Team Process

1. Receive work packet from a Development Group’s team. 
2. Check code meets Coding Standards Team’s coding standards. 
3. Check code does what it says. 
4. Either return item to the Development Group team for fixes, or passes to Testing Team. 

### Testing Team Process

1. Receive work packet from Code Approval Team. 
2. Check code’s unit tests or other testing scheme cover the functionality of the item. 
3. Check the tests are passed by the code. 
4. Either return item to the Development Group team for fixes or passes to Documentation Team. 

### Documentation Team Process

1. Receive work packet from Testing Team. 
2. Check documentation of what the item does meets Documentation Standards Team’s documentation standards. 
3. Check documentation describes what the item does and how to use it. 
4. Either return item to the Development Group team for fixes or passes to Build Team. 

Build Team Process

1. Receive work packet from Documentation Team. 
2. Creates build process. 
3. Checks new build works as expected. 
4. Either releases new version to the public, or returns to the Development Group team for fixes. 

## Project Direction Group 

### Overview 

The Project Direction Group provides a forum for end-users, supporters and developers to decide on the direction that the Riak open source project should go. They define new features wanted by industry, ensure the new features should be part of Riak, and provide overall guidance for the project. 
In other words, they provide the roadmap. 

### Membership 

In the Initial Period, members of the Project Direction Group will be appointed by the start-up group. This gets us up-and-running quickly.
In the Continuing Period, membership will be by election.

The Group will have three membership categories: 
* End-users – technical representatives from companies/organisations using Riak. 
* Developers – members of the Development Group. 
* Admin – a member of the Admin Group. 
 
There will be 11 positions in the Project Direction Group:
* 5 positions for End-Users.
* 5 positions for Developers.
* 1 position for Admin.

The equal number of positions between End-users and Developers is to ensure a balance between industry desires, technical realities and project ethos.

There will be one Admin member to ensure that required support systems are provided for. 

Each member is in the Project Direction Group for 1 year, but can be re-nominated by their company or re-elected by the Development Group and Admin Group. This stops automatic membership for life, and a healthy turnover of people. 

### Member removal 

Any member can be removed:
* At any time by themselves.
* By a majority (more than 50%) vote of the other members of the Project Direction Group. This should only happen in the case of serious misconduct.
* By losing an Election.

### Type of work packets 

* Proposals submitted by anyone involved with the project. 

### How they choose what to work on 

* At least once per month and more often if needed the Project Direction Group will meet online to go through submitted approvals in order of acceptance.

### Source of work packets 

* The Feedback Team of the Admin Group. 

### Process 

For each proposal: 
1. Evaluate if this should be part of Riak. 
2. Evaluate where in Riak it belongs. 
3. Evaluate how urgent this is. 
4. If more information is needed, send it back to proposer with a list of what is needed for a decision. 
5. Once evaluated, the proposal will then be packaged up as a work packet. 
6. The work packet will be placed in the prioritised list of new features. 
7. The work packet will then be sent to the Development Group. 

## Admin Group 

### Overview 

The Admin Group handles all the support mechanisms to keep the project afloat. These people will be either employed by the corporate sponsors, or just be very dedicated! 

### Membership (excluding Governance Team)

Positions are appointed by the Governance Team.

### Membership (Governance Team)

Positions are elected by the Project Direction Group.

### Governance Team 
In charge of: 
* Executing the vision laid down by the Project Direction Group. 
* Co-ordinating between Groups and Teams. 
* Process revision management:
    * Fixed review points with project wide feedback.
    * Dynamic review points upon issue identification.
* Running elections.

### Commercial Engagement Team 
In charge of: 
* Riak promotion material. 
* Content for public websites. 
* Exhibitions/conferences. 

### Finance Team 
In charge of: 
* Receives all money from sponsoring companies and other donations. 
* Produces public accounts. 
* Pays invoices for all services. 

### Services Team 
In charge of: 
* Running common technical services like FTP, web, CI/CD servers, etc... 
* Managing email addresses, spam, virus checks, mailing lists, etc... 
* Managing domains. 
* Taking regular backups of everything. 

### Feedback and Internal Communications Team 
In charge gathering and distributing: 
* Bug reports. 
* Security reports. 
* New feature proposals.
* Any other issues that need to be reported.
