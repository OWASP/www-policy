---

title: Chapters Policy - Draft Regional Proposal (WIP)
layout: col-document
document: Rules of Procedure
tags: Rules of Procedure
notice: 2021-02-23

---

DRAFT Regional chapter PROPOSAL. This document is not policy.

## Overview

Chapters are central to OWASP's mission of achieving community around the world. This policy defines the rules related to starting, running, maintaining, and dissolving OWASP chapters.

## Running a Chapter

### Discoverability

Chapters must be discoverable by new and existing members and participants.

- Chapter activities must appear on the owasp.org website.
- It is strongly recommended to use OWASP's official chapter and event scheduling platform. The Foundation pays event platform fees for active chapters.
- If you use the Foundation's scheduling service, your Chapter's group account must be defined under the OWASP Foundation account. Using the OWASP Foundation's scheduling service provides continuity for chapter members if chapter leadership becomes inactive.
- If you do not use OWASP's official event platform, you must mirror your events (whether automatically or manually) to your chapter page on the owasp.org website. The OWASP Foundation is not obliged to reimburse alternate meeting scheduling services expenses.
- Each chapter is responsible for creating and maintaining their owasp.org chapter home page (see also [Starting a New Chapter](#starting-a-new-chapter) and [Meetings and Activity Requirements](#meetings-and-activity-requirements)).
- A list of the current leaders and email addresses must be listed on the Chapter's web page on owasp.org. Leaders are strongly encouraged to use their @owasp.org email address on their chapter pages.

### Meetings and Activity Requirements

- Attendees do not need to be members. All members of the public are allowed to attend OWASP meetings. However, chapter leaders may organize reasonably restricted chapter events and activities in addition to regular meetings.
- Chapter meetings must be free.
- Chapters should host a minimum of 3 chapter activities a year to maintain an active OWASP chapter. The activity can be in person, virtual, or an [approved OWASP event](https://owasp.org/www-policy/operational/events) run by the OWASP chapter (or in collaboration with another chapter or external organization with the approval of the Foundation).
- Chapter activities are for the benefit of the community and could include, but are not limited to:
- Chapter meetings (traditional meetups)
- Training days
- Capture the Flag/Hack-a-Thon events
- Local/Regional AppSec Days events
- Student-focused activities, at secondary or college level
- Chapter leaders must post chapter activity information (date, time, and location) on the owasp.org chapter page before the event start date.

For chapters using OWASP Meetup Pro, mirroring meetings automatically is simple and easy. Add the following code to make your life a lot easier. In the header, please make sure the `meetup-group` parameter exists and is accurate:

```javascript
meetup-group: your-meetup-group
```

If the meetup-group header is identical to your OWASP Meetup Pro Group name (e.g. `meetup-group: OWASP-Colorado-Springs-Meetup`), the code will automatically mirror your upcoming meeting information as mandated by the policy above.

Add this line to where you would like your upcoming meetings to appear in the body automatically:

```javascript
. { % include chapter_events.html group=page.meetup-group %}
```

(Remove the space between `{` and `%` to make this work on your page)

NB: Per the policy above, if you don't use this, or it's set up incorrectly, you will need to do this step manually. Once an event is complete, please add it to the past events tab. For a more detailed example, see [https://owasp.org/www-projectchapter-example/]

#### Student chapter Activity Requirements

Student chapters must adhere to the City chapter activity requirements.

As many tertiary institutions have extensive time off between academic years or semesters, leaders should plan to meet activity requirements within each semester, as activity is measured over the previous 12 months.

#### Regional chapter Activity Requirements

Regional chapters must meet the following activity requirements:

- EITHER a minimum of THREE (3) activities per year in addition to a larger event under the events policy, e.g., AppSec Day jointly run by all participating branches or Chapters;
- OR a minimum of SIX (6) activities per year, including all branch activities.

Regional branch activities count towards Regional chapter activity requirements. Activities organized by participating City chapters do not count towards Regional chapter activity requirements.

#### Branch Activity Requirements

A Branch must host a minimum of one activity per year but should strive for more.

A Branch that is not meeting its minimum requirements should be reactivated by the Regional chapter Leaders if possible, including nominating a new Branch Organizer. If they are not successful in reactivating the Branch and the Branch continues to fail its requirements, the Regional chapter Leaders must deactivate and even remove the Branch as necessary. This will be monitored yearly by the Chapters Committee.

### Communication

OWASP is a social community, and we need to communicate with our community regularly.

- Chapter leaders should use their owasp.org email address for all OWASP related correspondence.
Chapter leaders should regularly monitor their owasp.org email address and respond within nine business days.
- Requests from OWASP staff, such as expense claims, should be responded to by one or more chapter leaders within nine business days.
- Leaders are encouraged, but not required, to monitor and participate in the [OWASP Leaders List](https://groups.google.com/u/1/a/owasp.org/g/leaders), other Google groups, and the Slack platform.
- OWASP chapters can create and manage their own social media presence and other reasonable communication channels. Chapter leaders must share access to these accounts with all Chapter leaders. The account administration should be handed over to a remaining chapter leader when stepping down.

We recommend that chapter leaders set an [out of office notification](https://support.google.com/mail/answer/25922?co=GENIE.Platform%3DDesktop&hl=en) within their @owasp.org email if they are planning to take leave, so that the chapter members, the Chapter Committee, and Foundation staff are aware of any absences or delays in responding to communications.

## Shared Services

OWASP Foundation will provide chapters with the following shared services at no cost. Chapters are encouraged to use these. Chapter leaders can access these services by submitting a ticket via [Contact Us](https://contact.owasp.org/). If, after nine business days have passed, and reasonable efforts have been made to attempt to utilize shared services, no response is received, the Chapter may, with due care, seek a reasonable alternative, filling out a [Chapter Funding Pre-Approval](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/107) ticket.

- Chapter page on the owasp.org website.
- A chapter scheduling service for meetings and local events with RSVP functionality and hidden video conference details.
- Video conferencing and webinar facilities for virtual meetings and events, and hybrid in-person/virtual events.
- Social messaging app to communicate in real-time with the OWASP community.
- Leaders should join leaders@owasp.org using their owasp.org email address.
- Assistance and resources are available through the [Chapter Committee](https://owasp.org/www-committee-chapter/) and other [OWASP Committees](https://owasp.org/committees/).
- Event insurance covering chapter meetings.

Services identical or like those provided by the Foundation cannot be expensed without [prior approval](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/107). Where possible, all chapters are encouraged to use a service that respects user privacy.

### Shared Services for Regional Branches

Shared services provided by the Foundation will be pooled by the Regional Chapter and not provided directly to the Branches.

## Defining and Naming Chapters

Chapter names should always aim to reduce confusion between the various chapter types to discover search engine. To that end, OWASP defines the following types of chapters and how they should be named:

### Defining and Naming City chapters

City chapters are the primary form of the OWASP chapter, with hundreds of chapters worldwide.

- Approved City chapters are named "OWASP «city name»". City chapter names must not be a regional or country name unless the city name is the country name (e.g., Monaco).
- City chapters are defined for a single city only; a new chapter may be denied approval if another chapter is within 80 km (50 miles).
- City chapter leaders must reside within 80 km (50 miles) of the chapter location.

Exceptions to distance rules may be approved on a case-by-case basis, for example, where travel times between two geographically close chapters are excessive (defined as more than one hour).

### Defining and Naming Student chapters

Students and faculty of institutions of higher education can create Student chapters. As Student chapters are associated with an educational institution, there can be many Student chapters within a city, even cities with a City chapter.

- Student chapters are named "OWASP «institution name»" or where the institution has different campus locations, "OWASP «institution name» «campus»"
- Student chapters are associated with one educational institution in a single geographic area. For example, each educational institution in a city is more than welcome to have its own Student chapter, which is not the case for regular City chapters.
- Student chapters must have at least one student leader and at least one leader from the institution's staff or faculty.

Student chapters in a city with an active OWASP City chapter should make meaningful efforts to collaborate with the local City chapter, and vice versa, as appropriate.

### Defining and Naming Regional chapters

A Regional chapter represents a larger geographic area with a cohesive community that is not limited to a specific city. This might be a state/district/province, a whole country, or a commonly recognized geographic area.

Regional chapters will have higher requirements and will require common consensus from the wider community in the area. (See "Starting a Regional chapter" for more details).

Regional chapter names must be recognized by residents living in the region as commonly associated with the region.

The existence of a Regional chapter does not conflict with the existence of a City chapter co-located in the same region. However, there are additional requirements.

There is no requirement to become a Regional chapter, even if multiple cities wish to run a joint event, and it is completely optional.

### Defining and Naming Regional branches

A Regional chapter may optionally have one or more Branches in more remote locations. A Branch is not a full-fledged Chapter and is considered a local representative of the Regional Chapter. Branches will be approved and managed by the leaders of the Regional Chapter, supported by OWASP Staff.

Branches should follow the naming rules of City chapters.

## Chapter Leadership

Chapter leaders serve as the main point of contact for their chapters and are responsible for ensuring the Chapter complies with all OWASP policies while fulfilling its mission and obligations.

- Chapter leaders are not required to be members, but it is recommended to become one to promote membership.
- Chapter leadership is open to all participants. Leadership is personal and not associated with any organization, company, or employer.
- Each Chapter must have a minimum of 2 and a maximum of 5 Foundation-recognized, official leaders. In the event of a resignation, leadership transition, or new leadership being appointed, a chapter is allowed a grace period of up to 3 months from the event to comply.
- A chapter leader can be a leader of only one Chapter.
- Leaders will sign and return a leader's agreement within 30 days of receipt.
- Each leader will annually confirm upon request within 30 days that they intend to continue volunteering as chapter leader.
- Leaders are encouraged to transition or rotate every 2-3 years (minimum two years, maximum three years) to allow fresh leaders to step up and participate in the chapter operations. Leader selection is at the Chapter's discretion, provided all policies are followed.
- If a chapter's leadership does not have consensus, fair and open elections should be administered with the support of OWASP staff and the [Chapter Committee](https://owasp.org/www-committee-chapter/).
- Any changes in chapter leadership should be done by submitting a ticket with all information to the [New Chapter/Leader Request](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/105) by one of the existing leaders. If the local chapter leadership is inactive, this request can be made by local chapter OWASP members.
- If a leader needs to step down, they should submit a ticket to the [New Chapter/Leader Request](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/105).
- If a leader is no longer reasonably responsive and contributing to the Chapter, the remaining chapter leaders may petition the leader's removal in accordance with the dispute resolution process.

### Student chapter Leadership

Student chapters must adhere to City leadership as above, but in addition:

- Student chapters must have at least one student leader and at least one leader from the institution's staff or faculty;
- If a student graduates from the institution or a faculty member no longer works at the institution, they can no longer be a Student chapter leader.

Student chapters do not need to meet minimum student leadership requirements during a semester or year breaks but must come back into compliance within 30 days of a new semester or year starting.

### Regional chapter Leadership

Regional chapter leaders have more requirements than City or Student chapters:

- Regional Leadership management is the same as per City chapters;
- Regional chapters must have at least three and usually a maximum of five Foundation-recognized leaders. If the region has more than five participating locations, it can have up to seven (7) leaders.

### Regional branch Leadership

A Branch must have at least one active Organizer and up to 3 official Organizers. Branch Organizers do not have to be Leaders but can additionally support the Regional Chapter as Leaders.

Branch Organizers do not automatically become Leaders or Members but may also be Leaders of the Regional Chapter. Branch Organizers do not receive any benefits.

Regional Chapter Leaders should attempt to find cost-effective ways to show appreciation for persistent Organizers. In addition, Regional Chapter Leaders are expected to mentor Branch Organizers in community management and organizing meetups.

## Starting a new chapter

Prospective chapter leaders should familiarize themselves with this policy and the draft [Chapter Handbook](https://owasp.org/www-committee-chapter/#div-resources_for_chapters) prior to submitting the form.

- New chapters must be approved by the Foundation by submitting a request through [Contact Us](https://contact.owasp.org/).
- After the new Chapter is approved, the chapter leader must:
  - Provide GitHub usernames in order to get admin access to your chapter repository.
  - Create new chapter pages within 30 days of GitHub access on the owasp.org website (see [Website Migration Information and Tutorial](https://owasp.org/migration/) for assistance).
  - Log into their owasp.org email account within Google's defined time period, or they will need to log a support ticket via [Contact Us](https://contact.owasp.org/) to have a password recovery email sent to their registered email address.

### Starting a City or Student chapter

All the above requirements for starting a chapter must be met.

### Starting a Regional chapter

Regional Chapters will only be created with the approval of the Chapter Committee after confirming the below requirements (in particular the first three bullet points below).

All of the following requirements must be met to start a new regional chapter.

- All "Starting a New City chapter" requirements must be met;
- Consensus on the creation of a new Regional chapter is required by at least three different City chapter leaders from within the region, each at least 80 km (50 miles) apart;
- All City chapter leaders within the defined region must agree to the creation of the new Regional Chapter, and there must be no *dissenting* City chapter leaders within the region;
- The new region chapter name must be recognized by residents living in the region as commonly associated with the region; and
- If there are overlapping regions, the new Regional Chapter will be the smallest of the overlapping regions that incorporate all participating locations.

Initial leadership must include the leaders from the initial consensus and from at least three different locations.

Regional Chapters must perform a "health check" of the "Starting a Regional Chapter" requirements with the Chapters Committee at least once a year.

### Starting a Regional branch

Regional leaders can create and manage Regional branches.

A Branch cannot exist independently without a managing Regional chapter. A Regional chapter can have multiple Branches. Branches differ from standard City chapters in the following ways:

- Branches will not have their own page on the OWASP website but should be listed on the Regional Chapter's webpage.

If the Regional Conference (as per B.3.b.(i) above) results in a net profit, the Regional Chapter may elect to provide a Meetup.com group or other shared service (under the regular OWASP account) for an active Branch at the Regional Chapter's own expense, if approved by the leaders of the Regional Chapter. This will be provided by OWASP Staff, on condition that the profits from the Regional Conference can cover the costs of the service. The costs of these Branch groups shall not be borne by the OWASP Foundation.

Branches are managed solely by the Regional Chapter and do not directly require Staff involvement. Regional chapter Leaders are responsible for their Branch's meeting requirements, for their continued activities, and for mentoring their Branch Organizers as needed. This will be additionally monitored by the Chapter Committee on a yearly basis.

If a Branch meets the standard requirements for a City chapter, they can opt to "graduate" to a full Chapter, as long as they continue to meet the requirements. However, while this should be encouraged, it is not mandatory, and they may continue as a Branch. If the Branch does become a Chapter, the Regional Chapter must continue to meet its requirements as well.

### Renaming a Chapter

- Any chapter name changes must be approved by the Foundation. A request for approval must be submitted through [Contact Us](https://contact.owasp.org/).

## Inactive Chapters

The OWASP Foundation aims to provide continuity for OWASP chapter members. The following process is to determine inactive chapters and try to install fresh leadership.

- An inactive OWASP chapter is a chapter that has not met [minimum activity requirements](#meetings-and-activity-requirements) defined in this policy.
- An inactive chapter must either be reactivated or dissolved.
- The OWASP Foundation will revoke the inactive chapter leadership and refer the inactive Chapter to the [Chapter Committee](https://owasp.org/www-committee-chapter/) to help find fresh leadership or to run elections to elect new leadership.
- Use this form to [reactivate a chapter](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/105). Where an inactive chapter does not hold a meeting within 90 days of being reactivated, or new leadership could not be appointed within 90 days of failing to meet activity targets, the [Chapter Committee](https://owasp.org/www-committee-chapter/) will discuss the inactive Chapter and vote on it. If agreed, the Chapter will be dissolved by the OWASP Foundation.

## Regional chapter conflict resolution

A Regional Chapter can exist with additional City Chapters that overlap in the same region, in the following circumstances only. In the case of overlapping Regional Chapter and City Chapter, these will be independent of each other and will not have control or influence over the other. In any unresolved event, the Chapters Committee will be the arbiters and provide a final decision.

### Creating a new Regional Chapter where City Chapters exist

New Regional Chapters may only be created upon the approval of the Chapters Committee. If the proposed Regional Chapter meets the requirements set out in "Starting a new Regional chapter," the staff will refer the Regional Chapter leaders to the Chapters Committee.

The Chapters Committee will review the Regional Chapter's proposal and discuss with relevant City Chapters as needed. The Chapters Committee will vote on the proposed Regional Chapter at the next Committee meeting after the review is completed.

In order to create a new Regional Chapter, there must be no existing chapters or active community leaders in the same region that object to the creation of this Regional Chapter, e.g., leaders of a City Chapter in the region claims that there is no regional community, or that the region does not include those cities.

If there are existing City Chapters in the same region, and the leaders of said chapters concur with the Regional Chapter's claims AND agree that the Regional Chapter can coexist, then the overlapping Regional Chapter can be created.

The City Chapter may opt to join the Regional Chapter as a Participating Chapter, downgrade to a Branch, or remain an independent overlapping City Chapter (with no connection to the Regional Chapter).

### Creating a new City Chapter within the region of an overlapping Regional Chapter

Where all requirements are met for starting a new City chapter, and the proposed City chapter lies within the defined region of an existing Regional chapter that meets all regional chapter requirements (including consensus), the requesting City Chapter leaders will first be referred to the leaders of the overlapping Regional Chapter to discuss mutually beneficial solutions, such as organizing an additional Branch of the Regional Chapter. The Chapters Committee will mediate as necessary.

However, if such a solution cannot be mutually agreed upon, the Regional Chapter will not have the power to block the City Chapter from being created. The new City Chapter will be created and exist independently of the Regional Chapter, with no effect on the Regional Chapter and no influence between the two.

The above will only apply if none of the Regional Chapter Leaders are from the same city as the proposed City Chapter. If leaders of the Regional Chapter reside/work in the same city in which the City Chapter is wanted to be created, and there are multiple activities held in the city, they will be considered the leaders of the City Chapter and will independently reach a decision regarding the creation of this City Chapter. The Chapter Committee will interpret this as a situation wherein someone wants to create a new City Chapter in the same city where an active City Chapter exists.

Note that both the City Chapter and the Regional Chapter must continue to meet their respective requirements. In particular, the Regional Chapter must still retain consensus from other community members, excluding the city wherein the City chapter exists. The Regional Chapter must have consensus from leaders in at least three cities, not including the one where the City Chapter is created.

## Finances, Oversight, and Transparency

Chapters are overseen on an operational basis by the [Chapter Committee](https://owasp.org/www-committee-chapter/), the OWASP Foundation staff, and, ultimately, the OWASP Board of Directors. Leaders who have not complied with this policy, leadership privileges may be revoked, suspended, or another action taken. The OWASP Foundation may revoke the leader's access to all OWASP accounts, shared services, including the leader's email, and any privileged functionality upon notification by the Chapter Committee, the OWASP Foundation, or Board of Directors of a breach of this policy.

### Code of Conduct and Other Relevant Policies

All leaders must follow and adhere to the latest published OWASP Foundation [policies and procedures](https://owasp.org/www-policy/). As a US-based 501 (c)(3) non-profit organization, OWASP must follow specific financial and legal guidelines that can change from time to time.

Chapters operate with a great deal of freedom; however, chapters must abide by the latest approved [Code of Conduct](https://owasp.org/www-policy/operational/code-of-conduct), [Foundation Bylaws](https://owasp.org/www-policy/legal/bylaws), and these [policies and procedures](https://owasp.org/www-policy/). Copies of older versions are not relevant.

### Privacy

OWASP membership and participation in chapter meetings are subject to locally applicable data protection regulations (for instance, see [GDPR](https://gdpr.eu)). Where conflicting local regulations exist, Chapter leaders should observe the most restrictive. All chapter meetings must comply with [OECD principles](https://www.oecd.org/sti/ieconomy/oecd_privacy_framework.pdf); the Collection Limitation Principle applies to all activities where personal information of participants is needed. Chapter leaders are not permitted to share member lists, event attendees, or private information with third parties except where operationally necessary and only after informing relevant parties with opt-in acceptance. Chapters should, where possible and not otherwise required by local legislation or compliance requirements, adopt a data minimization approach and delete data that is no longer necessary.

### Submitting Expenses

Chapter-related expenses incurred while holding a chapter meeting within the Chapter's geographic area must comply with the [expense policy](https://owasp.org/www-policy/operational/expense-reimbursement) and must be submitted within 60 days. The OWASP Foundation cannot reimburse chapter expenses for events or activities outside the Chapter's geographic area without prior approval.

The OWASP Foundation will manage regional chapter expenses the same way as City chapter expenses.

#### No Expense Access to Regional branches

Regional branches are not authorized to submit expenses directly. Regional branches must submit expenses via their Regional chapter leadership. Regional chapter leaders must approve regional branch expenses.

### Memberships

Members are the lifeblood of chapters. Memberships must be processed per the [membership policy](https://owasp.org/www-policy/operational/membership)

### Donations

Donations will be processed per the [donation policy](https://owasp.org/www-policy/operational/donations). Direct donations or sponsorships of local chapters are not permitted.

### Free and Paid Events

The OWASP Foundation will process free chapter training events, activities, workshops, and other local events not covered by the Events policy per the [expense policy](https://owasp.org/www-policy/operational/expense-reimbursement). Expense pre-approval limits and leader co-approvals apply.

The OWASP Foundation will process paid local or AppSec Days (formerly regional) events. These events are pre-approved in OCMS per the [Events policy](https://owasp.org/www-policy/operational/events), only if the Event policy applies. The Events policy does not apply to most free chapter meetings, local activities, or minor events. If in doubt, please [raise a ticket](https://contact.owasp.org).

For more information, leaders should review and follow the following policies:

[Expenses policy](https://owasp.org/www-policy/operational/expense-reimbursement)
[Events policy](https://owasp.org/www-policy/operational/events).

### Chapters are Not Legal Entities

The OWASP Foundation has authority over all OWASP chapters, projects, committees, and events. They are not separate legal entities.

### Finances are via OWASP Foundation Only

Chapters are not legal entities. The OWASP Foundation will process all membership dues and funds for transparency, US not-for-profit laws, regulations, and tax compliance. Chapters are not permitted to hold or use independent bank accounts, insurance, donation mechanisms. Chapters cannot ex[ense or use funds transfer mechanisms to store financial value such as gift cards, PayPal or Venmo, or other banking or financial instruments.

### Signing Authority

Chapters operate under the aegis and policies of the OWASP Foundation and are subject to the [OWASP signing policy](https://owasp.org/www-policy/operational/signatory2). As for non-legal entities, chapters leaders and members of chapters cannot sign contracts or enter into agreements with commercial organizations. Chapter leaders should refer all such agreements to the OWASP Foundation for pre-approval and possible signing.

### Supporters and Bartering Arrangements

Chapters are encouraged to obtain local chapter supporters via bartering arrangements (i.e., services, event spaces, or food and beverages are paid for by a chapter supporter) and donations via the OWASP website. Chapters can define the levels and benefits of local Chapter Supporters, including logos on the introduction slides and the Chapter home page. Any contractual agreement, bartering arrangement, or financial transaction must be registered and processed by the Foundation through our [service desk](https://contact.owasp.org/)

### Disputes

OWASP has various dispute resolution mechanisms. Please [contact the Compliance Committee](mailto:compliance@owasp.org) if you are unsure of reporting a complaint or raising a dispute. In general, disputes should be resolved between parties and not in the court of public opinion on social media or mail lists.

Chapter members and leaders can use the following policies and reporting mechanisms to resolve disputes or to report code of conduct breaches, violations of policy, or financial requirements:

- [Conflict resolution policy](https://owasp.org/www-policy/operational/conflict-resolution) for most disputes between participants.
- [Code of Conduct](https://owasp.org/www-policy/operational/code-of-conduct) policy for ethical or conduct breaches.
- The [OWASP Chapter Committee](https://owasp.org/www-committee-chapter/) is the first escalation point.
  - The [Executive Director](https://owasp.org/corporate/) as the second point of escalation, and finally.
  - the [Global Board](https://owasp.org/www-board/).

To report severe policy, financial, or fiduciary misconduct violations, please refer to the [whistleblower and anti-retaliation policy](https://owasp.org/www-policy/operational/whistleblower).

### Sanctioned Countries and Leaders

OWASP must comply with international laws and regulations, including international sanctions. Sanctions take many forms and are often limited in scope to access specific intellectual property, organizations, governments, or individuals.

From time to time, the Executive Director and Community Manager will review sanctions from the EU, USA, and anywhere else the Foundation has an operating entity and apply the following policies.

The OWASP Foundation must comply with US Government or EU sanctions. Breaching sanctions may cause the OWASP Foundation to be subject to fines, civil or criminal liability. The following policies apply against sanctioned individuals, entities, or countries to manage this risk:

a) New chapters cannot be formed.
b) Existing chapters may be disbanded or made independent of the Foundation depending on the nature of the sanctions.
c) For sanctioned leaders and members, the OWASP Foundation will remove individuals from any leadership positions and any membership fees refunded, including Lifetime membership.
d) Access to OWASP materials is free and open-source, and can be obtained through any means, including OWASP shared cloud platforms. OWASP relies solely upon the technical controls in place by our shared cloud platforms to prevent access or prohibit the "export" of such freely available information. The OWASP Foundation has no control over these technical controls. The OWASP Foundation will not subvert these technical controls to allow access in sanctioned countries.

The OWASP Foundation will inform the OWASP Global Board and Chapter Committee of any sanctioned chapters, leadership, or access changes.

The OWASP Foundation will periodically review the list of sanctioned chapters and leaders to determine if the Foundation can restore the Chapter, leadership, and membership.
