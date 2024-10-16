**Version 2**

This Google Ads script automates the budget adjustment process for active campaigns labeled with "auto-adjust budget." The key features of this script include:

- **Performance monitoring**

It evaluates the average cost per conversion over the last 7 days using the "Conversions by Conversion Time" metric.

- **Dynamic Budget Adjustment**: If the average cost per conversion is below the specified target, the script increases the daily budget :
  
    - 10% Budget Increase: If the average cost per conversion is close to but still under the target, the script will apply a more conservative 10% budget increase to avoid overspending while still capitalizing on good performance.

    -  20% Budget Increase: If the average cost per conversion is significantly lower than the target, indicating strong performance, the script will apply a more aggressive 20% increase to maximize potential gains while the campaign is performing efficiently. by a calculated percentage (e.g., 15%) while ensuring that the new budget does not exceed a predetermined maximum budget limit.

- **Logging**

All budget changes are recorded in a Google Sheet for historical reference, providing transparency and accountability for budget adjustments.

- **Campaign Label update** :

The script updates the campaign label with the date of the last budget change, ensuring that users can track when adjustments were made.
This script is designed to optimize ad performance while maintaining budgetary constraints, ultimately enhancing the effectiveness of advertising campaigns.

**Lines to Customize:**

1. Campaign Names and Budgets: Modify in the campaignBudgets variable (starting at line 20).

2. Target Cost per Conversion: Adjust the targetCostPerConversion on line 27.

3. Google Sheets URL: Replace "PUT_YOUR_GOOGLE_SHEET_URL_HERE" with your actual Google Sheets URL on line 30.

4. Email Alert: Update your email address in the sendAlertEmail function on line 113.

-------------------------------
Version 1 : 
This Google Ads script automates budget management by incrementally increasing the daily budget for selected campaigns over time. It ensures the budget is gradually adjusted every 4 days by 15%, helping to scale ad spend without triggering a new learning phase for the campaign. Additionally, the script allows users to set a maximum target budget for each campaign, ensuring the budget doesn’t exceed the desired limit.

The script also tracks each budget increase using Google Sheets for logging, and labels campaigns with the date of the last budget increase.

Key Benefits:
Automated Budget Scaling: Gradually increases budgets without disrupting campaign performance or triggering new learning phases.
Customizable Target Budgets: Set individual target budgets for each campaign to ensure they do not exceed the specified limit.
Multi-Campaign Management: Manage and adjust budgets for multiple campaigns in a single run.
Logging & Tracking: Records all budget changes in Google Sheets, providing a clear overview of spending adjustments.


Here are the variables 👇 that you can change to adapt the script to your accounts ( once you paste scripts in google ads ):

→ Campaign names and target budgets (starting from line 21)

→ Percentage increase if you want to change from 15% to 20%, for example (line 62)

→ Add the Google Sheets link for your tracking file (line 116)

→ Change from 4 to 5 days, for example (lines 74 & 82)

→ Set the script execution frequency to Daily (in the scripts page)
