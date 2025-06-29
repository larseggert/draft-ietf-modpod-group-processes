---
title: "IETF Community Moderation"
category: bcp

docname: draft-ietf-modpod-group-processes-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
obsoletes: 3683, 9245
updates: 2418
venue:
    mail: mod-discuss@ietf.org
    github: larseggert/draft-ietf-modpod-group-processes
    latest: https://larseggert.github.io/draft-ietf-modpod-group-processes/draft-ietf-modpod-group-processes.html

author:

-
    name: Lars Eggert
    role: editor
    org: Mozilla
    street: Stenbergintie 12 B
    city: Kauniainen
    code: "02700"
    country: FI
    email: lars@eggert.org
    uri: <https://eggert.org/>
-
    name: Eliot Lear
    role: editor
    org: Cisco Systems
    street: Richtistrasse 7
    code: "8304"
    city: Wallisellen
    country: Switzerland
    phone: "+41 44 878 9200"
    email: lear@lear.ch

normative:

informative:
  AHP:
    title: IETF Anti-Harassment Policy
    date: 2013-11-03
    author:
        - org: IESG
    target: <https://www.ietf.org/about/groups/iesg/statements/anti-harassment-policy/>
  OT:
    title: Ombudsteam
    date: false
    target: <https://www.ietf.org/contact/ombudsteam/>
  MODML:
    title: IESG Guidance on the Moderation of IETF Working Group Mailing Lists
    date: 2000-08-29
    author:
        - org: IESG
    target: <https://www.ietf.org/about/groups/iesg/statements/mailing-lists-moderation/>
  DP:
    title: IESG Statement on Disruptive Posting
    date: 2006-02-16
    author:
        - org: IESG
    target: <https://www.ietf.org/about/groups/iesg/statements/disruptive-posting/>

--- abstract

The IETF will treat people with kindness and grace, but not endless patience.

This memo describes the creation of a moderator team for all the
IETF's various contribution channels. Without removing existing responsibilities
for working group management, this team enables a uniform approach to moderation
of disruptive participation across all mailing lists and other methods of IETF
collaboration.

--- middle

# Introduction

This memo proposes the creation of a moderator team for all the
IETF's various contribution channels. The moderator team is modeled
after, and subsumes, the moderator team for the IETF discussion list
{{?RFC9245}} and is tasked to moderate **all** IETF participation channels.

As a consequence, this memo obsoletes {{!RFC3683}} and the "posting rights"
(PR) action it defines. It also obsoletes {{Section 4 of !RFC9245}}, which
defines the IETF discussion list moderation team. Finally, it updates {{Section
6.1 of !RFC2418}}, because the moderator team will now work together with
working group chairs to moderate disruptive behavior.

## Background {#background}

The IETF community has defined general guidelines for
personal interactions in the IETF {{?RFC7154}}, and the IESG has
defined an anti-harassment policy for the IETF {{AHP}} for which the IETF
community has defined anti-harassment procedures {{!RFC7776}},
empowering an ombudsteam {{OT}} to take necessary action.

Dealing with *disruptive* behavior, however, is not part of the role
of the ombudsteam. {{?RFC3934}} tasks the chairs of each IETF working
group with moderating their group's in-person meetings and mailing
lists, and an IESG statement {{MODML}} describes additional guidance
to working group chairs about how — but not when — to moderate their
lists.

For IETF mailing lists not associated with a working group, another
IESG statement {{DP}} clarifies that the list administrators are
tasked with moderation. And the IETF list for general discussions
has, mostly for historic reasons, a team of moderators that are not
list administrators and operate by a different set of processes
{{?RFC9245}}.

Note that the term "moderation" can refer both to *preemptive*
moderation, where moderators review attempted participation before it occurs
(such as reviewing messages to a mailing list), and *reactive* moderation,
where moderators intervene after problematic participation has occurred. The
IETF historically mainly practiced reactive moderation, with a spectrum from
gentle reminders on- and off-list, all the way to suspension of posting rights
and other ways of participating or communicating. It is up to the moderators
to decide which mix of preemptive and reactive moderation to employ as
part of their processes.

