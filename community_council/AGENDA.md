
# sktime community meeting notes 2023-06-23

**Date:** 
23/06/2023, 4:00pm UTC

**Attendees:**

**Minuting:**

Moderator:

[dev meet-up channel](https://discord.com/channels/723500657255907408/875422707523682335)

[link to minutes on hackmd](https://hackmd.io/LUsu_aLHSDWPg9ofJ3urzg)

## Agenda

1. Review of agenda points

2. Review of minutes
   * 2023-06-16 - https://github.com/sktime/community-org/blob/main/community_council/previous_meetings/20230616-meeting.md

3. Review of outstanding actions
    * action FK: update doc on gov & decision making to include new discord channels
        * not done, track
    * actions re conferences
        * pydata Prague (Aug submission)
            * deadline June 23
            * topics
        * pydata Amsterdam (early June submission)
            * all submitted
            * for review: in sktime gmail

        * action MR - pycon Sweden, check process, requirements, topic
            * still todo, track

        * europython & community sprint
            * action FK: find out about need for ticket to attend if only attending sprint (not conf)
                * sprints are free to attend!
                * https://ep2023.europython.eu/sprints
            * action FK: put attendance into the public actions channel
                * sub-decisions on event in decisions channel

    * actions re governance:
        * action JB: explore and possibly set up anonymous voting, checking out "easypoll.bot" for next time and report
            * dummy vote
            * check reporting results (how)

        * action JS - open issue on voting technology to collect options https://github.com/sktime/community-org/issues/55
                * issues opened
                * track until decision
        * action JS - draft statutes
            * 1st draft finished
            * meeting with FK, shared with MR
            * open questions to be shared today
        * KR - reserved actions, track
            * ongoing, track

        * action MR - draft and put up for discussion treasurer/budgeting proposal (see June 9 for high-level summary)
            * ongoing, track

    * action FK - user registration, voter registration message
        * opened PR for call to action on landing page for user registration

        * draft sth on linkedin, suggestion - together with publicizing vision
            * draft shared in private channel

    
4. scheduling
    * EuroPython
        * prep - who/when
    * governance - statutes, elections

5. FK - proposed expenditure - GitHub LFS
    * timelines
        * reading June 23-30 CoB
        * decision June 30 - July 7 CoB
    * expenditure: 60 USD yearly for 1 tier
        * 50 GB file size, 50 GB monthly bandwidth
        * from sktime open collective
    * context: data repositories have become unreliable
        * occasional changes, no deprecation message
        * impacts users as it suddenly breaks loaders
    * potential technical solutions:
        * option A: fallback - from mirror only if primary source fails
        * option B: buffer - always from mirror, keep mirror update
        * both solutions require our own file hosting
    * GitHub LFS - GitHub based file hosting of large files
        * in line with "open" spirit - anyone can clone and mirror!
        * primary repositories are not easy to replicate
    * affected data repos are ca 10 GB
        * up to 1GB is free on GitHub LFS
    * alternatives: any file hoster (cost usually starts between 1-5 GB size)


7. conferences - update

    * EuroPython - speaker opportunity
        * track speakers
        * track attendance
        * Europython is 17-21 July
    * FK - europython sprint, community sprint
        * reminder of attendance
        * linkedin post

8. governance working group

    * JS - statutes (track)
    * FK - voting/election design
    * JB - easypoll for voting

9. UO - community outreach

    * UO - updates
        * linkedin posts
        * blog medium

10. AOB
