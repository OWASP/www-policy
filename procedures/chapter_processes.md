---

title: Chapter Procedures (WIP)
layout: col-sidebar

---
v2021.01.07
## Chapter Processes
To create a new chapter repository in GitHub and CRM record of chapter and leaders.(minmum of 2 leaders to start)
**Relevant Policy: [Chapter Policy](https://owasp.org/www-policy/operational/chapters) and Leader Policy**    

**[Start a New Chapter/New Leader](https://owasporg.atlassian.net/servicedesk/customer/portal/7/group/18/create/73) request subitted.**
* Contact Us or on owasp.org> chapter page click and submit request ticket NFRSD ticket# 
  * Review for a minimum of 2 leaders & all required information is included.
  * Check to make sure there is not an existing chapter.
  * Check to make sure there is not a current chapter within 50 miles/80 km  
  * Check to make sure that the leaders’ residence is within 50 miles/80 km of the chapter city.
  * If all the information requested on ticket is not submit, will delay or could cancel processing.
   
**Leaders owasp.org email address MANUAL creation**
   * Google Admin - Admin Console   
![Chapter Processes Admin]({{site.base_url}}/assets/images/GoogleAdmin_User.png)
   * Click User   
   * Click Add New User   
![Add New User]({{site.base_url}}/assets/images/Add_new_user.png)
    * Pop Box appears
    * Fill in First nam
    * Fill in Last name
    * Primary email john.smith@owasp.org
    * Secondary email is the personal email address 
    * Email User Sign-in Info   
![Email Login]({{site.base_url}}/assets/images/Email_login_info.png)
    * Send   
**The OWASP.org email address that is to be used for the leader in leader.md file in chapter repository.**
 Leader will receive a Google WorkSpace email like below. (link is only good for 48 hours)
![Chapter Processes Admin]({{site.base_url}}/assets/images/GoogleWorkspace_email.png)
  
**Slackbot command "/chapter-create"**
* Generates a templated form to create GitHub chapter repository & CRM records.
   * Chapter City name ONLY
   * Chapter leader’s name
   * Chapter leader owasp.org emails
   * City
   * Country
   * Region -6 choices: Africa, Asia, Europe, North America, Oceania, and South America
* SUBMIT to create the GitHub chapter repository and Copper CRM record.
![Slackbot template]({{site.base_url}}/assets/images/chapter_slackbot_temp.png)

**CRM (Copper) MANAUL Entry**
* Chapter file (OWASP-City) 
  * Add JIRA/NFRSD ticket URL or number in field.
  * Check city, country, and region fields were populated
  * Chapter status is set to Active
  * All leaders are related on rightside under "People"
* People - Leader’s record - MANUAL
   * Enter secondary personal email address
   * Job Title
   * Company
   * phone#
   * Address
   * Tag as Chapter leader
   * Contact - General
   * File - attach a copy of resume from NFRSD ticket.
* Send out a Welcome letter in email to leaders.
* Resolve and Close the JIRA ticket. 
**SLA for first response is 72 hours and 144 working hours to complete; pauses when ticket is set to "Waiting for Customer Response"**
**Issues:**
 * All of the owasp.org emails need to be reviewed and validated that users are current members or leaders.
 * JIRA tickets need a complete overhaul.  Update requirements and use of correct fields and workflows. Stop mass grouping Membership, Chapters, Projects, Corporate Members & Sponsors, Events, Marketing and Other

## Add/Change Chapter Leadership Process - same ticket as New Chapter Request
 Relevant Policy: [Chapter Policy](https://owasp.org/www-policy/operational/chapters) and [Leaders Policy](https://owasp.org/www-policy/operational/leader)
    **Remove leader**
    * The Leader(s) stepping down sends an email to the Foundation.  
    * Complimentary membership and owasp.org email address will be suspended when the email is received.
 **Add New leader(s)**
    * Submit [Start New chapter/new leader request ticket](https://owasporg.atlassian.net/servicedesk/customer/portal/7/group/18/create/73)
    * Answer and submit all requested information. (Delay only if the information is missing.)
    * Create owasp.org email address for the leader(s)
    * Resolve and close ticket
    * Leader to update leader.md file in the chapter repository - leader name and leader owarp.org email address
**SLA for first response is 72 hours and 144 working hours to complete; pauses when ticket is set to "Waiting for Customer Response"**
**Issue:** Membership policy does not address what happens to a complimentary membership if a leader steps down or the chapter is deemed inactive. 
OWASP.org email addresses deactivation did not follow a consistant policy when membership or leadership ended. This was and still is manual process.

## Chapter Reimbursement Process
**Relevant Policy:** [Expense Policy](https://owasp.org/www-policy/operational/expense-reimbursement)
   * Submit [Expense Reimbursement](https://owasporg.atlassian.net/servicedesk/customer/portal/4/group/9) request ticket (OSD) 
   * Expense is for $ 250 or under and is applicable to chapters
   * Copy of receipt is attached and is within 60 days of receipt
   * All payment information is included
     * Amount
     * Currency - exchange 
     * Chapter Name
     * Expense and description if applicable
     * Payment method 
   * Assign a leader to Request a Participant for Leader the second approval
**SLAs:** 
    * To respond to OSD JIRA ticket is 72 working hours.
    * Submit expense for reimbursement within 60 days[Expense Policy](https://owasp.org/www-policy/operational/expense-reimbursement)  
    * AP runs twice a month not sure of the two monthly cut off dates to make the AP run.(Virtual)
**Issue:** SLA reponse from second leader is (7 to 9 days) as listed in Chapter policy for a leaders to respond to the request from the Foundation. 
    
**Google Group for Chapter or Chapter leaders creation**
**Relevant Policy:** [Mailing List](https://owasp.org/www-policy/operational/mailing-list), [Code of Conduct](https://owasp.org/www-policy/operational/code-of-conduct) and [Privacy Policy](https://owasp.org/www-policy/operational/privacy)
  * Submit ["Contact Us"](https://owasporg.atlassian.net/servicedesk/customer/portal/7/create/720) Request ticket  
    * Topic: Choose - Request and OWASP email address from the drop down menu.
    * Name: First and Last name
    * Company: Put the Chapter Name
    * Description: Requesting google group for chapter or chapter leaders
    * Submit recieve NFRSD# for records and referene when inquiring.
    * Resolve as done and close JIRA ticket

**Request for Shared Services offered to Chapters at no charge.**
  * Submit ["Contact Us"](https://owasporg.atlassian.net/servicedesk/customer/portal/7/create/72)
    * Topic: Choose - Request Meetup or other Shared Services from drop down menu
    * Name: First and Last name
    * Company: Put the Chapter Name
    * Description: Type shared service requesting
How the staff creates the Virtual Meeting - Slack command /provision-zoom [chapter-url]. Example: Cairo it would be /provision-zoom www-chapter-cairo
Response to the Requestor: "You have been assigned a shared Zoom account. As this is a shared account, you need to coordinate with other groups using the Zoom Scheduler.   Also, you are not allowed to change account settings or the account password.
You will receive two emails shortly. One will contain the name of the account. The other will contain a link to the password. Be sure to check Spam as these emails often wind up there.
How the staff creates the Chapter scheduling service for meeting/activity - LastPass sign in for Meetup using LastPass signin using the City and Country
Response to the Requestor: Send Leader(s) New Meetup templated email in CRM with URL. 
   
**SLA for first response is 72 working hours; pauses when ticket is set to "Waiting for Customer Response"**
**Issue:** 
1. Meetup Groups are set up by city location, not region or country. 
2. Some Leaders do not join or use Meetup. 
3. Allowed to use other social media do not post activity on chapter page.
5. Automation not available to truly identify 3 meeting activity but just identifies activity as simply as opening and closing a file in the chapter repository.  

**Deactivation of Chapter**
**Relevant Policy:** [Chapter Policy](https://owasp.org/www-policy/operational/chapters)
* Review Chapter meetings and activites on chapter page to meet the criteria outlined in the chapter policy.
* Send the inactive chapter(s) name(s)to the Chapter Committee.
* Chapter Committee to reachout to leaders to help reactivate or confirm deactivate within 30 days.
   *  Remove leaders as co-organzier on Meetup Group if applicable
   *  Remove Admin access to Chapter repository
   *  Remove leaders from leader.md file
   *  Suspend OWASP email address. (If individual Does not have a paid membership.)
* Chapter deemed deactivated then deactivate Meetup and email sales rep the name of the group. 
**Issue:**
* Relying on the chapter committee to reachout and respond back to Community Manager within the 30 days.
* Secondary contact information (email address) not available for all leaders and members. 

**Chapter Reactivation**
**Relevant Policy:** [Chapter Policy](https://owasp.org/www-policy/operational/chapters)
* Follow the Start a New Chapter/New Leader BUT 50% of the leadership must be new
**[Start a New Chapter/New Leader](https://owasporg.atlassian.net/servicedesk/customer/portal/7/group/18/create/73) request subitted.**



