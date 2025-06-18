---
title: "Report"
sidebar_position: 6
---

# Building a Report

To build a report, follow these steps:

For more information about reports, you can refer to [Reports](../../../guide/information-structures-concepts/basic-concepts/reports).

## Building the Monthly Performance Report

1. Go to the reports window within the "Support Tickets" entity.

2. Click on the "+" sign.

![Reports Window](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_reports(1).png)

3. The report information page appears.

4. Fill in the report information:

   - Name: "Performance Report".
   - Query: Select the query on which the report is based, "Ticket Classification" which we built earlier.
   - Icon: Choose an appropriate icon for the report, which is "align-right".
   - Fields: Select all the fields we want.

![Select Fields](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_reports(2).png)

5. Enable the "Page Header" button.

6. Enable the "Organization Header" button.

7. Enable the "Report Header" button where two fields appear:

   - Content Type: Select text.
   - Text: Write "Monthly Performance Report".

8. Enable the "Page Footer" button.

9. Enable the "Organization Footer" button.

10. Report layout: Select "Horizontal".

![Report Design](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_reports(3).png)

11. Users: Select employees and the manager.

12. Interval Type: Select "Recurring".

13. Schedule Expression: To send the report two or three days before the end of the month, the expression will be "**28 8 0**".

14. Start Date: Specify the start date.

15. End Date: Specify the end date for the recurrence.

![Report Settings](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_reports(4).png)

16. Channel Type: Select email, which is the current option.

17. Subject: Name it "Performance Report".

18. Report Content: Monthly Performance Report.

19. Source: Select user.

20. Type: Static.

21. Value: "Manager".

![Report Settings](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_reports(5).png)

22. Enable the "Send Report Link" button.

23. Enable the "Send Report as File" button, where a field appears to choose the report type; we will select "pdf".

![Report Settings](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_reports(6).png)

24. Click the "Finish" button to save the report.

![Save Confirmation](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_reports(7).png)

25. Click the "Publish" button to send the report periodically.

26. A popup appears to confirm the publication of the report.

27. Click the "Confirm" button to publish the report.

![Publication Confirmation](../../../../../../../static/img/tutorial/customer-support-system/customer_support_creating_reports(8).png)