---

title: Setting Up Events
layout: col-sidebar

---

### Github Repository 

*Not a github admin?  Quick jump to [Configuring the Event](#configureevent)*

For OWASP Foundation Global or similar events, the repository should be created by someone with Github Administrator privileges following the standard event repository naming convention: www-event-YYYY-EVENTNAME, where YYYY is the 4 digit year and EVENTNAME is the name of the event.  For instance, an event named Yolo which is in 2021 would have a repository named www-event-2021-yolo.  In the case where multiple events of the same name occur in the same year, the pattern for the repository name should be www-event-YYYY-MM-EVENTNAME, where MM is the 2 digit month of the event. In addition, the repository should be created from the www-event-example template (see steps below).  The following is a general guideline for event repository creation:

1. On the main [OWASP Github Page](https://github.com/owasp/), Click New
   ![New Repository Image](/www-policy/www-policy/assets/images/event_site_setup_new_repo.png)
2. On the next page, click the Repository template dropdown and select OWASP/www-event-example
   ![Choose Template Image](/www-policy/assets/images/event_site_setup_template.png)
3. Type in a Respository name following the aforementioned conventions, choose the Public option, and click Create repository
   ![Name and Create Image](/www-policy/assets/images/event_site_setup_name_create.png)

The repository will be created after a minute or two.  At this stage, the repository is not yet accessible as a website (this is covered in [Publish the Event](#publishevent), below) 

<a href='' id='configureevent'>

### Configuring the Event

In order to configure the event, it is necessary to be familiar with the general layout of the event site. Note the sections on the following image:

![Event Site Image](/www-policy/assets/images/event_site_setup_layout.png)

The event site will be populated with certain files and folders. We will cover the more commonly edited files when setting up an event site.

#### Header

Note that the header section, above, contains the menu, the Join Us button, the event title, where it is located, the dates, and the background image.  Nearly everything in this section can be modified by modifying the event-details.yml file which is located in the _data folder in the repository:

![Event Site Data Files Image](/www-policy/assets/images/event_site_setup_data_files.png)

Within the event-details.yml file, you will find the following sections:

| Section | Description |
| -----: | --- |
| title | The name of the event (e.g AppSec Days Summer of Security 2020) |
| dates | The dates of the full event |
| training | The dates of training portion (e.g. June 23-24, July 28-29, August 25-26) |
| conference | The dates of the conference portion |
| registration_url | Link for the Join Us button to the registration page for this event (almost always /register/) |
| venue | The venue for this event (e.g. Your Computer) |
| location | Leave empty or provide more information regarding Venue location |
| background | File used as the background image in the header |
| color | Accent color used for bars on secondary pages like Sponsors or Schedule |
| analytics | Google Analytics tracking tag (needs to be generated for each event) |
| registration_open | Can be set to true or false.  If false, the registration page tells the user to come back later |
| pitch | This is the event 'description' which displays in the body on the main page (may contain markdown) |

#### Body

The body section contains the venue and pitch from the event-details.yml file mentioned above.  It may also contain other text as added to the index.md file in the root folder of the repository.  In addition, the body section displays the pricing as determined by the pricing.yml file which is located in the _data folder.

The pricing.yml file is a data file that contains pricing details for each 'ticket' type sold. To understand the pricing file structure, see the following image and explanation of the data:

![Event Site Pricing Image](/www-policy/assets/images/event_site_setup_pricing.png)

This image is produced by the following data in the pricing.yml file:

```
- title: Full Conference
  price: TBD
  info: '*See pricing*'
  items: 
    - title: Early Bird
      price: TBD
      info: '*Contact Bob*'
- title: Member Conference
  price: TBD
  items:
    - title: Member Early Bird
      price: TBD
      info:
```

| Section | Description |
| -----: | --- |
| title | The name of this ticket section or ticket type |
| price | The price of this ticket |
| info | An optional line of text explaining this ticket |
| items | Indicates that this ticket type contains sub ticket types<br>Each item should contain title and price, like above <br> There can be multiple sub tickets under items |

The body section also contains the Keynote Speakers section which was not in the above picture (the event shown has no keynote speakers).  The keynote speakers sections looke like the following:

![Eent Site Keynotes Image](/www-policy/assets/images/event_site_setup_keynotes.png)

This section is controlled by the keynotespeakers.yml file located in the _data folder.  The keynotespeakers.yml file expects the following fields for each speaker:

| Section | Description |
| ---: | --- |
| image | The image for the speaker |
| name | Name of the speaker |
| title | The title of the speaker, if any |
| bio | The biographical information for the speaker, usually contained within double quotes |
| subject | The title of the talk being presented |
| abstract | Abstract of the talk, usually contained within double quotes |
| style | Optional item that alters the appearance of the keynote speakers image |


#### Footer
Everything in the footer section comes from the sponsors.yml file in the _data folder.  A typical sponsors.yml file contains the following fields:

| Section | Description |
| ---: | --- |
| logo | The path to the sponsor logo |
| name | The name of the sponsor |
| url | The url of the sponsor |

