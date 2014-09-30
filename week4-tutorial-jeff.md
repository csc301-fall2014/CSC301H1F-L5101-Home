Week 4 Tutorial: Designing an MVP
====

The domain: software for DNA sequencing lab
----
* Sequencing: turn sample in test tube into digital sequence ACTGGACT....
* Sequencing is expensive, but lots of biology labs need it
    * So, universities establish central sequencing centre
* You pay sequencing centre from your lab budget
    * You give them sample, they give you back the digital sequence

The users
----
1. The researcher
    * Likely an overworked, underpaid grad student
    * He doesn't want to deal with software
        * He just wants his sequence back so he can get on with his research
2. The sequencing tech
    * Her job is to take submitted samples, sequence them, then return these data to the researcher
    * Again: busy, underpaid, not a programmer -- wants software to get out of the way, be unobtrusive
3. The sequencing administrator
    * aka "the bean counter"
    * Wants to know which labs are using sequencing, how much they're paying, what costs of sequencing centre are

The plan
----
* MVP will be our first release
    * Anything less than MVP is useless to the centre -- must support at least the researcher and the sequencing tech
    * *Any* software will be big improvement on current pen/paper system
    * All high priority features will be implemented for MVP. Low/med come later

Features for researcher
----
* User permissions -- we must present different systems to researcher and sequencing tech (med priority)
    *  We don't *need* this for MVP -- we're in university setting, so we can trust people to be who they say they are
*  Monitor status of sequencing jobs -- is it done yet? (med priority)
    * Explicit listing not necessary -- if files not available for network-based access, then they're not ready
* E-mail notifications of sequencing status (low priority)
* Initial information entry before sequencing -- name, sample ID, etc. (high priority)
* Network-based access to sequence results (high priority)
* Idea: can we use existing issue tracker like [JIRA](https://www.atlassian.com/software/jira)?
    *  JIRA: you have tasks, users, status of task, notifications ... this sounds a lot like our domain
    *  JIRA has an API, so we could later build our own frontend, but continue using JIRA as our backend

Features for sequencing tech
----
* Needs access to initial data accompanying sample (high priority)
* Must be able to link output on computer attached to sequencer to the customer record (high priority)
* Barcodes on test tubes could ease information retrieval (med priority)

Architecture
----
* Build desktop app for local users (sequencing tech), web app for customers
    * Customers could also enter data in computer in sequencing centre, when dropping off their samples
* We need tons of storage for sequencing results (multi-GB text files), but not much computation
    * Can delete sequencing results ater they're downloaded -- but what if user doesn't download them for a month?
 * Can we build this in three months?
   * We have ~10 programmers working 40 hours/week
   * Consensus: yes, definitely -- we'll follow an agile process