In addition, {{?RFC3683}} defines a process for revoking an
individual's posting rights to IETF mailing lists following a
community last-call of a "posting rights" action (PR-action) proposed
by the IESG, often in response to complaints from the community.

Experience and community input suggests that an evolution of the
existing processes is necessary (see {{motive}}).

## General Philosophy

The cornerstone of our philosophy is first and foremost the individual, whose
responsibility is to further the goals of the organization {{!RFC3935}} in a
manner consistent with the policy laid out in {{!RFC7154}}.

The IETF is an open standards organization.  Engaged, respectful
discussion that is within the scope of a forum should not be considered abuse,
nor should someone be considered abusive solely because they are outside the rough
consensus.  Disagreement and diverse points of view within any standards organization
are to be expected, and are even healthy. However, when someone crosses the line
into disruptive behavior, some action must be taken in order to maintain
decorum of the community.

The moderation policy goals are as follows:

- Apply consistent, fair, and timely moderation of communication across all IETF
  channels without regard to one's position or previous contributions;
- Disagreements about moderation actions are addressed through appeals;
- Balance transparency against both privacy of individuals involved and further
  disruption to the community;
- Allow moderators to reconsider decisions; and
- Provide the broadest possible latitude to moderators, so that they may have the
  flexibility to address a broad range of individuals and circumstances.

Questions about processes detailed below should be answered through the lens
of these aims.

The goal is explicitly **not** punishment, but to maintain an open, welcoming,
non-hostile environment in which all may participate on an equal footing,
regardless of their position or past contributions.

# IETF Moderator Team

This memo proposes a different, uniform approach to moderating the
IETF's various participation channels: a moderator team for the IETF.
The creation of this team intends to address the issues identified
in the previous model {{motive}} and the principles described in the introduction.

## Composition

The moderator team consists of no less than five
individuals.  The IESG appoints and replaces moderators.
In selecting members, the IESG will take into
account geographic coverage, expected and unexpected absences, and
team diversity.  The moderator team may expand or contract
based on operational experience.  Apart from appointing and replacing
moderators, the IESG shall refrain from the day-to-day operation
and management of the moderator team. The moderators may decide to
consult with the IESG when needed.

Because the IESG and IAB are in the appeals chain for moderator team
decisions (see {{appeals}}), the IESG must not appoint a
moderator who is serving on the IESG or IAB. Individuals serving on
other bodies to which the NomCom appoints members, such as the IETF
Trust or the LLC Board, as well as LLC staff and contractors shall
also be excluded from serving on the moderator team. If a moderator
is assuming any such role, they shall step down from the moderator team
soon after.

### Team Diversity

Due to the global nature of the IETF, the membership of this team
should reflect a diversity of time zones and other participant
characteristics that lets it operate effectively around the clock and
throughout the year. Ideally, the moderators should be able to
respond to issues within a few hours.

Team diversity is also important to ensure any participant observing
problematic behavior can identify a moderator they feel comfortable
contacting.

## Training

The IETF is committed to providing and/or funding training for
appointed moderators as necessary. The IESG will negotiate any
required funding or resources with IETF Administration LLC
{{?RFC8711}}.

# Scope

The IETF moderator team is responsible for establishing processes to
address moderation needs across all IETF fora, both present and
future, including, but not limited to, mailing lists, chat channels,
and discussions in other systems that the IETF or WGs have chosen to
employ, such as GitHub repositories, Wikis, or issue trackers.

The moderators are authorized to moderate all
fora, including the IETF discussion and last-call mailing lists
all WG and non-WG mailing lists, area mailing lists, and chat systems in
coordination with the owners (if there are any) of those fora.
Participants
should contact both fora owners and moderators when they have concerns,
and moderators should only act when the owners do not respond in a
timely fashion.  In general, their first act should be to contact the
fora owners, and then only act if the owners remain unresponsive.

