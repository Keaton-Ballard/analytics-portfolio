# Keaton Ballard's Portfolio

## [Project 1: Weighted HubSpot Lead Distributor](https://github.com/Keaton-Ballard/keaton__ballard_portfolio/blob/main/weighted-hubspot-lead-distributor)

This project automates the assignment of HubSpot contacts to owners (such as sales reps) using a **weighted random distribution** approach. Reps with more "weight" are more likely to be assigned a new contact.

Since using round-robin logic doesn't work well in HubSpot, this script enables a more customized and stable probability-based assignment strategy.

---

### Features

- Assigns leads based on customizable weight values (probabilities).
- Securely connects to HubSpot using a private app token.
- Updates the contact’s `hubspot_owner_id` field via HubSpot's CRM API.
- Designed to be triggered by HubSpot workflows or run as a standalone script.

---

### How It Works

Each owner is assigned a "weight" value. When a new lead enters the system, the script:
1. Calculates the total weight across all owners.
2. Picks a random number between 0 and total weight.
3. Assigns the lead to the owner whose weight range includes that number.

This makes it easy to adjust how often each owner's distribution weight.




