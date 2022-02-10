---

title: Chapters Policy - Draft (WIP)
layout: col-document
document: Rules of Procedure
tags: Rules of Procedure
#notice: 2022-03-21

---

{% include draft-notice.html %}

This is a DRAFT Chapter policy incorporating improvements to the existing policy as well as incorporating a standardized regional model created by the Chapter Committee after more than a year of consultations with all OWASP regional chapters. Please provide comments on this policy via the [Community Review Process](https://owasp.org/www-policy/operational/community-review-process).

## Overview

Chapters are central to OWASP's mission of building a community of appsec professionals and developers around the world. This policy defines various chapter types, starting, running, maintaining, and dissolving OWASP chapters. Prospective chapter leaders should familiarize themselves with this policy and the [Chapter Committee leader resources](https://owasp.org/www-committee-chapter/#div-resources_for_chapters) prior to submitting the form.

## Running a Chapter

### Discoverability

Chapters must be discoverable by new and existing members and participants.

- Chapter activities must appear on the owasp.org website.
- Chapter leaders should use OWASP's official chapter and event scheduling platform. The OWASP Foundation pays event platform fees for active chapters.
- If you use the OWASP Foundation's scheduling service, your Chapter's group account must be defined under the OWASP Foundation account. Using the OWASP Foundation's scheduling service provides continuity for chapter members if chapter leadership becomes inactive.
- If you do not use OWASP's official event platform, you must mirror your events (whether automatically or manually) to your chapter page on the owasp.org website. The OWASP Foundation is not obligated to reimburse for the use of alternative platform service expenses.
- Each chapter is responsible for creating and maintaining their owasp.org chapter home page (see also [Starting a New Chapter](#div-starting-a-new-chapter) and [Meetings and Activity Requirements](#div-meetings-and-activity-requirements)).

### Meetings and Activity Requirements

- Attendees do not need to be members. All members of the public are allowed to attend OWASP meetings. However, chapter leaders may organize restricted chapter events and activities in addition to regular meetings.
- Chapter meetings must be free to attend, both in monetary and access terms
- Chapters must host a minimum of 3 chapter activities a year to maintain an active OWASP chapter. The activity can be in person, virtual, or an [approved OWASP event](https://owasp.org/www-policy/operational/events) run by the OWASP chapter (or in collaboration with another chapter or external organization with the approval of the OWASP Foundation).

Chapter activities are for the benefit of the community and could include, but are not limited to:

- Chapter meetings - virtual, hybrid, or in-person gatherings or meeting
- Training days
- Capture the Flag/Hack-a-Thon events
- Local/Regional AppSec Days events
- Student-focused activities, at secondary or college level
- Chapter leaders must post to their chapter home page on owasp.org before the meeting or activity starts with sufficient notice for people to attend. All event announcements need to include the date and time, location if in person, and/or the URL to a virtual meeting if hybrid or virtual.

For chapters using the standard OWASP meeting platform, mirroring meetings automatically is simple and easy. Chapter leaders should add the following code to minimize the amount of manual work required. In the header, please make sure the `meetup-group` parameter exists and is accurate:

```javascript
meetup-group: your-meetup-group
```

The above code will automatically mirror your upcoming meeting information if the meetup-group header is identical to your OWASP meeting platform group name. e.g., `meetup-group: OWASP-Colorado-Springs-Meetup`

Add this line to where you would like your upcoming meetings to appear in the body automatically:

```javascript
. { % include chapter_events.html group=page.meetup-group %}
```

(Remove the space between `{` and `%` to make this work on your page)

NB: Per the policy above, if you misconfigure or do not use the above automation, you will need to do this step manually. Once your event is complete, please add it to the past events tab. For a more detailed example, see [https://owasp.org/www-projectchapter-example/]

#### Student chapter Activity Requirements

Student chapters must adhere to the City chapter activity requirements.

As tertiary institutions often have significant vacations between academic years or semesters, Student chapter leaders should plan to meet activity requirements within each semester.

#### Regional chapter Activity Requirements

Regional chapters must meet the following activity requirements:

- EITHER a minimum of THREE (3) activities per year in addition to a significant event under the events policy, e.g., an AppSec Day jointly run by all associated branches or Chapters;
- OR a minimum of SIX (6) activities per year, including all branch activities.

Regional branch activities count towards Regional chapter activity requirements. Activities organized by associated City chapters do not count towards Regional chapter activity requirements.

#### Regional Branch Activity Requirements

A Branch must host a minimum of one activity per year but should strive for more.

A Branch that is not meeting its minimum requirements should be reactivated by the Regional chapter Leaders if possible, including nominating a new Branch Organizer. Regional chapter Leaders must deactivate and remove the Branch if the branch organizers do not meet branch activity requirements. Branch activity compliance will be monitored yearly by the Chapters Committee.

### Communication

OWASP is a social community, and we need to communicate with our community regularly.

- A list of the current leaders and email addresses must be listed on the Chapter's web page on owasp.org.
- Chapter leaders should use their owasp.org email address for all OWASP related correspondence.
- Chapter leaders should regularly monitor their owasp.org email address and respond within nine business days. Leaders can forward owasp.org email to another platform.
- Requests from the OWASP Foundation, such as expense claims, should be responded to by one or more chapter leaders within nine business days.
- Leaders are should monitor and participate in the [OWASP Leaders List](https://groups.google.com/u/1/a/owasp.org/g/leaders), other Google groups, and the Slack platform.
- OWASP chapters can create and manage their own social media presence and other reasonable communication channels. Chapter leaders must share access to these accounts with all of the Chapter's leaders. When a Chapter Leader steps down, the Chapter Leader should hand over the account administration to an active chapter leader.

If Chapter Leaders plan to take leave, please set an [out of office notification](https://support.google.com/mail/answer/25922?co=GENIE.Platform%3DDesktop&hl=en) on your owasp.org email to inform chapter members, the Chapter Committee, and the OWASP Foundation of the potential for delays in responding.

## Shared Services

OWASP Foundation will provide chapters with the following shared services at no cost. Chapters are encouraged to use these. Chapter leaders can access these services by submitting a ticket via [Contact Us](https://contact.owasp.org/).

- Chapter page on the owasp.org website.
- A chapter scheduling service for meetings and local events with RSVP functionality and hidden video conference details.
- Video conferencing and webinar facilities for virtual meetings and events, and hybrid in-person/virtual events.
- Social messaging app to communicate in real-time with the OWASP community.
- Leaders should join leaders@owasp.org using their owasp.org email address.
- Assistance and resources are available through the [Chapter Committee](https://owasp.org/www-committee-chapter/) and other [OWASP Committees](https://owasp.org/committees/).
- Insurance coverage for standard chapter meetings and local activities.

If you are planning to host a longer or larger meeting or activity, or sign a contract with an event space, or take sponsorships, or charge a registration fee, OWASP deems these as AppSec Days events and not local chapter meetings or activities, as they will need a separate event insurance policy and different expense handling. Please [create an AppSec Days regional event in OCMS](https://owasporg.atlassian.net/servicedesk/customer/portal/7/group/19/create/82) and [follow the event policy](https://owasp.org/www-policy/operational/events). Event expenses are managed per event via a budgeting process. The Event policy covers approved spending mechanisms, including the ability for an event to establish awards, scholarships, and grants for various purposes. For more details, please see the Event policy, and the associated [Awards and Scholarships Policy](https://owasp.org/www-policy/operational/awards-and-scholarships) and the [Grant Policy](https://owasp.org/www-policy/operational/grants).

Chapter leaders cannot expense services identical or similar to those provided by the OWASP Foundation without [prior approval](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/107). Where possible, all chapters are encouraged to use a service that respects user privacy.

The Chapter may seek a reasonable alternative to OWASP Foundation shared services only if there is no response to a [Chapter Funding Pre-Approval ticket](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/107) after nine business days outside of published office closures. For Chapter leaders to be reimbursed for alternative platforms after no response, the leader must provide details in the pre-approval ticket that they have selected an alternative platform and any likely costs.

### Shared Services for Regional Branches

Regional Chapter will pool OWASP Foundation shared services for their branches. Shared services are not provided directly to the Branches.

## Defining and Naming Chapters

Chapter names should always reduce confusion between the various chapter types to discover in search engines. To that end, OWASP defines the following types of chapters and how they should be named:

### Defining and Naming City chapters

City chapters are the primary form of the OWASP chapter, with hundreds of chapters worldwide.

- City chapters should be named "OWASP «city name»". City chapter names must not be a regional or country name unless the city name is the country name (e.g., Monaco).
- City chapters are defined for a single city only.
- City chapters should be more than 80 km (50 miles) apart or more than one hour travel distance of the next nearest chapter.
- City chapter leaders should reside in the same country as their city chapter.

The Chapter Committee or the OWASP Foundation may deny approval of a new city chapter if another city chapter is within 80 km (50 miles) or within one hour travel distance of an existing chapter. The Chapter Committee or OWASP Foundation may approve exceptions to distance rules on a case-by-case basis. For example, if two chapters are located close together, but in two separate countries, or if travel times are excessive and would limit participation as a result.

### Defining and Naming Student chapters

Student chapters are encouraged at all educational institutions. Student chapter members, leaders, and faculty have access to discounted OWASP membership rates as a member benefit, as long as membership registration email comes from the institution's email address. Once the student, leader, or faculty is no longer present at the insitution, membership rates revert to the standard rate.

Students and faculty of institutions of higher education can create OWASP Student chapters associated with their educational institution, and optionally campus location.

- Student chapters are named "OWASP «institution name»" or where the institution has different campus locations, "OWASP «institution name» «campus»"
- Student chapters must have at least one student leader and at least one leader from the institution's staff or faculty.
- Every educational institution in a region or city can form a Student chapter at one or more campus locations. Each campus location is treated as a separate Student chapter requiring separate Student chapter leadership, requiring at least one student and one faculty member. There cannot be more than one Student Chapter per campus location.
- Student chapters can be created even if there are nearby city or encompassing regional chapters. Nearby city chapters or encompassing regional chapters do not control the Student chapter. Student chapters should collaborate with nearby city or regional chapters.

Students or Faculty can also create city chapters, as long as all city chapter requirements are met, but they will be city chapters, and do not have access to Student chapter benefits.

### Defining and Naming Regional chapters

A Regional chapter represents a larger geographic area with a cohesive community not limited to a specific city. A region might be a state/district/province, a whole country, or a commonly recognized geographic area.

Regional chapters will have higher requirements and require common consensus from the broader community in the area. (See "Starting a Regional chapter" for more details).

Regional chapters are to be named "OWASP «region name»" Residents living in the region must recognize regional chapter names as commonly associated with the region. For example, a fictional leader from Sto Plains cannot create "OWASP Ramtops" when the regional Chapter aims to encompass Sto Plains, not the Ramtops.

The existence of a regional chapter does not conflict with a City chapter co-located in the same region. However, there are additional requirements to forming a regional chapter. There is no requirement to become a regional chapter, even if multiple cities wish to run a joint event, and it is entirely optional.

### Defining and Naming Regional branches

A Regional chapter may optionally have one or more Branches in more remote locations. A Branch is not a full-fledged Chapter and is considered a local representative of the Regional Chapter. Branches will be approved and managed by the leaders of the Regional Chapter, supported by the OWASP Foundation.

Branches should follow the naming rules of City chapters.

## Chapter Leadership

Chapter leaders serve as the main point of contact for their chapters and ensure they comply with all OWASP policies while fulfilling its mission and obligations.

- Chapter leaders are not required to be members. The OWASP Foundation recommends membership to all leaders and participants to support our mission.
- Chapter leadership is open to all participants. Leadership is personal and not associated with any organization, company, or employer.
- Each Chapter must have a minimum of two (2) and a maximum of five (5) OWASP Foundation-recognized, official leaders. Chapters have three months to have sufficient leaders after a leader's resignation, or if leadership is vacated, such as through inactivity.
- A chapter leader can be a leader of only one Chapter.
- Leaders will sign and return a leader's agreement within 30 days of receipt.
- Each leader will annually confirm upon request within 30 days that they intend to continue volunteering as chapter leader.
- Leaders are encouraged to transition or rotate every 2-3 years (minimum two years, maximum three years) to allow fresh leaders to step up and participate in the chapter operations. Leader selection is at the Chapter's discretion, provided all policies are followed.
- If a chapter's leadership does not have consensus, Chapter leaders should log a ticket to run a free and fair election.
- Any changes in chapter leadership must be done by submitting a ticket with all information to the [New Chapter/Leader Request](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/105) by one of the existing leaders. If the local chapter leadership is inactive, local chapter members can request new leadership using this form.
- If a leader needs to step down, they should submit a ticket to the [New Chapter/Leader Request](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/105).
- If a leader is no longer reasonably responsive and contributing to the Chapter, the remaining chapter leaders may petition the leader's removal following the dispute resolution process.

Leader benefits will only apply to the first five chapter leaders.

### Student chapter Leadership

Student chapters must adhere to City leadership as above, but in addition:

- Student chapters must have at least one student leader and at least one leader from the institution's staff or faculty;
- If a student graduates from the institution or a faculty member no longer works at the institution, they can no longer be a Student chapter leader.

Student chapters do not need to meet minimum student leadership requirements during semester or year breaks. Still, they must come back into compliance within 30 days of starting a new semester or year.

Leader benefits will only apply to the first five Student chapter leaders.

### Regional chapter Leadership

Regional chapter leaders have more requirements than City or Student chapters:

- Regional Leadership management is the same as per City chapters;
- Regional chapters must have at least three and usually a maximum of five OWASP Foundation-recognized leaders. If the region has more than five associated locations, it can have up to seven (7) leaders.

Leader benefits will only apply to the first five regional chapter leaders.

### Regional branch Leadership

A Branch must have at least one active Organizer and up to three official Organizers. Branch Organizers do not have to be Leaders but can additionally support the Regional Chapter as Leaders.

Branch Organizers do not automatically become Leaders or Members but may also be Leaders of the Regional Chapter. Branch Organizers do not receive any benefits.

Regional Chapter Leaders should attempt to find cost-effective ways to show appreciation for persistent Organizers. Regional Chapter Leaders should mentor Branch Organizers in community management and organizing meetings.

Leader benefits will only apply to the first five branch leaders.

## Starting a new chapter

Prospective chapter leaders should familiarize themselves with this policy before submitting an application to start a new chapter. The Chapter Committee maintains [resources for leaders to assist running a chapter](https://owasp.org/www-committee-chapter/#div-resources_for_chapters).

Prospective Chapter leaders must submit a request through [Contact Us](https://contact.owasp.org/), including GitHub account IDs for each leader. If all policy requirements are met, the OWASP Foundation will create the new chapter.

After the new Chapter is created by the OWASP Foundation, chapter leaders must:

- At least one leader, but preferably all leaders, must accept the GitHub invite before it expires. A leader with chapter repository admin rights can grant other leaders admin access.
- Leaders must create new chapter pages in GitHub within 30 days of chapter approval, to publish their chapter's home page automatically on the owasp.org website. See [Website Migration Information and Tutorial](https://owasp.org/migration/) for assistance.
- Log into their owasp.org email account before the Google invite expires. If the invite expires, leaders will need to log a support ticket via [Contact Us](https://contact.owasp.org/) to send a password recovery email to their registered email address.

Automation validation for leader and membership benefits are tied to the leaders.md file. Any changes to chapter leadership should be done via the process outlined in [Chapter Leadership](#div-chapter-leadership). Please do not add or remove leaders from the leaders.md file without first submitting a ticket.

### Starting a Regional chapter

Regional leaders should meet all the following requirements to start a new regional chapter.

- All "Starting a New City chapter" requirements must be met;
- At least three prospective regional chapter leaders, each at least 80 km (50 miles) apart or more than an hour apart for smaller regions, from within the region must have consensus on the creation of a new regional chapter.
- All City chapter leaders within the defined region must agree to the creation of the new Regional Chapter, and there must be no *dissenting* City chapter leaders within the region.
- The new region chapter name must be recognized by residents living in the region as commonly associated with the region; and
- If there are overlapping regions, the new Regional Chapter will be the smallest of the overlapping regions that incorporate all associated locations.

The OWASP Foundation will only create regional Chapters with the approval of the Chapter Committee after confirming regional policy requirements are met.

Regional Chapters must perform a "health check" of the "Starting a Regional Chapter" requirements with the Chapters Committee at least once a year. Failing to meet minimum requirements may be cause for the regional chapter to be asked to resolve the identified policy gaps, leadership added or replaced, or in severe cases, disbanded altogether.

### Starting a Regional branch

Regional leaders can create and manage Regional branches.

A Branch cannot exist independently without a managing Regional chapter. A Regional chapter can have multiple Branches. Branches differ from standard City chapters in the following ways:

- Branches will not have their own page on the OWASP website but should be listed on the Regional Chapter's webpage.

If an AppSec Day event results in a net profit, the Regional Chapter may elect to provide a OWASP meeting platform group or other shared service (under the regular OWASP account) for an active Branch at the Regional Chapter's own expense, if approved by the leaders of the Regional Chapter. Shared services will be provided by the OWASP Foundation, on condition that the profits from the Regional Conference can cover the costs of the service. The OWASP Foundation shall not bear the costs of Branches.

Branches are managed solely by the Regional Chapter and do not directly require OWASP Foundation involvement. Regional chapter Leaders are responsible for their Branch's meeting requirements, continued activities, and mentoring their Branch Organizers as needed. The Chapter Committee will additionally monitor this yearly.

If a Branch meets the standard requirements for a City chapter, they can opt to "graduate" to a full Chapter, as long as they continue to meet the requirements. However, while this should be encouraged, it is not mandatory, and they may continue as a Branch. If the Branch does become a Chapter, the Regional Chapter must continue to meet its requirements.

### Renaming a Chapter

- The OWASP Foundation must approve any chapter name changes. Chapter leaders must submit a request for approval through [Contact Us](https://contact.owasp.org/).

## Inactive Chapters

The OWASP Foundation aims to provide continuity for OWASP chapter members. The following process is to determine inactive chapters and try to install fresh leadership.

- An inactive OWASP chapter is a chapter that has not met [minimum activity requirements](#div-meetings-and-activity-requirements) defined in this policy.
- An inactive chapter must either be reactivated or dissolved.
- The OWASP Foundation will revoke the inactive chapter leadership and refer the inactive Chapter to the [Chapter Committee](https://owasp.org/www-committee-chapter/) to help find fresh leadership or to run elections to elect new leadership.
- Use this form to [reactivate an inactive chapter](https://owasporg.atlassian.net/servicedesk/customer/portal/8/group/20/create/105).

Where an inactive chapter does not hold a meeting within 90 days of being reactivated, or new leadership could not be appointed within 90 days of failing to meet activity targets, the [Chapter Committee](https://owasp.org/www-committee-chapter/) will discuss the inactive Chapter and vote on it. If agreed, the Chapter will be dissolved by the OWASP Foundation.

## Regional chapter conflict resolution

A Regional Chapter can exist with additional City Chapters that overlap in the same region only in the following circumstances. In the case of overlapping Regional Chapter and City Chapter, these will be independent of each other and will not have control or influence over any other chapter. The Chapters Committee will be the arbiters and provide a final decision in any unresolved event.

### Creating a new Regional Chapter where City Chapters already exist

The Chapters Committee must approve all new Regional Chapters. If the proposed Regional Chapter meets the requirements set out in "Starting a new Regional chapter," the OWASP Foundation will refer the Regional Chapter leaders to the Chapters Committee.

The Chapters Committee will review the Regional Chapter's proposal and discuss with relevant City Chapters as needed. The Chapters Committee will vote on the proposed Regional Chapter at the next Committee meeting after completing the review.

There must be no existing chapters or active community leaders in the same region that object to creating this Regional Chapter, e.g., leaders of a City Chapter in the region claim that there is no regional community or that the region does not include those cities.

If there are existing City Chapters in the same region, and the leaders of said chapters concur with the Regional Chapter's claims AND agree that the Regional Chapter can coexist, then the OWASP Foundation can create the overlapping Regional Chapter.

The City Chapter may opt to join the Regional Chapter as an associated Chapter, downgrade to a Branch, or remain an independent overlapping City Chapter (with no connection to the Regional Chapter).

### Creating a new City Chapter within the region of an overlapping Regional Chapter

Where all requirements are met for starting a new City chapter, and the proposed City chapter lies within the defined region of an existing Regional chapter that meets all regional chapter requirements (including consensus), the requesting City Chapter leaders will first be referred to the leaders of the overlapping Regional Chapter to discuss mutually beneficial solutions, such as organizing an additional Branch of the Regional Chapter. The Chapters Committee will mediate as necessary.

However, if Chapter leaders cannot mutually agree upon a solution, the existing Regional Chapter will not have the power to block the new City Chapter from being created by the OWASP Foundation. The new chapter will exist independently of the Regional Chapter, with no effect on the Regional Chapter and no influence between the two.

The above will only apply if none of the Regional Chapter Leaders are from the same city as the proposed City Chapter. If leaders of the Regional Chapter reside/work in the same city in which the City Chapter is wanted to be created, and there are multiple activities held in the city, they will be considered the leaders of the City Chapter and will independently reach a decision regarding the creation of this City Chapter. The Chapter Committee will interpret this as a situation wherein someone wants to create a new City Chapter in the same city where an active City Chapter exists.

Note that both the City Chapter and the Regional Chapter must continue to meet their individual requirements. In particular, the Regional Chapter must still retain consensus from other community members, excluding the city wherein the City chapter exists. The Regional Chapter must have consensus from leaders in at least three cities, not including the one where the City Chapter is created.

## Finances, Oversight, and Transparency

Chapters are overseen on an operational basis by the [Chapter Committee](https://owasp.org/www-committee-chapter/), the OWASP Foundation, and, ultimately, the OWASP Board of Directors. Leaders who have not complied with this policy, leadership privileges may be revoked, suspended, or another action taken. The OWASP Foundation may revoke the leader's access to all OWASP accounts, shared services, including the leader's email, and any privileged functionality upon notification by the Chapter Committee, the OWASP Foundation, or Board of Directors of a breach of this policy.

### Code of Conduct and Other Relevant Policies

All leaders must follow and adhere to the latest published OWASP Foundation [policies and procedures](https://owasp.org/www-policy/). As a US-based 501 (c)(3) non-profit organization, OWASP must follow specific financial and legal guidelines that can change from time to time.

Chapters operate with a great deal of freedom; however, chapters must abide by the latest approved [Code of Conduct](https://owasp.org/www-policy/operational/code-of-conduct), [OWASP Foundation Bylaws](https://owasp.org/www-policy/legal/bylaws), and these [policies and procedures](https://owasp.org/www-policy/). Copies of older versions are not relevant.

### Privacy

OWASP membership and participation in chapter meetings are subject to locally applicable data protection regulations (for instance, see [GDPR](https://gdpr.eu)). Where conflicting local regulations exist, Chapter leaders should observe the most restrictive. All chapter meetings must comply with [OECD principles](https://www.oecd.org/sti/ieconomy/oecd_privacy_framework.pdf); the Collection Limitation Principle applies to all activities where personal information of participants is needed. Chapter leaders are not permitted to share member lists, event attendees, or confidential information with third parties except where operationally necessary and only after informing relevant parties with opt-in acceptance. Chapters should, where possible and not otherwise required by local legislation or compliance requirements, adopt a data minimization approach, and delete data that is no longer necessary.

### Submitting Expenses

Chapter-related expenses incurred while holding a chapter meeting within the Chapter's geographic area must comply with the [expense policy](https://owasp.org/www-policy/operational/expense-reimbursement) and must be submitted within 60 days. The OWASP Foundation cannot reimburse chapter expenses for events or activities outside the Chapter's geographic area without expense pre-approval.

The OWASP Foundation will manage regional chapter expenses the same way as City chapter expenses.

#### No Expense Access to Regional branches

Regional branches are not authorized to submit expenses directly. Regional branches must submit expenses via their Regional chapter leadership. Regional chapter leaders must approve regional branch expenses.

### Memberships

Members are the lifeblood of chapters. Memberships must be processed per the [membership policy](https://owasp.org/www-policy/operational/membership)

### Donations

Donations will be processed per the [donation policy](https://owasp.org/www-policy/operational/donations). Direct donations or sponsorships of local chapters are not permitted.

### Free and Paid Events

The OWASP Foundation will process free chapter training events, activities, workshops, and other local events not covered by the Events policy per the [expense policy](https://owasp.org/www-policy/operational/expense-reimbursement). Expense pre-approval limits and leader co-approvals apply.

The OWASP Foundation will process paid local or AppSec Days (formerly regional) events. According to the [Events policy], these events are pre-approved in OCMS per the [Events policy](https://owasp.org/www-policy/operational/events), but only if the Event policy applies. The Events policy does not apply to most free chapter meetings, local activities, or minor events. If in doubt, please [raise a ticket](https://contact.owasp.org).

For more information, leaders should review and follow the following policies:

[Expenses policy](https://owasp.org/www-policy/operational/expense-reimbursement)
[Events policy](https://owasp.org/www-policy/operational/events).

### Chapters are Not Legal Entities

The OWASP Foundation has authority over all OWASP chapters, projects, committees, and events. They are not separate legal entities.

### Finances are via OWASP Foundation Only

Chapters are not legal entities. The OWASP Foundation will process all membership dues and funds for transparency, US not-for-profit laws, regulations, and tax compliance. Chapters are not permitted to hold or use independent bank accounts, insurance, donation mechanisms. Chapters cannot expense or use funds transfer mechanisms to store financial value such as gift cards, PayPal or Venmo, or other banking or financial instruments.

### Signing Authority

Chapters operate under the aegis and policies of the OWASP Foundation and are subject to the [OWASP signing policy](https://owasp.org/www-policy/operational/signatory2). As for non-legal entities, chapters leaders and members of chapters cannot sign contracts or enter into agreements with commercial organizations. Chapter leaders should refer all such contracts to the OWASP Foundation for pre-approval and subsequent signing.

### Supporters and Bartering Arrangements

Chapter leaders are encouraged to obtain local chapter supporters via bartering arrangements (i.e., services, event spaces, or food and beverages are paid for by a chapter supporter) and donations via the OWASP website. Chapters can define the levels and benefits of local Chapter Supporters, including logos on the introduction slides and the Chapter home page. Any contractual agreement, bartering arrangement, or financial transaction must be registered and processed by the OWASP Foundation through our [service desk](https://contact.owasp.org/)

### Disputes

OWASP has various dispute resolution mechanisms. Please [contact the Compliance Committee](mailto:compliance@owasp.org) if you are unsure of reporting a complaint or raising a dispute. In general, disputes should be resolved between parties and not in the court of public opinion on social media or mail lists.

Chapter members and leaders can use the following policies and reporting mechanisms to resolve disputes or to report code of conduct breaches, violations of policy, or financial requirements:

- [Conflict resolution policy](https://owasp.org/www-policy/operational/conflict-resolution) for most disputes between participants.
- [Code of Conduct](https://owasp.org/www-policy/operational/code-of-conduct) policy for ethical or conduct breaches.
- The first escalation point is the [OWASP Chapter Committee](https://owasp.org/www-committee-chapter/).
  - The [OWASP Foundation Executive Director](https://owasp.org/corporate/) as the second point of escalation, and finally.
  - the [Global Board](https://owasp.org/www-board/).

Please refer to the [whistleblower and anti-retaliation policy](https://owasp.org/www-policy/operational/whistleblower) to report severe policy, financial, or fiduciary misconduct violations.

### Sanctioned Countries and Leaders

OWASP must comply with international laws and regulations, including international sanctions. Sanctions take many different forms. Sanctions are often limited in scope to specific intellectual property, organizations, governments, or individuals.

From time to time, the OWASP Foundation will review sanctions from the EU, USA, and anywhere else the OWASP Foundation has an operating entity and apply the following policies.

The OWASP Foundation must comply with US Government or EU sanctions. Breaching sanctions may cause the OWASP Foundation to be subject to fines, civil or criminal liability. The following policies apply against sanctioned individuals, entities, or countries to manage this risk:

- New chapters cannot be formed.
- Existing chapters may be dissolved or made independent of the OWASP Foundation, depending on the nature of the sanctions.
- For sanctioned leaders and members, the OWASP Foundation will remove individuals from any leadership positions and any membership fees refunded, including Lifetime membership.
- Access to OWASP materials is free and open-source, and can be obtained through any means, including OWASP shared cloud platforms. OWASP relies solely upon the technical controls in place by our shared cloud platforms to prevent access or prohibit the "export" of such freely available information. The OWASP Foundation has no control over these technical controls. The OWASP Foundation will not subvert these technical controls to allow access from sanctioned countries.

The OWASP Foundation will inform the OWASP Global Board and Chapter Committee of any sanctioned chapters, leadership, or access changes.

The OWASP Foundation will periodically review the list of sanctioned chapters and leaders to determine if the OWASP Foundation can restore the Chapter, leadership, and membership.
