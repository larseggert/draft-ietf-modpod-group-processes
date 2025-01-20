---
title: "IETF Community Moderation"
category: bcp

docname: draft-ietf-modpod-group-processes-latest
submissiontype: IETF
number:
date:
consensus: true
v: 3
venue:
    mail: mod-discuss@ietf.org
    github: larseggert/moderation
    latest: https://larseggert.github.io/moderation/draft-ietf-modpod-group-processes.html

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
and other ways of participating or communicating. It is up to the moderators
to decide which mix of preemptive and reactive moderation to employ as
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

## Composition

The moderator team consists of no less than five
individuals.  The IESG appoints and replaces moderators.
In selecting members, the IESG will take into
account geographic coverage, expected and unexpected absenses, and
team diversity.  The moderator team may expand or contract
based on operational experience.  Apart from appointing and replacing
moderators, the IESG SHALL refrain from the day-to-day operation
and management of the moderator team. The moderators MAY decide to
consult with the IESG when needed.

Because the IESG and IAB are in the appeals chain for moderator team
decisions (see {{appeals}}), the IESG MUST NOT appoint a
moderator who is serving on the IESG or IAB. Individuals serving on
other bodies to which the NomCom appoints members, such as the IETF
Trust or the LLC Board, as well as LLC staff and contractors SHALL
also be excluded from serving on the moderator team. If a moderator
is assuming any such role, they SHALL step down from the moderator team
soon after.

### Team Diversity

Due to the global nature of the IETF, the membership of this team
SHOULD reflect a diversity of time zones and other participant
characteristics that lets it operate effectively around the clock and
throughout the year. Ideally, the moderators should be able to
respond to issues within a few hours.

Team diversity is also important to ensure any participant observing
problematic behavior can identify a moderator they feel comfortable
contacting.

## Scope

The IETF moderator team is responsible for establishing processes to
address moderation needs across all IETF fora, both present and
future, including, but not limited to, mailing lists, chat channels,
and discussions in other systems that the IETF or WGs have chosen to
employ, such as GitHub repositories, Wikis, or issue trackers.

The moderators are authorized to moderate all non-working group
fora, including, the IETF discussion and the last-call mailing lists
and all non-WG mailing lists, as well as area mailing lists.  This
also includes non-WG IETF-sponsored chat mechanisms.

Interactions with WGs are discussed below.

It is not expected that the moderators will be monitoring every
IETF channel, but rather that participants MAY and chairs SHOULD flag
concerns about disruptive behavior to the moderators. However,
the moderators SHOULD actively monitor a small set of key
participation channels, including, for example, the IETF discussion
and last-call mailing lists or the IETF plenary chat channel. The
moderators should decide which channels are in this set based on
their own judgment and community suggestions. (Note that some participation
channels, such as the examples given in the previous sentence, have no
chairs or other community leadership, so the moderators MUST handle those.)

### Non-IETF Communication Channels And Private Communications Excluded

It is important to note that the moderator team only
moderates *public* IETF participation channels. Their mandate does
not extend to problematic behavior in private channels, such as
private chat channels, direct messages, or conversations or other
interactions outside of meetings. In such cases, the Ombudsteam
should be approached.

### IETF Working Groups

The management and moderation of participation channels associated
with various IETF groups, including their mailing lists, chat channels
and in-person, remote, or interim meetings remains primarily a task of
the relevant group's management, such as WG chairs. However,
moderators are available for consultation and assistance should issues
arise, and they MAY proactively confer with the group management over
potential patterns of behavior. Group participants MAY and chairs
MUST alert the moderators to problematic behavior that rises to the
level that some action is needed. Similarly, when moderators
observe or are alerted to problematic behavior on such channels, they
MUST consult with the group's management to jointly determine an
appropriate response.

Only when necessary MAY the moderators take actions against
someone in a working group setting, but they MUST inform management of
relevant groups, including WG chairs and area directors, when they do
so.