In the case of plenary fora, such as the ietf list, last-call list, and
other channels in which all or a large portion of the IETF community
engage, moderators shall act as owners, and they will be the primary
contacts for complaints.

Forum owners and moderators shall act in a manner
consistent with guidelines approved by the IESG.  In cases of
disagreement between the chairs and moderation team
over a moderation decision, the matter should be taken up
with the responsible area director for resolution, or the IETF chair
if a responsible area director cannot be determined or is not assigned.

It is not expected that the moderators will be monitoring every
IETF channel, but rather that participants may and group management
should flag concerns about disruptive behavior to the moderators and
owners of those channels. However,
the moderators should actively monitor a small set of key
participation channels, including, for example, the IETF discussion
and last-call mailing lists or the IETF plenary chat channel. The
moderators should decide which channels are in this set based on
their own judgment and community suggestions. (Note that some
participation channels, such as the examples given in the previous
sentence, have no chairs or other community leadership, so the
moderators must handle those.)

Moderators are expected to be a resource that the community can use
to address problematic contributions.

## Non-IETF Communication Channels And Private Communications Excluded

It is important to note that the moderator team only
moderates *public* IETF participation channels. Their mandate does
not extend to problematic behavior in private channels, such as
private chat channels, direct messages, or conversations or other
interactions outside of meetings. In such cases, the Ombudsteam
should be approached.

# Operations and Procedures of the Moderator Team and Transparency

Within the bounds of the policies set herein and with the
approval of the IESG, the moderator team shall define any additional
processes and moderation criteria necessary to execute their role.
Those processes and criteria shall be developed with community input
and made public, but need not be documented in the RFC series.

The intent of this memo is to provide the widest possible freedom of
action to the moderators, with a few constraints.  Examples of
actions that could be taken include:

- Automated rate limiting mechanisms;
- Review and approval of submissions/messages;
- A private or public admonishment;
- Temporary or permanent bans in one or more fora.

We stress that these are only examples, and not in any way
prescriptive. The moderator team is free to decide on these or other
actions.

The expectation is that the minimal action necessary to maintain the
comity of a forum will be attempted.

Any attempt to circumvent or otherwise ignore a moderation action
is a demonstration of bad faith that may warrant further moderation.

The moderator team is responsible to the IESG.  The IESG
may create or designate a forum to facilitate discussion about
moderation, and refer interested parties to that forum.  All actions
taken by the moderator team shall be reported to the IESG,
as well as to those against whom those actions are directed.
To address inappropriate contributions in a timely manner, only
bans longer than fourteen (14) days shall be reported to the forum in
which the person was banned, and in the case of a ban that spans more
than one forum, to the community in a manner decided by the IESG.

Content removal or redaction from IETF archives are not moderation
actions, and are therefore beyond the scope of this memo.

## Appeals {#appeals}

Because the moderator team serves at the discretion of the IESG,
any moderation decision can be appealed to the IESG by anyone,
per {{!RFC2026}}. Disagreements with a decision by the moderator team can
be brought to their attention. If this does not lead to a resolution, a
decision by the IESG can be appealed to the IAB as described in
{{!RFC2026}}.

## Reinstatement

People and circumstances change.  Individuals who have been banned
from a forum may request reinstatement.  Any such request must be
directed to the entity who made the decision (e.g., moderation team,
working group chairs, etc.) or their successors.  That party may at
their discretion
reinstate someone, conditionally or unconditionally.  So as to avoid
denial of service attacks on our processes, decisions to not reinstate
someone who has been the subject of a moderation action
may not be appealed.  Any reinstatement is a grace and not a right.
Decisions to
not reinstate someone may not be appealed.  Requests for reinstatement
may be entertained only a year after the initial decision, and then
only annually.

A ban imposed prior to this process shall be reconsidered only in
accordance with the processes in place at the time of the ban,
even if the corresponding RFC has been formally obsoleted.

# Relationship to other IETF functions

## Relation to the Ombudsteam

