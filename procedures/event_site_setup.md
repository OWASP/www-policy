---

title: Setting Up Events
layout: col-sidebar

---

v 2020.12.09

### Github Repository 

*Not a github admin?  Quick jump to [Configuring the Event](#configureevent)*

For OWASP Foundation Global or similar events, the repository should be created by someone with Github Administrator privileges following the standard event repository naming convention: www-event-YYYY-EVENTNAME, where YYYY is the 4 digit year and EVENTNAME is the name of the event.  For instance, an event named Yolo which is in 2021 would have a repository named www-event-2021-yolo.  In the case where multiple events of the same name occur in the same year, the pattern for the repository name should be www-event-YYYY-MM-EVENTNAME, where MM is the 2 digit month of the event. In addition, the repository should be created from the www-event-example template (see steps below).  The following is a general guideline for event repository creation:

1. On the main [OWASP Github Page](https://github.com/owasp/), Click New
   ![New Repository Image]({{site.base_url}}/assets/images/event_site_setup_new_repo.png)
2. On the next page, click the Repository template dropdown and select OWASP/www-event-example
   ![Choose Template Image]({{site.base_url}}/assets/images/event_site_setup_template.png)
3. Type in a Respository name following the aforementioned conventions, choose the Public option, and click Create repository
   ![Name and Create Image]({{site.base_url}}/assets/images/event_site_setup_name_create.png)

The repository will be created after a minute or two.  At this stage, the repository is not yet accessible as a website (this is covered in [Publish the Event](#publishevent), below) 

<a href='' id='configureevent'>

### Configuring the Event

In order to configure the event, it is necessary to be familiar with the general layout of the event site. Note the sections on the following image:

![Event Site Image]({{site.base_url}}/assets/images/event_site_setup_layout.png)

The event site will be populated with certain files and folders. We will cover the more commonly edited files when setting up an event site. First, however, note that the repository has the following layout:

![Event Site Structure Image]({{site.base_url}}/assets/images/event_site_setup_structure.png)

The following files and folders are commonly used for events. This is by no means a comprehensive list and events may have more or less in their respositories.

| File or Folder | Description |
| -----: | --- |
| index.md | Controls what is displayed in the body of the main page |
| _data | Contains data files that control most aspects of the site |
| _data\countries.json | Used on the registration form to display countries in dropdown |
| _data\event-details.yml | Controls site details about the event |
| _data\keynotespeakers.yml | Information about event keynote speakers |
| _data\menu.yml | Controls the top navigation menu for the site |
| _data\pricing.yml | Controls the prices displayed on the site |
| _data\products.json | Created through automation - do not modify |
| _data\sponsors.yml | Controls which sponsors are displayed for the event |
| _data\team.yml | Contains the information for the event team |
| _data\trainings.yml | Contains training information for the event |
| _includes | Folder with files used to control site UX |
| _layouts | Folder containing files that control site UX |
| _layouts\register.html | Created through automation - do not modify |
| about | Folder containing various pages for the site |
| about\code-of-conduct.md | Contains the Code of Conduct |
| about\diversity-statement.md | The statement of diversity |
| about\team.md | Displays information about the event team<br>Controlled by the _data\team.yml file |
| assets | Folder containing assets in use by the site pages |
| assets\images | Folder containing image assets |
| assets\images\keynotes | Folder containing keynote speaker images |
| assets\images\sponsors | Folder containing sponsor logos not found on owasp.org site |
| pages | Folder containing other site pages |
| pages\register.md | Created through automation - do not modify |
| pages\registration-error.md | Shows error if registration unsuccessful |
| pages\registration-success.md | Shows successful registration message |
| pages\schedule.md | Displays the conference schedule |
| pages\sponsors.md | Displays information about event sponsorship |

#### Header

Note that the header section, above, contains the menu, the Join Us button, the event title, where it is located, the dates, and the background image.  Nearly everything in this section can be modified by modifying the event-details.yml file which is located in the _data folder in the repository:

![Event Site Data Files Image]({{site.base_url}}/assets/images/event_site_setup_data_files.png)

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

The menu.yml file controls the navigation options in the header.  That file has the following structure:

| Section | Description |
| -----: | --- |
| title | The name of the menu item |
| url | An optional url to link the title to |
| items | A set of the sub-items for the parent menu item<br>There can be multiple title/url sub items for each parent |


#### Body

The body section contains the venue and pitch from the event-details.yml file mentioned above.  It may also contain other text as added to the index.md file in the root folder of the repository.  In addition, the body section displays the pricing as determined by the pricing.yml file which is located in the _data folder.

The pricing.yml file is a data file that contains pricing details for each 'ticket' type sold. To understand the pricing file structure, see the following image and explanation of the data:

![Event Site Pricing Image]({{site.base_url}}/assets/images/event_site_setup_pricing.png)

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

![Event Site Keynotes Image]({{site.base_url}}/assets/images/event_site_setup_keynotes.png)

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

<a href='' id='publishevent'>

### Publishing the Event

Once the site has basic information and is set up to your satisfaction, it is time to make the site available over HTTPS.  In order to do that, you must go to the repository in GitHub and select the Settings tab.

![Event Site Settings Image]({{site.base_url}}/assets/images/event_site_setup_settings.png)

On the settings page, scroll down to the GitHub Pages section and change Source from None to Branch: master and leave the folder as / (root) then click Save.

![Event Site GitHub Pages Source Image]({{site.base_url}}/assets/images/event_site_setup_source.png)

At this point, your site is available as a page under the owasp.org site but the links will not work.  To get the links to work, you need to set up the Custom domain below where we just set up the GitHub Pages Source.  In addition, you will need to have already had configured a domain to point this repository at (DNS setup is outside this scope, please ask your I.T. admin to set this up).

Under Custom domain type in your domain for this event WITHOUT the leading https://.  For instance, if your event website was meant to be https://mybigvent.owasp.org, you would type in mybigevent.owasp.org and then click Save.  You can now test your site and verify your configuration by going to the website