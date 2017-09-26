# Riak Project Proposal v0.1.3

## Contents

* [Document Information](#document-information)
* [Background](#background)
* [Aims](#aims)
* [Short-term objectives and time periods](#short-term-objectives-and-time-periods)
* [Governance](#governance)
* [Development Group](#development-group)
* [Release Management Group](#release-management-group)
* [Project Direction Group](#project-direction-group)
* [Admin Group](#admin-group)

## Document Information

### History

* 2017-08-24 - v0.1.0 - First version created from discussions on Slack.
* 2017-08-26 - v0.1.1 - Updated with feedback from [Slack meeting on 2017-08-25](meeting-minutes/2017-08-25-slack.md).
* 2017-09-01 - v0.1.2 - Updated with feedback given in the past week.
* 2017-09-01 - v0.1.3 - Updated with feedback from [Slack meeting on 2017-09-01](meeting-minutes/2017-09-01-slack.md).

### Authors

These people took active part in the disucssions on Slack providing inspiration, review and feedback of this document.

| Name | Slack alias | Company | Email address |
| --- | --- | --- | --- |
| Nick Adams | nadams | TI Tokyo | nicholas.adams@tiot.jp
| Mark Allen | mrallen1 | Alert Logic | mrallen1@yahoo.com
| Russell Brown | russelldb | Infinity Works | russell@wombat.me
| Peter Clark | peterclark | TI Tokyo | peter.clark@tiot.jp
| Sargun Dhillon | sargun |  | sargun@sargun.me
| Heinz Gies | heinz | Project-Fifo | heinz@licenser.net
| Bryan Hunt | binarytemple | Erlang Solutions Ltd | admin@binarytemple.co.uk
| Damien Krotkine | dams | Booking.com | damien@krotkine.com
| Pedram Nimreezi | deadzen | Zen Enterprise Networks | deadzen@deadzen.com
| Azhar Nisar | azhar.nisar_nhs| NHS Digital | azhar.nisar@hscic.gov.uk
| Gianluca Padovani | gpad | Coders51 | gpadovani@gmail.com
| Alejandro Ramallo | alejandro.ramallo | Leapsight | alejandro.ramallo@leapsight.com
| Steve Roberts | steve_erlang | Erlang Solutions Limited | steve.roberts@erlang-solutions.com
| Bill Smargiassi | smarg | TI Tokyo | bill.smargiassi@tiot.jp
| Stuart Whitfield | sjmw | Erlang Solutions Limited | stuart.whitfield@erlang-solutions.com

### Introduction 

This is a proposal for the structure of a community-led open source project for the promotion and development of Riak and related software. 

This document is not intended to be final, and it is expected to go through considerable revision from discussion with end-users and developers. 

### Purpose 

The purpose of this document is to define a structure for the project and an outline of procedures that shall be implemented by the members of the groups defined in the document.  

### Scope 

The scope of this document is to: 
* define overall aims of the project 
* define the groups needed to make the project work 
* describe who should belong to each group 
* describe what each group does 
* describe how the groups interact 
* common methods and tools 
* timescales 
* funding 

### Naming conventions 

#### Riak 

The open source version of Riak is licensed under the Apache license which means we are entitled to use the name Riak to describe the product (but not in a company name). The new owner of Riak (bet365) has announced they intend to make all Basho IPR open source, so I have assumed the same.  

Riak has commonly referred to Riak KV as well as the larger Riak family. In this document, it shall refer to the family of all Riak products. 

#### Riak {Product Name} 

* Riak KV - the open source version of Riak KV, the key-value store. 
* Riak CS - the open source version of Riak CS, aka Riak S2. 
* Riak TS - the open source version of Riak TS, the time-series store. 

## Background 
([Return to top](#contents))

Much has changed since May when Basho started to demonstrate issues at maintaining company stability. End-users have had their support services cut off, most without notice and with no plan in place by Basho to replace them.  

As the owner and primary developer of Riak has now gone, and the product's Enterprise Edition code is being made Open Source by bet365 (the new owners of all Basho IPR) the viability of the Riak platform has come into question. Some end-users have already made decisions to leave, and some have decided on a wait-and-see for a period of time. 

To stabilize this, we need a single canonical source for Riak and other Basho software to demonstrate to end-users that this platform is stable (won’t disappear), safe (bugfixes, security patches) and under development (new features and new OS support). 

## Aims 
([Return to top](#contents))

The overarching ethos of this project is to produce a high-reliability, light-weight key-value store that can be easily extended with end-user desired functionality.

The aim of this project is to provide: 

* A canonical open source version of source code for Riak. 
* Tested installation packages of Riak for supported OSs. 
* A canonical set of client libraries for Riak.
* Canonical documentation on how to use Riak. 
* Product information on when and why to use Riak. 
* A public and easily understood minimalist structure.  

## Short-term objectives and time periods
([Return to top](#contents))

* Initial Period (starting 2017-08-25)
    * By October 2017 (2017-10-01), this document should reach version 1.0. 
    * By November 2017 (2017-11-01), all groups should have initial members. 
    * By December 2017 (2017-12-01), basic services should be up and running.
    * By February 2018 (2018-02-01), revisit proposal document to discuss possible required changes.
    * By July 2018 (2018-07-01), set a date for the first set of elections and voting.
* Continuing Period (starting 2018-07-01)

## Governance
([Return to top](#contents))

### Overview

The Project Direction Group provides the overall guidance to the project. They decide where the project should go and what is important. Their directives are sent to the Admin Group's Management Team for implementation.

Day-to-day activities will be managed by the Admin Group's Management Team, who will direct members of the Admin Group to ensure the project's services and facilities are working properly. It is similar to the Executive office of a company.

The most important function of the Management Team will be to manage the elections.

### Groups and Teams list 

The Riak Project (aka the Project) refers to all Teams and Groups that make it up. Riak Project Members (aka the Members) refers to all members of all Groups and Teams. 

The Project is made up of four Groups handling different areas. These Groups are the Development Group, the Release Management Group, the Project Direction Group and the Admin Group.

Each Group is made up of Teams which deal with specific areas of responsibility and dependant projects do not dictate the development of their dependencies. For example, a Team might deal with writing source code for Riak Core, which may break Riak KV. The Riak KV Team would then be responsible for patching Riak KV. Teams will work together, and membership is intended to be fluid between them.

* Riak Project (the 'Project')
    * Development Group (a 'Group')
        * Coding Standards Team  (a 'Team')
        * Documentation Standards Team  (a 'Team')
        * N x Riak {subproject} Team – for example: (each a 'Team')
            * Riak Core Team 
            * Riak KV Team 
            * Riak CS Team
            * Riak Client Tools for Java Team 
    * Release Management Group  (a 'Group')
        * Code Approval Team (a 'Team')
        * Testing Team (a 'Team')
        * Build Team (a 'Team')
        * Documentation Team (a 'Team')
    * Project Direction Group  (a 'Group')
    * Admin Group  (a 'Group')
        * Management Team (a 'Team')
        * Commercial Engagement Team (Riak promotion, public websites, etc...) (a 'Team')
        * Finance Team (Handling donations, payments, subscriptions, etc...) (a 'Team')
        * Services Team (running common services like FTP, web, CD/CI servers, email and mailing list provision, backups, etc...) (a 'Team')
        * Feedback Team (collate bug reports, proposal submissions, security notifications, etc...) (a 'Team')

### Election Rules

Elections will happen at least once per year, but may also occur whenever a Group or Team decides by majority vote to call an election. This allows for a Team to get more help if needed.  An Election can be called in one of three ways:
* By the majority (more than 50%) of the members of a Group or Team the Election is for. This allows for Groups or Teams to deal internally with issues.
* By the Management Team. This allows for periodic elections, and emergency actions like when there are no Team members.
* By request of more than 30% of the members of all Groups. This allows for the general opinion to be heard.

Elections are run by the Management Team, and will be done online.

All election details are public, apart from individual votes.

Elections automatically happen if a Team has 0 members. 

Each election will be decided by a Candidate getting a majority vote (more than 50%) of the votes cast. 

A person can only hold one position in the Project Direction Group.

Elections are for specific people, not positions for a company to fill. Shoud a person need to stand-down, a special election would be called.

A company or organisation can only have a maximum of 1 End-User representative, 1 Developer Group representative and 1 Admin Group representative, and an overall maximum of 2 people in the Project Direction Group overall.

For places on the Project Direction Boards, each sub-group (end-users, developers and admin) will have their regular elections staggered so as to be spread out across the year. Special elections can be called at any time, but should not be part of the regular election cycle.

The Election Process shall be:

1. Day 0: An election is called.
2. Within 1 week of step 1: All eligible voters are informed of the election details, and are asked for candidate nominations to be submitted within 14 calendar days. The elcection details sent shall comprise of;
    1. what positions; and
    2. why it was called; and
    3. when the vote will be; and
    4. who can vote.
3. Within 2 weeks of step 2: All nominated people are contacted to confirm they wish to accept their nomination as a Candidate.
4. Within 1 week of step 3: All Candidates have written a short blurb (max 500 works) on why they should be elected and submitted it.
5. Within 1 week of step 4: All eligible voters are informed of all Candidates, their blurbs, and the voting dates.
6. Within 1 week of step 5: The votes are cast and counted. Each voting person shall have one vote.
7. Within 1 week of step 6:
    1. Assuming a win (more than 50%): 
        - The winners take their positions.
    2. Assuming a tie (there are two or more Candidates with an equally largest number of votes): 
        - All Candidates below the tied Candidates are removed from the ballot.
        - The election is re-run from step 5 with the smaller list of Candidates.
    3. Assuming a majority is not achieved (all Candidates get 50% or less): 
        - The Candidate with the lowest number of votes is removed.
        - The election is re-run from step 5 with the smaller list of Candidates.
    4. Assuming a technical failure: 
        - The election is re-run from step 5.

### Voting Eligibility

#### Development Group
* All members of the Development Group will get 1 vote.

#### Development Group Teams
* All members of the Development Group Team will get 1 vote.

#### Release Management Group and Teams
* All members of the Development Group will get 1 vote.

#### Project Direction Group
* All members of the Development Group will get 1 vote for the Developer positions.
* All companies supporting the project through resources or financing in the 6 months prior to an election being called will get 1 vote for the End-User positions.
* All members of the Admin Group will get 1 vote for the Admin position.

* **How to decide membership of PDG for end-users is TO BE DECIDED.** [Issue 3](https://github.com/TI-Tokyo/riak-community-admin/issues/3).

#### Admin Group
* All members of the Admin Group will get 1 vote.

#### Admin Group's Management Team
* All members of the Project Direction Group will get 1 vote.

### Process to change the Project's governance structure or processes

#### General Changes
General changes to the Project's governance structure or processes can be proposed by any project member to the Project Direction Group via the Admin Group's Feedback Team. 

A Project Direction Group member must sponsor a proposal and it must be seconded by another member to then go to a vote of all members. 

The vote is passed with a majority vote of more than 75% of the members of the Project Direction Group. 

This result can be contested by a group consisting of more than 10% of the voting eligible members of the Project, which will lead to a Project-wide referendum held by the same rules as an election.

#### Group-level Changes
Changes that apply to only one Group can be contested by a group consisting of more than 10% of the voting eligible members of the Group in question, which will lead to a Group-wide referendum held by the same rules as an election.

#### Team-level Changes
A Team can change it's internal processes with a majority vote of more than 75% of the eligible voters.

The Project Direction Group can veto the changes voted at on the Team level with a majority vote of more than 50% of the Project Direction Group members.

## Development Group
([Return to top](#contents))

### Overview 
Members of this group actually write the code.

### Membership

Open to anyone actively developing Riak. 

In the Initial Period, this is anyone who registers. 

In the Continuing Period, this is anyone who has committed code in the last 6 months that was either accepted or is undergoing review.

### Member removal 

A Development Group member can be removed from the Development Group by:
* a majority vote (more than 50%) of the other members of the Development Group. A removal vote shall only occur in the case of serious misconduct. 
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
([Return to top](#contents))

### Overview 

This Group does quality and sanity checks to make sure that only high-quality code, tests and documentation goes into official releases. 

### Membership 

In the Initial Period, members will be appointed by the Authors of this document. This gets us up-and-running quickly. 

In the Continuing Period, members of the Release Management Group will be elected by the members of the Development Group. The idea is to get people the developers trust approving their work. 

Each Team should have at maximum 10 members. 

A member is in the Release Management Group for 1 year, but can be re-elected. This stops automatic membership for life, and a healthy turnover of people. 

Anyone in the Development Group can be nominated for membership to any Release Management Group team by anyone at any time before an election is called. 

### Member removal 

A Release Management Group member can be removed from the Release Management Group by:
* a majority vote (more than 50%) of the members of the Release Management Group. A removal vote shall only occur in the case of serious misconduct. This is specifically not done at a team level to stop camps developing.
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

### Code Approval Team Process

1. Receive work packet from a Development Group’s team. 
2. Check code meets Coding Standards Team’s coding standards. 
3. Check code does what it says. 
4. Either return item to the Development Group team for fixes, or passes to Testing Team. 

### Testing Team Process

1. Receive work packet from Code Approval Team. 
2. Check code’s unit tests or other testing scheme cover the functionality of the item. 
3. Check the tests are passed by the code. 
4. Either return item to the Development Group team for fixes or passes to Documentation Team. 

### Documentation Team Process

1. Receive work packet from Testing Team. 
2. Check documentation of what the item does meets Documentation Standards Team’s documentation standards. 
3. Check documentation describes what the item does and how to use it. 
4. Either return item to the Development Group team for fixes or passes to Build Team. 

### Build Team Process

1. Receive work packet from Documentation Team. 
2. Creates build process. 
3. Checks new build works as expected. 
4. Either releases new version to the public, or returns to the Development Group team for fixes. 

## Project Direction Group 
([Return to top](#contents))

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
* By a majority (more than 50%) vote of the other members of the Project Direction Group. A removal vote shall only occur in the case of serious misconduct.
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
([Return to top](#contents))

### Overview 

The Admin Group handles all the support mechanisms to keep the project afloat. These people will be either employed by the corporate sponsors, or just be very dedicated! 

### Membership (excluding Management Team)

Positions are appointed by the Management Team.

### Membership (Management Team)

Positions are elected by the Project Direction Group.

### Management Team 
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