The moderator team shall complement the efforts of the IETF
ombudsteam {{OT}}, whose focus on anti-harassment and operation
shall remain unchanged. The moderator team and ombudsteam are
expected to work together in cases that may involve both disruptive
behavior and harassment; they may determine the most effective way to
do so in each case. For example, the ombudsteam may decide to have
one of their members serve as a liaison to the moderator team.

The ombudsteam has strict rules of confidentiality. If a moderation
case overlaps with an ombudsteam case, confidential information must
not be shared between the teams.

## Relation to the IETF LLC

The Board of Directors of the IETF Administration LLC (IETF LLC) has
fiduciary duty for the overall organization, which includes the duty
to protect the organization from serious legal risk that may arise
from the behavior of IETF participants.

This protection may include the need for the IETF LLC to take
emergency moderation actions. These emergency actions are expected to
be taken only when the IETF LLC has received legal advice that such
action is necessary, and therefore extremely rare in frequency. Some
examples of where this might be necessary are:

- Someone making credible threat of harm to other IETF participants.
- Someone using IETF mailing lists and/or websites to share content
  where publishing that content on IETF lists and/or websites brings
  serious legal risk.
- Someone making credible threats of legal action where any form of
  interaction with them on IETF mailing lists may have serious legal
  consequences for the IETF.

If any such action is taken, the IETF LLC should, except where
limited by legal advice to the contrary, inform the IESG as soon as
possible, providing full details of the subject of the action, nature
of the action, reason for the action and expected duration. The IETF
LLC should also inform the moderator team and IETF community, except
where it receives legal advice to the contrary.

As such an action would be taken by the IETF LLC in order to protect
the IETF according to its fiduciary duty, then it cannot allow that
to be overridden by a decision of the moderation team or the IESG.
The subject of any such action may request a review by the IETF LLC
board, as documented in section 4.7 of {{!RFC8711}}

Any such action taken by the IETF LLC under this section of this
policy, is not subject to the rest of this policy.

## Relation to the IRTF

The Internet Research Task Force (IRTF) {{?RFC2014}} is a peer
organization separate from the IETF that is governed by its own
set or rules and processes. {{Sections 3, 6 and 7 of
?I-D.perkins-irtf-code-of-conduct}} discuss rules for participating
in the IRTF and moderation of IRTF participation channels.

# Security Considerations

The usual security considerations {{?RFC3552}} do not apply to this
document.

Potential abuse of the moderation process for the suppression of
undesired opinions is counteracted by the availability of an appeals
process, per {{appeals}}.

The actions of the moderator team are intended to limit the likelihood
of disruptive behavior by a few IETF participants from discouraging
participation by other IETF participants.

# IANA Considerations

No IANA actions are requested.

# Acknowledgments

