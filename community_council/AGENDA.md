# sktime CC meeting agenda

[![hackmd-github-sync-badge](https://hackmd.io/y1OcL1QMQLiZjRwVB0t0RQ/badge)](https://hackmd.io/y1OcL1QMQLiZjRwVB0t0RQ)

**Date:** 
31/05/2022, 5:00pm UTC

**Attendees:**: 

**Location:** `sktime` discord

[governance / community council channel](https://discord.com/channels/723500657255907408/875425974345416734)

## Agenda

1. Review of [last meeting's minutes](https://github.com/sktime/community-org/tree/main/community_council/previous_meetings)


2. Review of actions from May 17 and other outstanding or ongoing actionsw
    1. action TB: sktime domain emails - track
    2. action TB to change URL for readthedocs - track
    3. action FK: write email with list to Arliss. action FK chase, write again.
    4. action FK: scheduling - track
        * bring Thu-Fri and general scheduling up in core devs, formulate vote
        * propose updated schedule when interns have joined (dependent on topics, projects, etc) - post in core 
    5. action TB on budget
        * action TB: prepare monthly spreadsheet, share with CC
    6. action FK related to pydata
        * explore whether sprint possible at pydata
        * explore whether core devs can meet in London around pydata

3. summer programme org updates
    * dev sprint and doc sprint, funding bottleneck
    * UKRI grant, funding model
    * pydata London updates
    * [minutes of org meeting May 30](https://github.com/sktime/community-org/blob/main/community_team/previous_meetings/20220530-meeting.md)

4. UEA grant update
    * discussion not completed on May 17 - no involvement of sktime CC in hiring process?
    * Tony said he cannot attend today (May 31)

5. budget update ???
    * Tony not here
    * committed to sharing spreadsheet, but not done
    * actions?

6. roll-over items, from ages ago:
    * FK: special roles for contributors
    * Patrick - KNIME

7. AOB

## Notes



## Appendix A - special roles for contributors proposal (from Franz)

by FK for discussion, possibly decision

I have seen situations where it would be useful to give non-core-devs elevated access rights to the repo, or a right to review.
I would propose to discuss these and introduce additional roles.

Situation 1: owner of a contributed algorithm or interface

In this case, our rules say the person should be notified if PR is made to their algorithm, and they should be able to review and possibly approve changes to their algorithm (in compliance with sktime rules and interface specifications). Currently, we maintain a CODEOWNERS file for this.
However, the PR notifications and review permissions only work if the user has write access.
Examples: statsforecast, multirocket, augmenters, hcrystalball

Situation 2: "allied" library core devs

Direct dependencies or reverse dependencies may be very active in reporting and reviewing contributions around the relevant dependency interface points. They tend to make PR or review PR with a quick turnaround, especially around the times where we or they move to a new version. Such contributors do not have the capacity to take on full responsibilities of an sktime core dev (because they are already core dev of an allied package), but they - and sktime - may benefit from them acting as core devs around the direct interface points, e.g., having the power to review and approve PR of core devs, push directly to the sktime repo, or getting notifications via CODEOWNERS.
Examples: pycaret, statsforecast, pywatts, tsfresh

for situation 1, we already have a role - algorithm maintainer. We may have to specify how this translates into access rights to the repo.
For situation 2, we could introduce the role of allied or affiliated core dev.


## Appendix B - KNIME (from Patrick)

from Patrick: Potential Cooperation with KNIME (https://www.knime.com)
    * KNIME is a software to create and productionize data science using one easy and intuitive environment
    * KNIME is currently working on python M/L functionality 
    * We might cooperate with KNIME on integrating sktime their software by adapters
    * Advatanges: increase visibility of sktime - integrate into an easy to use GUI with a large (commercial) customer base, might be part of some hackathon? Other options (thought og pydata initially)?
    * Disadvantages: KNIME is partially commercial, but distribtues its software open source (GNU)
