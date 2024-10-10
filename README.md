This Google Ads script automates budget management by incrementally increasing the daily budget for selected campaigns over time. It ensures the budget is gradually adjusted every 4 days by 15%, helping to scale ad spend without triggering a new learning phase for the campaign. Additionally, the script allows users to set a maximum target budget for each campaign, ensuring the budget doesn’t exceed the desired limit.

The script also tracks each budget increase using Google Sheets for logging, and labels campaigns with the date of the last budget increase.

Key Benefits:
Automated Budget Scaling: Gradually increases budgets without disrupting campaign performance or triggering new learning phases.
Customizable Target Budgets: Set individual target budgets for each campaign to ensure they do not exceed the specified limit.
Multi-Campaign Management: Manage and adjust budgets for multiple campaigns in a single run.
Logging & Tracking: Records all budget changes in Google Sheets, providing a clear overview of spending adjustments.


Here are the variables 👇 that you can change to adapt the script to your accounts:

→ Campaign names and target budgets (starting from line 21)

→ Percentage increase if you want to change from 15% to 20%, for example (line 62)

→ Add the Google Sheets link for your tracking file (line 116)

→ Change from 4 to 5 days, for example (lines 74 & 82)

→ Set the script execution frequency to Daily (in the scripts page)