This memo is based on two individual Internet-Drafts,
[draft-ecahc-moderation](<https://datatracker.ietf.org/doc/draft-ecahc-moderation/>)
authored by Lars Eggert, Alissa Cooper, Jari Arkko, Russ Housley and Brian E.
Carpenter, and
[draft-lear-bcp83-replacement](<https://datatracker.ietf.org/doc/draft-lear-bcp83-replacement/>)
authored by Eliot Lear, Robert Wilton, Bron Gondwana and John R. Levine.
Robert Sayre authored
[draft-sayre-modpod-excellent](<https://datatracker.ietf.org/doc/draft-sayre-modpod-excellent/>),
which also originated ideas reflected in this work.  Pete Resnick provided the basis for
how the moderators interact with list / forum leadership.

These individuals contributed additional improvements:

- Alissa Cooper
- Chris Box
- Eric Rescorla
- Jay Daley
- Joel Halpern
- Melinda Shore
- Michael Richardson
- Rich Salz
- Robert Sayre
- Brian Carpenter

--- back

# Changes

{:aside}
> RFC Editor: Please remove this appendix before publication.

## Since draft-ietf-modmod-group-processes-06

- [Normalize handling of moderation across all fora](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/129)

## Since raft-ietf-modpod-group-processes-05

- [New attempt to address moderation/WG interactions](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/126)

## Since draft-ietf-modpod-group-processes-04

- [Use plain English instead of BCP 14 language](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/120)

## Since draft-ietf-modpod-group-processes-03

- [Non-normative Examples of Disruptive Behavior](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/121)

## Since draft-ietf-modpod-group-processes-02

- [Say which RFCs this obsoletes and updates.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/105
)
- [Address issue 113](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/116)
- [Rewrite philosophy](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/103)
- [Reinstatement](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/107)
- [Content removal is not moderation.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/109)

## Since draft-ietf-modpod-group-processes-01

- [Update "Relation to the IETF LLC".](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/92)
- [Point to relevant IRTF material.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/97)
- [Add some text to explain the role of moderators.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/100)

## Since draft-ietf-modpod-group-processes-00

- [Spelling fix](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/80)
- [Initial attempt to balance what the moderator defines and what](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/75)
- [Scope and relationship between WG chairs and moderators](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/76)
- [Fix wording, spelling and capitalization.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/88)
- [Editorial changes to acknowledgments.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/87)

## Since draft-ecahc-moderation-01

- Content taken from
  [draft-ecahc-moderation-01](https://datatracker.ietf.org/doc/draft-ecahc-moderation/01/).
  [Updated editors. Acknowledge authors of original pre-WG I-Ds.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/65)

# Problems with the Previous Approach {#motive}

The previous approach to moderation of disruptive participation
through chairs, list administrators, and moderator teams, combined
with the IESG-led process of PR-actions, has proven to be less than
ideal:

- The IETF community has not been able to agree on a common definition
  of disruptive behavior. Therefore, chairs and list administrators
  apply individually different criteria when making decisions, and
  participants have different expectations for when PR-actions are
  warranted.

- The moderation process that chairs and list administrators need to
  follow {{?RFC3934}} is slow and cumbersome, which makes it
  ill-suited to situations that escalate quickly. It also assumes
  that the originator of disruptive behavior is a misguided
  participant who can be reasoned with and who will change their
  ways.

- Chairs and list administrators may only enact moderation actions for
  their single list, which is ill-suited when a pattern of disruptive
  behavior spans multiple lists. Also, chairs and list administrators
  may not be fully aware of disruptive behavior that spans multiple
  lists, due to not being subscribed to some of them.

- PR-actions, which can address disruptive behavior across several
  lists, are cumbersome and slow, and the community has not been able
  to agree on a common definition of disruptive behavior. This has
  led to a situation where PR-actions are rarely used, and when they
  are used, they are perceived as very heavy-handed.

- For a given mailing list, participants may not feel comfortable
  reporting disruptive behavior to a chair or list administrator, for
  various reasons. For mailing lists not associated with working
  groups, list administrators are not even publicly identified - they
  can only be contacted through an anonymous alias address. This
  exacerbates the problem, because participants may not be
  comfortable reporting disruptive behavior to an anonymous party.

- The IETF offers participation not only through in-person meetings
  and mailing lists, which are the two channels of participation for
  which moderation processes are currently defined. IETF business
  also happens in chat channels, remote meeting participation
  systems, virtual meetings, wikis, GitHub repositories, and more.
  How disruptive behavior is moderated in these channels is currently
  undefined.

# Non-Normative Examples of Disruptive Behavior {#examples}

The list below describes some types of disruptive behavior, but it
is non-exhaustive.

- unsolicited bulk e-mail;

- discussion of subjects unrelated to IETF policy, meetings,
  activities, or technical concerns;

- uncivil commentary, regardless of the general subject;

- announcements of conferences, events, or activities that are not
  sponsored or endorsed by the Internet Society or IETF;

- repeatedly arguing counter to a WG charter that has been approved by
  the IESG; and

- "sealioning", where a participant makes incessant requests for evidence or
  data, even while remaining superficially polite.

These items are just examples. The moderator team's task consists of
subjective judgement calls. Behaviors not listed here might require
moderation, and it is not possible to write a complete list of all such
behaviors.
