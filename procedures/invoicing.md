---

title: Invoice Process
layout: col-sidebar

---
v2020-12-09

## Creating Invoice

1. Opportunity in Copper is moved by staff from “60-Contact-Sent” to “75-Contract-Signed” stage
2. Automation in Copper creates:
  - Collect Corporate Assets via https://owasp.wufoo.com/forms/corporate-supporter-assets/
  - Post Corporate Assets on Event/Main website as appropriate
  - Create invoice in Stripe
3. Create Invoice in Stripe
  - Navigate in Copper to Opportunity
  - Copy the Email address of the Opportinity Primary Contact
  - Login to Stripe
  - Validate or Create Customer in Stripe
    - Search for email address of Opportunity Contact
    - If not found, add Contact into Stripe
      - Name is person’s name
      - Click on Company Name for Billing Details (Address)
    - Use company name in Address Line 1
    - If Billing Details are missing assign task to staff to collect (or review documents in DocuSign section of Opportunity).
    - Select Language (if appropriate)
    - Select Currency of the invoice (not necessarily the country of the company)
    - If there is a VAT number, select the correct VAT type for Tax ID and put the number in the value box.
    - Add Customer
4. Navigate in Stripe to Customers > Invoices
5. Select NEW Invoice
  - Enter Customer Email
  - Enter Item as {item - detail} as in “Event Sponsorship - 2020 Summer of Security” or “Corporate Membership - Annual”
  - Use Memo field for Corporate Memberships ONLY and include:

```
Summary of OWASP Corporate Membership Benefits:

- Listing in rotation as Corporate Supporter site-wide on https://owasp.org/
- Up to $2,500 of your Fee can be applied to Corporate Sponsorship https://owasp.org/pages/corporate-sponsorships
- Public acknowledgment on various other channels.
```

6. Send Invoice
  - Validate customer email address
  - CC accounting@owasp.com, kelly.santalucia@owasp.com
  - Press Send Invoice
7. Update Copper
  - From Stripe Copy 12 digit Invoice number
  - Return to Copper and the Opportunity
  - Paste Invoice number into “Invoice number” field
  - Change “Invoice Date” to “today”
  - Change opportunity stage from “75-Contract-Signed” to “90-Invoice-Sent”
8. Close Task as done
9. Virtual accounting will enter invoice received via email to QuickBooks
10. Customer can pay via CC or wire transfer directly to Stripe
10. Virtual accounting will mark invoice paid once payment recieved via Stripe
11. At anytime staff/Virtual can [check Stripe for status of open invoices](https://dashboard.stripe.com/invoices?closed=false&status=open)

## Changing Invoice

Stripe does not allow invoices which have been finalized/sent to be changed. Not the amount, not the date, not the items. This seems to make a good deal of sense for auditing purposes. If an invoice was sent in error, or it contains errors you must:

1. VOID the invoice in Stripe and include a reason in the note field
2. Download a PDF of the VOIDED invoice 
3. Email the PDF to accounting@owasp.com, kelly.santalucia@owasp.com
4. Create a new invoice with the process above

## Payment made to the Wrong Invoice

1. Create a note on the paid invoice of overpayment and which invoice overage will be apply to.
2. Open the invoice to which the payment was to be made and issue a CREDIT NOTE
3. Include the paid invoice reference number
2. Download a PDF of the paid invoice 
3. Email the PDF to accounting@owasp.com, kelly.santalucia@owasp.com
