---

title: Refunding Membership
layout: col-sidebar

---

v2021.4.5 

In order to properly refund a membership, it is necessary to not only refund the customer but also update existing data in Stripe, Copper, and Mailchimp

### Stripe

1. Log into [Stripe](https://www.stripe.com/)
2. Search for the user by email address of the membership on file (this may or may not be their @owasp.org email address)
3. Click on the Customer 
4. Under **Payments** click the payment for which you wish to issue a refund
5. On the Payment screen, upper right, click Refund
6. Follow the prompts to issue a refund for the payment
7. After Performing the steps under the [Copper](#copper) section, update the Customer membership metadata as follows:
    1. Update the Membership Type according to the Membership Type from the Opportunity noted in the [Copper](#copper) section
    2. Update the Membership Start to the Close Date from the Opportunity noted in the [Copper](#copper) section
    3. Update the Membership End to the End Date from the Opportunity noted in the [Copper](#copper) section


### Copper

1. Log into [Copper](https://www.copper.com/)
2. Search, using the top search bar, for the member by the email address of the membership on file (this may or may not be their @owasp.org email address)
3. Click the People object representing the member
4. On the right panel under Opportunities should be listed Memberships including the one you just refunded
5. Click once on the opportunity name of the refunded membership
6. In the details panel that pops out, edit the following details:
    1. Change Status to Lost and give the reason as Requested Refund
    2. Change Stage to Refunded
7. Note whether or not the person has an existing membership opportunity and click it, looking for the following details:
    1. Note the Close Date (which is usually the membership start date but can sometimes be the date of import into Copper)
    2. Note the End Date (which should be the membership end date)
    3. Note the Membership Type indicated by the Opportunity name (One Year, Two Year, Lifetime, or Complimentary)
8. Under the Membership section of the People object for the member, change the following:
    1. Update the Membership Type according to the Membership Type from the Opportunity noted above
    2. Update the Membership Start to the Close Date from the Opportunity mentioned above
    3. Update the Membership End to the End Date from the Opportunity mentioned above
9. If not already done, return to [Stripe](#stripe) section and complete step 7.


### Mailchimp

1. Log into [Mailchimp](https://www.mailchimp.com/)
2. Go to the Audience tab (currently located on the left tool bar)
3. Choose the OWASP-main audience from the **Current audience** drop down
4. Click **View Contacts**
5. Click the hourglass Search icon above the contacts list
6. Search for the user using the email address of the membership on file (this may or may not be their @owasp.org email address)
7. Edit the Profile Information and update membership details to match either the previous Membership (from Copper, above), if existing, or to remove the fields

