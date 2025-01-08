---
title: "IETF Community Moderation"
category: bcp

docname: draft-ecahc-moderation-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
venue:
    mail: mod-discuss@ietf.org
    github: larseggert/moderation
    latest: https://larseggert.github.io/moderation/draft-ecahc-moderation.html

author:

-
    name: Lars Eggert
    org: Mozilla
    street: Stenbergintie 12 B
    city: Kauniainen
    code: "02700"
    country: FI
    email: lars@eggert.org
    uri: https://eggert.org/
-
    name: Jari Arkko
    org: Ericsson
    city: Kauniainen
    code: "02700"
    country: FI
    email: jari.arkko@ericsson.com
-
    name: Russ Housley
    org: Vigil Security
    email: housley@vigilsec.com
-
    name: Brian E. Carpenter
    ins: B. Carpenter
    org: The University of Auckland
    abbrev: Univ. of Auckland
    extaddr: School of Computer Science
    street: PB 92019
    city: Auckland
    code: 1142
    country: NZ
    email: brian.e.carpenter@gmail.com

normative:

informative:
  AHP:
    title: IETF Anti-Harassment Policy
    date: 2013-11-03
    author:
        - org: IESG
    target: https://www.ietf.org/about/groups/iesg/statements/anti-harassment-policy/
  OT:
    title: Ombudsteam
    date: false
    target: https://www.ietf.org/contact/ombudsteam/
  MODML:
    title: IESG Guidance on the Moderation of IETF Working Group Mailing Lists
    date: 2000-08-29
    author:
        - org: IESG
    target: https://www.ietf.org/about/groups/iesg/statements/mailing-lists-moderation/
  DP:
    title: IESG Statement on Disruptive Posting
    date: 2006-02-16
    author:
        - org: IESG
    target: https://www.ietf.org/about/groups/iesg/statements/disruptive-posting/

--- abstract

This document describes the creation of a moderator team for all of the
IETF's various contribution channels. Without removing existing responsibilities
for working group management, this team enables a uniform approach to moderation
of disruptive participation across all mailing lists and other methods of IETF
collaboration.

--- middle

# Introduction

This document proposes the creation of a moderator team for all of the
IETF's various contribution channels. This moderator team is modeled
after, and subsumes, the moderator team for the IETF discussion list
{{?RFC9245}}.

# Conventions and Definitions

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT",
"SHOULD", "SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this
document are to be interpreted in their normal English sense; they are shown
in uppercase for emphasis and clarity.

{:aside}
> TODO: Get feedback from the community whether this redefinition of BCP14
> terms in process documents is something they support.

# Motivation {#motiv}

The IETF community has defined general guidelines of conduct for
personal interaction in the IETF {{?RFC7154}}, and the IESG has
defined an anti-harassment policy for the IETF {{AHP}} for which the IETF
community has defined anti-harassment procedures {{!RFC7776}},
empowering an ombudsteam {{OT}} to take necessary action.

Dealing with *disruptive* behavior, however, is not part of the role
of the ombudsteam. {{?RFC3934}} tasks the chairs of each IETF working
group with moderating their group's in-person meetings and mailing
lists, and an IESG statement {{MODML}} describes additional guidance
to working group chairs about how - but not when - to moderate their
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
and other ways of participating or communicating. It is up to the moderator
team to decide which mix of preemptive and reactive moderation to employ as
part of their processes.

In addition, {{?RFC3683}} defines a process for revoking an
individual's posting rights to IETF mailing lists following a
community last-call of a "posting rights" action (PR-action) proposed
by the IESG, often in response to complaints from the community.

This fractured approach to moderation of disruptive participation
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
  lists, due to not being subscribed to some of the affected.

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

# IETF Moderator Team

This document proposes a different, uniform approach to moderating the
IETF's various participation channels: a moderator team for the IETF.
The creation of this team intends to address the issues identified
in {{motiv}}.

## Scope

The IETF moderator team consists of a number of individuals
that SHALL moderate all the IETF's various
current and future participation channels. At present, these include
mailing lists, chat channels, and discussions in other systems that
the IETF or WGs have chosen to employ, such as GitHub repositories,
Wikis, or issue trackers.

The moderator team consists of no less than five individuals,
to establish some minimum basis for consensus-based team decisions
and geographic spread, but realistically needs to have several more
members to spread the moderation load and provide redundancy
in the cases of absences, etc. It is up to the moderator team to determine
a useful team size.

It is not expected that the moderator team will be monitoring every
IETF channel, but rather that participants MAY and chairs SHOULD flag
concerns about disruptive behavior to the moderator team. However,
the moderator team SHOULD actively monitor a small set of key
participation channels, including, for example, the IETF discussion
and last-call mailing lists or the IETF plenary chat channel. The
moderator team should decide which channels are in this set based on
their own judgment and community suggestions. (Note that some participation
channels, such as the examples given in the previous sentence, have no
chairs or other community leadership, so the moderation team MUST handle those.)

It is important to note that the moderation team only
moderates *public* IETF participation channels. Their mandate does
not extend to problematic behavior in private channels, such as
private chat channels, direct messages, or conversations or other
interactions outside of meetings. In such cases, the Ombudsteam
should be approached.

The management and moderation of participation channels associated
with various IETF groups, inculding their mailing lists, chat
channels and in-person, remote, or interim meetings remains primarily a
task of the relevant group's management, such as WG chairs. However,
moderators are available for consultation and
assistance should issues arise, and they MAY proactively confer with the group
management over potential patterns of behavior. Group participants MAY
and chairs SHOULD alert the moderators to problematic behavior. When moderators
observe or are alerted to problematic behavior on such channels, they
SHOULD consult with the group's management to jointly determine an
appropriate moderation response. The moderation team should respect
the views of the group management in such cases, and the group
management should respect the moderation team's task of upholding an
overall IETF-wide uniformity for moderation.

