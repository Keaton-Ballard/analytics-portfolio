# Welcome to My Portfolio!

I'm Keaton Ballard, a data analyst interested in automation, business operations, and data-driven decision-making. This portfolio highlights my experience working with real-world CRM workflows. The first section showcases Python scripts I built to optimize processes within HubSpot. The second section features scripts I used during my Data Analytics Master's program. 

### HubSpot Custom Code Projects 

(HubSpot scripts require a private app with the correct scopes and API key.) 

## [Project 1: Weighted HubSpot Lead Distributor](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/weighted-hubspot-lead-distributor)


This script automates the assignment of HubSpot contacts to owners (such as sales reps) using a **weighted random distribution** approach. Reps with more "weight" are more likely to be assigned a new contact.
Since using round-robin logic doesn't work well in HubSpot, this script enables a more customized and stable probability-based assignment strategy that efficiently distributes leads to reps with a simple syntax that simplifies changing the distribution weights.


---

## [Project 2: HubSpot Record Meeting Associatior](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/hubspot-meeting-deal-associator)


Our sales process in HubSpot creates deal records after a contact book a meeting, which makes the meeting information only present in the contact record and not the deal record. This script corrects this error by automatically associating the most recently booked meeting with the most recent deal tied to a contact in HubSpot. Ensuring the sales reps have all the correct meeting and sales information in one place before they meet with their clients.


---

## [Project 3: HubSpot Phone Number Formatter](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/hubspot-phone-number-formatter)


This script automates the formatting of U.S. phone numbers for contacts in HubSpot. It standardizes phone numbers into the format `(XXX) XXX-XXXX` using a Python script that I deploy in a HubSpot *custom code action* in workflow, ensuring that all phone numbers in our CRM will have the same format. It also includes built-in error handling, API rate limit retries, and permission checks to ensure it stays within HubSpot's API limits.

---

## [Project 4: Hubspot Smart Record Merger](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/hubspot-smart-record-merger)


The purpose of this script is to automatically detect and merge a specialized group of duplicate HubSpot contacts. I created this automation due to a steady amount of contacts using one email on the ad form and a separate email on the meeting book form. HubSpot's merging system is currently manual. It first attempts to identify duplicates using the contact's phone number. It returns to searching by exact first and last name if no matches are found. The goal is to ensure that the correct records are being merged within the CRM.

<!-- force update -->
