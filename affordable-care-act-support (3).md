Generate reports to comply with the Affordable Care Act 
===================


Functionality is available to assist employers that need to track the information reported on form 1095-C in support of the **Employer Mandate** portion of the Affordable Care Act.  Note this functionality is only enabled for legal entities in the US. 

##Getting started
When beginning to track information to report on form 1095-C, you must first create one or more Affordable Care coverage groups. These Affordable Care coverage groups will be used to indicate the offer of coverage that was provided to an employee, the employee's share of the lowest cost monthly premium (if the cost is above the federal poverty line) as well as Safe Harbor used by the employer, if applicable. Using Affordable Care Act groups enables you to manage the information for these fields without needing to touch every employee record where the conditions are the same. In addition, Affordable Care coverage groups can easily be assigned to one or more employees using the Mass assign functionality on the page.

##Maintaining multiple versions of a coverage group
You can maintain multiple versions of any coverage group, which allows you make changes that keep the group’s information current, without having to create a new group and reassign employees to it when something changes in your organization or in the benefits that are offered. Using an example in the preceding illustration, if the employee share of the lowest-cost monthly premium was changing in 2016 a new version could be created for the MEC w/W2 group with a Group valid from date of 2016 and the new cost could be entered.

After you’ve created the Affordable Care coverage groups that you need, you can choose to Mass assign the groups to employees using the Mass assignment functionality on the page, or you can go to each employee and indicate whether ACA information needs to tracked and reported for that employee as well as assigning the employee to an Affordable Care coverage group.

If Affordable Care coverage information doesn't need to be tracked or reported for an employee, for example if they are a part-time employee, the Report coverage field could be set to No. This example shows the need to capture and report whether or not coverage was offered to Alan Steiner; he has been assigned to the MEC < FPL Affordable Care coverage group. Although each employee for which ACA information needs to be tracked needs to be assigned to an Affordable Care coverage group, you can still change the Offer of coverage, Employee share of cost and Safe Harbor options for any month – or months – that may need different values than those entered in the Affordable Care coverage group.

To enter exceptions to any of the Affordable Care coverage group values, click on the Affordable Care Coverage link found on the Worker detail page, which is under the Additional information section on the Employment tab.

##Reporting health care coverage
In addition to tracking what if any health insurance coverage was offered to a full-time employee, if the employer offers employer-sponsored self-insured health coverage for which the employee is enrolled (regardless of whether their employment status is full-time or part-time), additional information needs to be reported on the 1095-C. Each employee (including dependents) covered by the employer-sponsored benefit plans needs to be included on the report for the months they were covered. To assist with tracking this information some additional enhancements have been made to the Benefit plans and dependent coverage offerings in Dynamics AX 2012.

You can indicate whether or not each Benefit plan must be reported by selecting the ACA reportable check box.
 
In addition, if employees have chosen to have any of their dependents covered under a benefit you can indicate the dates the dependent was covered for each employee on the Maintain benefits page.   To indicate that the dependent is covered under the benefit, choose the Edit button in the action pane of the Dependents FastTab.

In the Dependent coverage date manager window you can indicate the dates the dependent was covered by the benefit. Entering dates in this window will automatically select the Covered checkbox in the Maintain benefits window.

##Viewing information
You can use the Worker Affordable Care coverage page to see which employees have been assigned to each coverage group, which employees don’t need to be included on a report, and which employees are unassigned.

If any of the default values from the Affordable Care coverage group have been overridden an asterisk will appear next to the value that was changed.   If the values for all 12 months are the same and haven't been overridden, the value will print in the All 12 months column.

You can also use the inquiry window to understand which employees have been flagged as not ACA reportable, meaning you don't need to track whether coverage was offered to them and will not need to issue a 1095-C to them at the end of the year. By selecting Not ACA reportable in the Filter by, you can generate a list of all employees that have been flagged to not receive a 1095-C.

In addition to viewing a list of employees that are not ACA reportable, you can also view any employees who are unassigned (the ACA Report coverage field is empty) or that have been assigned to an Affordable Care coverage group that is expired for the year selected in the Year field.

You can export lists of employees that were generated using any of the filtering options to Excel.

If you need to report covered individuals because as an employer you provide self-insured coverage you can also view any dependents covered under benefit plans that have been marked as ACA reportable by selecting the View Dependent coverage action on the action pane strip.

*Note: Only benefits whose plan has been marked as ACA reportable will display in the inquiry window.