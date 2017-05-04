#Personnel actions [FAQ]


> Written with [StackEdit](https://stackedit.io/).
> This topic contains answers to questions that you might have if your organization uses personnel actions. Personnel actions are additional steps that you must complete when you perform certain personnel-related tasks. Examples of tasks that might require personnel actions are when you create new positions, modify existing position values, hire new workers, transfer workers, change worker compensation, change position assignments, or terminate workers. 
> 
> >**Note**
> >Personnel actions are available only if Dynamics 365 for Talent is installed and the Personnel actions configuration key is selected. 

##How can I tell if my organization requires personnel actions?
Personnel actions are required by your organization if you are asked to select a personnel action when you create new positions, change existing positions, hire new workers, transfer workers, change worker compensation, change position assignments, terminate workers, or enter leave for workers. 


## What is the difference between a position action and a worker action?

There are two types of personnel actions: 

 - Position action – A position action is performed on existing positions or new positions. For example, a position action might be required if you change a value on an existing position or if you create a new seasonal position. For detailed information about how to use position actions, see Key tasks: Existing worker positions or Key tasks: New worker positions. 

 - Worker action – A worker action is performed on existing employees or new employees. For example, a worker action might be required when a new employee is hired or an existing employee is promoted. For detailed information about how to use worker actions, see Assign personnel actions to workers. 

## What do the stauses of the personnel actions mean?
Personnel actions can have the following statuses: 

 - **Draft** – If workflow is used, the action hasn’t been submitted. If workflow isn’t used, the action hasn’t been completed. 
 -  **In review** – The personnel action has been submitted to workflow, but the workflow is not completed. 
 - **Approved waiting** – The workflow is completed, but the changes are still in process.
 - **Canceled** – The workflow was canceled or the personnel action was recalled.
 - **Rejected** – The action request was rejected by the approver. 
 - **Processing action** – The action request has been approved and the changes are being processed.
 - **Workflow complete** – The workflow is completed and the changes have been processed.
 - **Failed** – The workflow failed because the information is out of date. Click **Reactivate** to display the latest information and continue.
 - **Completed** – The position was successfully created or modified, or the employee was successfully hired, transferred, or terminated, or had their compensation changed. 
 - **Error** – A problem occurred other than information being out of date. Open the **Personnel actions message log** to determine the cause of the error.
 - **Denied** – The action request was denied by the approver. 

## Can I delete a personnel action?
Yes, you can delete personnel actions that have a status of **Draft**, **Error**, **Failed**, or **Canceled**.

## What is the fastest way to check the status of a personnel action request?
Open any of the personnel action list pages and select a personnel action. The **Related information** section in the FactBox displays the number of attachments that are assigned to it. 

## What should I do if a personnel action request fails?
If a personnel action request fails, follow these steps to resolve the error and resubmit the request: 

 1. On the **Action Pane**, click the **Error** text button to view the message
    text that describes the problem.  
    
 2. On the **Action Pane**, click **Reactivate** to load the latest information and set the status of the personnel action back to **Draft**.  
    
 3. Resolve the error, and then click **Complete** or **Submit**.

> **Tip**:
> If you received an error message that says a worker already exists, but you want to add the new worker anyway, you can open the personnel action and clear the **Check for duplicates** box on the **Action** tab to resolve the error. 

## What happens to a personnel action that uses workflow when the final approval is completed? 
If there are no errors, the personnel action becomes read-only. (You can view the history on the **All worker actions** list page, but you can’t change the personnel action.) When the status of a personnel action is **Completed**, the position or worker record has already been updated. To view the changes that were performed, open the **Positions** or **Workers** list page.

>**Tip**:
>If you find that you're clearing this field too often, you can ask your system administrator to remove the association on the **Personnel action types** page. Alternatively, the system administrator can create a new personnel action type that has the **Fixed compensation action** field cleared on the **Personnel action types** page. 

##Why do I receive the following error when I enter a non-zero value in the Pay rate field? "The value is out of its valid range – it much be between 0.00 and 0.00" 
You receive this message because the Level field in the Job form is blank for the job that is associated with the selected position. 

To resolve this error, follow these steps: 

 1. On the **Worker position assignments** tab, right-click in the **Position** field and select **View details**. 
 2. Click the **Job** field value (the link) to open the **Job** page. 
 3. On the **Action pane**, click **Edit**.
 4. Click the **Compensation** tab. 
 5. In the **Level** field, select a level. 
 6. Close the **Job** page. 
 7. Close the **Position** page. 
 8. Return to the **Compensation** tab on the **Worker** page, select a value in the **Plan** field, and then enter the employee's compensation in the **Pay rate** field. 

## Why can't I change the effective date in the header of the Worker action form?
You can't change the effective date because the field is populated with the most logical date for the action type.

For example: 

 - The effective date in the header of a **Terminate a worker** action is the date you entered in the **Termination date** field. 
 - The effective date of a **Hire a worker** action is the date that you entered in the **Employment start date** field. 
 - The effective date of a **Transfer a worker** action is the date that you entered in the Assignment start date/time field for the worker. 

   
  