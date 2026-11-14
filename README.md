# Brightpath Lead Management

## Keep new enquiries organised and make it easier to follow up.

When a business gets enquiries from potential customers, someone has to collect the details, work out which ones deserve attention first, and make sure nobody gets forgotten.

That can become difficult when enquiries keep coming in and the team is busy serving existing customers.

Brightpath is a portfolio project built around that everyday problem. It brings lead intake, prioritisation, follow-up, and a daily lead report into one process.

## What it does

There are two connected parts to this project.

### 1. New enquiry handling

When someone submits the enquiry form, the workflow:

- Collects their contact details and what they are looking for.
- Looks at the budget and how soon they want to get started.
- Gives the enquiry a score and marks it Hot, Warm, or Cold.
- Saves the details in a lead tracking sheet.
- Prepares a more personal follow-up for high-priority enquiries.
- Checks the message before sending it. If it does not pass the checks, it is held for a person to review.

The idea is simple: your team should not have to treat every enquiry as if it has the same level of urgency.

### 2. Daily lead summary

The second workflow runs every morning at 8:00. It checks the lead sheet and looks at enquiries received in the previous 24 hours.

It then puts together a report showing:

- How many new enquiries came in.
- How many were marked Hot, Warm, and Cold.
- The details of each lead, including the company, budget, service interest, urgency, and score.

The report is sent by email, so the business owner or sales team can see what came in without going through every row in the sheet.

## Why this is useful

A new enquiry is only useful if someone notices it and follows up.

This setup gives a business a clearer way to see which prospects may need attention, keep their details in one place, and start each day with a quick picture of recent enquiries.

It does not make sales decisions for your team. It helps your team see what is happening and decide what to do next.

## Screenshots

These spaces are here for screenshots from the actual project. The notes explain exactly what to capture.

### 1. New enquiry workflow

<!-- Add screenshot: images/01-enquiry-workflow.png -->
![New enquiry workflow](images/01-enquiry-workflow.png)

*Capture the full first workflow on the n8n canvas. Zoom out enough to show the form, lead scoring, Google Sheets, follow-up message, and review steps. Keep the node labels readable.*

### 2. Daily summary workflow

<!-- Add screenshot: images/02-daily-summary-workflow.png -->
![Daily summary workflow](images/02-daily-summary-workflow.png)

*Open the Brightpath Daily Lead Summary workflow in n8n. Capture the full canvas showing the schedule, Google Sheets lookup, 24-hour filter, summary creation, and email step.*

### 3. Enquiry form

<!-- Add screenshot: images/03-enquiry-form.png -->
![Enquiry form](images/03-enquiry-form.png)

*Open the form preview for the first workflow. Capture the blank form with the questions a potential customer answers, including their contact details, service interest, budget, urgency, and project description.*

### 4. Lead tracking sheet

<!-- Add screenshot: images/04-lead-tracking-sheet.png -->
![Lead tracking sheet](images/04-lead-tracking-sheet.png)

*Open the Google Sheet used by the workflows. Capture the column headings and a few sample rows so someone can see how enquiries, scores, and categories are recorded. Use made-up sample details only.*

### 5. Follow-up email

<!-- Add screenshot: images/05-follow-up-email.png -->
![Follow-up email](images/05-follow-up-email.png)

*Capture an example of the follow-up prepared for a Hot lead. Use a fictional prospect and hide all private inbox details. Show the message itself, not your account settings.*

### 6. Daily summary email

<!-- Add screenshot: images/06-daily-summary-email.png -->
![Daily summary email](images/06-daily-summary-email.png)

*Capture the daily report email showing the total number of leads and the Hot, Warm, and Cold sections. Use fictional sample data and hide the recipient address and any private information.*

## Tools used

- n8n
- Google Sheets
- Google Gemini
- Gmail

## Project notes

This is a portfolio demonstration based on a business scenario. It is not presented as a live client deployment, and no client results are being claimed.

Both workflow exports are included in this repository. They are intentionally inactive. The public copies have been cleaned of credential references and private account details. The spreadsheet ID and email recipient are placeholders, so the workflows need to be connected to the business's own accounts and tested before use.

The daily report is scheduled for 8:00 according to the timezone configured in the n8n environment. It uses a rolling 24-hour window, not a calendar-day report.

## Files in this repository

- `brightpath-lead-intake-scoring.json`: collects and prioritises new enquiries, records them, and prepares a follow-up.
- `brightpath-daily-lead-summary.json`: checks the previous 24 hours of enquiries and emails a daily report.

## Need a better way to handle incoming enquiries?

If enquiries are coming in but your team is finding it hard to keep track of them, decide who to contact first, or follow up consistently, I can help you map out a process that fits your business.

The first thing I would want to understand is how enquiries reach you today and where they tend to get missed.