If working group management and moderators have a disagreement about
how to proceed in any given circumstance, before any further action is
taken, the matter should be taken up with the responsible area
director(s) for resolution, and, when more than one area is involved,
with the IESG.

It is anticipated that such disagreements will be exceedingly rare.
The moderators should respect the views of the group management
in such cases, and the group management should respect the moderators'
task of upholding an overall IETF-wide uniformity for
moderation.

## Operations of the Moderator Team and Transparency

Within the bounds of the policies set within this memo and with the
approval of the IESG, the moderator team SHALL define any additional
processes and moderation criteria necessary to execute their role.
Those processes and criteria SHALL be developed with community input
and made public, but need not be documented in the RFC series.

The intent of this memo is to provide the widest possible freedom of
action to the moderators, with a few constraints.  Examples of
actions that could be taken include:

- Automated rate limiting mechanisms;
- Review and approval of submissions/messages;
- A private or public admonishment;
- Temporary or permanent bans in one or more fora.

We stress that these are only examples, and not in any way
prescriptive. The moderator team is free to decide on these actions.

The expectation is that the minimal action necessary to maintain the
comity of a forum will be attempted.

The moderator team is responsible to the IESG.  The IESG
MAY create or designate a forum to facilitate discussion about
moderation, and refer interested parties to that forum.  All actions
taken by the moderator team SHALL be reported to the IESG.  All
bans longer than fourteen (14) days SHALL be reported to the forum in
which the person was banned, as well as to that person, and in the
case of a broad ban, to the community in a manner decided by the IESG.

## Training

The IETF is committed to providing and/or funding training for
appointed moderators as necessary. The IESG will negotiate any
required funding or resources with IETF Administration LLC
{{?RFC8711}}.

## Appeals {#appeals}

Because the moderator team serves at the discretion of the IESG,
any moderation decision can be appealed to the IESG by anyone,
per {{!RFC2026}}. Disagreements with a decision by the moderator team can
brought to their attention. If this does not lead to a resolution, a
decision by the IESG can be appealed to the IAB as described in
{{!RFC2026}}.

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
communicated to the IETF community.

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

The actions of the moderator team are intended to limit the likelihood
of disruptive behavior by a few IETF participants from discouraging
participation by other IETF participants.

# IANA Considerations

This document has no IANA actions.

# Acknowledgments

This document is based on two individual Internet-Drafts,
[draft-ecahc-moderation](<https://datatracker.ietf.org/doc/draft-ecahc-moderation/>)
authored by Lars Eggert, Alissa Cooper, Jari Arkko, Russ Housley and Brian E.
Carpenter, and
[draft-lear-bcp83-replacement](<https://datatracker.ietf.org/doc/draft-lear-bcp83-replacement/>)
authored by Eliot Lear, Robert Wilton, Bron Gondwana and John R. Levine. Many of
the ideas in this document originated in those I-Ds. Robert Sayre authored [draft-sayre-modpod-excellent](<https://datatracker.ietf.org/doc/draft-sayre-modpod-excellent/>), which also originated ideas reflected in this WG document.

These individuals suggested additional improvements to this document:

- Alissa Cooper
- Chris Box
- Eric Rescorla
- Jay Daley
- Joel Halpern
- Melinda Shore
- Michael Richardson
- Rich Salz
- Robert Sayre

--- back

# Changes

{:aside}
> RFC Editor: Please remove this appendix before publication.

## Since draft-ietf-modpod-group-processes-00

- [Spelling fix](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/80)
- [Initial attempt to balance what the moderator defines and what](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/75)
- [Scope and relationship between WG chairs and moderators](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/76)
- [Fix wording, spelling and capitalization.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/88)

## Since draft-ecahc-moderation-01

- Content taken from
  [draft-ecahc-moderation-01](https://datatracker.ietf.org/doc/draft-ecahc-moderation/01/).
  [Updated editors. Acknowledge authors of original pre-WG I-Ds.](https://github.com/larseggert/draft-ietf-modpod-group-processes/pull/65)