The moderator team MAY initiate moderation actions by itself;
individual participants SHOULD also alert the team to disruptive
behavior they observe. Participants should be able to contact the
moderator team in ways that are, ideally, integrated into the various
participation channels the IETF offers. The moderator team SHALL keep
the identities of participants requesting moderation confidential.

## Transparency

The moderator team SHALL operate according to a consistent
set of criteria, processes, and actions. The moderator team SHALL
independently define and execute their role. They SHALL maintain a
public set of moderation criteria, processes, actions, and other
material that allows the community to understand and comment on the
role of the team. The moderator team SHOULD consider adopting
moderation criteria, processes, and actions that other technical
communities have found suitable. The moderator team's criteria and
processes SHALL be developed with community input, but they are not
expected to be documented in the RFC series.

Some of these processes may rely on automated mechanisms, such as
rate-limiting emails to lists or messages to chat channels.
(The IETF's deliberately low bar to participation makes it easy to
create throw-away personas for such denial-of-service behavior.)

{:aside}
> TODO: This gives the moderator team broad freedom to define
  processes and actions. Should this document define some boundaries
  for what the moderator team can do?

The moderator team is responsible to the IETF Chair.  The IETF Chair
MAY create or designate a forum to facilitate discussion about
moderation, and refer interested parties to that forum.  All actions
taken by the moderation team SHALL be reported to the IETF Chair,
as well as to the person who is the target of the action.  All
bans longer than fourteen (14) days SHALL be reported to the forum in
which the person was banned, and in the case of a broad ban, to the
community in a manner decided by the IESG.

## Membership

The IETF Chair appoints and replaces members of the moderator team.
Apart from appointing and replacing moderators, the IETF Chair SHALL
refrain from the day-to-day operation and management of the moderator
team. The moderator team MAY decide to consult with the IETF Chair
when needed.

Because the IESG and IAB are in the appeals chain for moderator team
decisions (see {{appeals}}), the IETF Chair MUST NOT appoint a
moderator who is serving on the IESG or IAB. Individuals serving on
other bodies to which the NomCom appoints members, such as the IETF
Trust or the LLC Board, as well as LLC staff and contractors SHALL
also be excluded from serving on the moderator team. If a moderator
is assuming any such role, they SHALL step down from the moderator team
soon after.

## Training

The IETF is committed to providing and/or funding training for
appointed moderators as necessary. The IETF Chair will negotiate any
required funding or resources with IETF Administration LLC
{{?RFC8711}}.

## Appeals {#appeals}

Because the moderator team serves at the discretion of the IETF Chair,
any moderation decision can be appealed to the IETF Chair by anyone,
per {{!RFC2026}}. Disagreements with a decision by the IETF Chair can
brought to their attention. If this does not lead to a resolution, a
decision by the IETF Chair can be appealed as described in
{{!RFC2026}}, as with any other Area Director decision. In this case,
the appeals chain starts with an appeal to the entire IESG.

## Team Diversity

Due to the global nature of the IETF, the membership of this team
SHOULD reflect a diversity of time zones and other participant
characteristics that lets it operate effectively around the clock and
throughout the year. Ideally, the moderator team should be able to
respond to issues within a few hours.

Team diversity is also important to ensure any participant observing
problematic behavior can identify a moderator they feel comfortable
contacting.

## Relation to the Ombudsteam

The moderator team SHALL complement the efforts of the IETF
ombudsteam {{OT}}, whose focus on anti-harassment and operation
SHALL remain unchanged. The moderator team and ombudsteam are
expected to work together in cases that may involve both disruptive
behavior and harassment; they may determine the most effective way to
do so in each case. For example, the ombudsteam MAY decide to have
one of their members serve as a liaison to the moderator team.

The ombudsteam has strict rules of confidentiality. If a moderation
case overlaps with an ombudsteam case, confidential information MUST
NOT be shared between the teams.

## Relation to the IETF LLC

The Board of Directors of the IETF Administration LLC (IETF LLC) has
fiduciary duty for the overall organization, which includes the duty
to protect the organization from legal risk that may arise from
illegal, vulgar, or manifestly harassing behavior of IETF participants.

This protection MAY include the need for the LLC to take emergency moderation
actions. These emergency actions are expected to be extremely rare, of temporary
nature, and the incidents that required them SHOULD be immediately raised with
the moderator team to let them determine any follow-up or more permanent
moderation action. These incidents and the taken emergency action SHOULD also be
communitated to the IETF community.

# Changes to Existing RFCs

Creation of the IETF moderator team requires some changes to existing
RFCs and also requires the IESG to update a number of their
statements. This section describes these changes.

{:aside}
> TODO: Add once we know this I-D will go forward in some form.

# Security Considerations

The usual security considerations {{?RFC3552}} do not apply to this
document.

Potential abuse of the moderation process for the suppression of
undesired opinions is counteracted by the availability of an appeals
process, per {{appeals}}.

The actions of the moderation team are intended to limit the likelihood
of disruptive behavior by a few IETF participants from discouraging
participation by other IETF participants.

# IANA Considerations

This document has no IANA actions.

# Acknowledgments

These individuals suggested improvements to this document:

- Alissa Cooper
- Chris Box
- Eric Rescorla
- Jay Daley
- Melinda Shore
- Michael Richardson
- Rich Salz
- Joel Halpern
- Robert Sayre

--- back
