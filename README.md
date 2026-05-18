This workflow collects customer feedback through a form, rewards positive feedback with discount eligibility, and logs all responses to Google Sheets.

<img width="1403" height="721" alt="Workflow Image" src="https://github.com/user-attachments/assets/3c31747b-4d1e-4963-9f46-5a04635ad950" />


How it works:

Form Trigger - Presents a feedback form collecting:

Email ID (required)
Name (required)
Age (required)
Feedback dropdown: Positive, Neutral, or Negative
Conditional Check - The IF node evaluates whether feedback equals "Positive"

Discount Assignment - Two branches:

True branch (Positive): Adds Discount: "Yes" field
False branch (Neutral/Negative): Adds Discount: "No" field
Merge - Combines both branches back into a single flow using append mode

Google Sheets Logger - Appends every submission as a new row with all fields including the discount status

Key benefits:

Automated incentive system for positive feedback
Complete audit trail of all customer responses
Preserves all original form data throughout the workflow
Handles all feedback types uniformly after discount assignment
