When opening or modifying a defect's state be sure that the **Responsible Organization** field is updated to reflect correct organization, your options are **Galileo Dev, Galileo QA, IDEV or UX-User Experience**

 

**State**

 

 

**From**

**To**

**Resolution State**

**Process**

 &lt;Does Not Exist&gt;

 New

 

Defect is opened and assigned it to the appropriate lead.  The responsible organization should be set.

 New

 Work In Progress

 

The lead assigns the defect out to the appropriate resource using the "Owned By" field.  The assigned resource changes the state of the defect to "Work In Progress" when they start to investigate the defect

 Work In Progress

 Waiting on Dev

 

State is for Dev assigned defects.  “Waiting on Dev” state has multiple descriptions including but limited to the following:

The developer delivers defect fix; they then mark the defect as Waiting on Dev and use the defect Approval tab to define a development resource to review the code change.  Once the code change has been reviewed the approving developer will need to change the Approval State to either Approved or Rejected.

The developer has determined that the fix is dependent on an external product or team and defect is waiting on that development team.  Defect description needs to be updated to give team detailed information on blocking issue.

 Work In Progress

 Resolved

 

The assigned resource delivers the fix and then marks the defect as Resolved/Fixed, updates the defect with a brief explanation of the fix, assigns the defect back to the "Created By" resource and sets the responsible organization to the appropriate value.

 Work In Progress

 Returned

 Need More Info

The assigned resource cannot reproduce the defect, so they update the defect with comments asking for clarification, reassigns the defect back to the "Created By" resource, sets the responsible organization to the appropriate value and sets the status of the defect to Returned and the Resolution state to Need More Info.

 Work In Progress

 Returned

 Won't Fix

The Project Team has agreed to not fix/alter the behavior identified by the defect.  The assigned resource sets the status of the defect to Returned and the Resolution state to Won't Fix, updates the defect with a brief explanation of why it will not be fixed, assigns the defect back to the "Created By" resource and sets the responsible organization to the appropriate value. Defect will be considered a "rationalized" defect and will closed by the originator.

 Work In Progress

 Returned

 Works As Designed

The behavior identified by the defect is correct, so the assigned resource sets the status of the defect to Returned and the Resolution state to Works as Designed, provides a brief explanation of why the behavior is Working As Designed, reassigns the defect back to the "Created By" resource and sets the responsible organization to the appropriate value.

 Work In Progress

 Returned

 Duplicate

Another defect that tracks the **exact same** issue is already open and has not been delivered. Assigned resource sets the status of the defect to Returned and the Resolution state to Duplicate, updates the defect with a duplicate defect number, assigns the defect back to the "Created By" resource and sets the responsible organization to the appropriate value

 Waiting on Dev

 Resolved

 

State is for Dev assigned defects.  The code change to fix the defect has been reviewed and approved, the defect "Owned By" developer then marks the defect as Resolved/Fixed.

 Returned

 Closed

 Works As Designed

If "Created By" resources agrees with explanation that a defect is "Works As Designed", they will close it out.

 Returned

 Open

 

"Created By" resources can either: reproduce the defect, provide clarification on how to produce the defect, or rationalize why the defect needs to be addressed.  The appropriate comments should be made in the defect and the resource who had worked on the defect should be reassigned as the owner using the "Owned By" field.  The defect should be reopened to be re-addressed by that appropriate responsible organization.

 Resolved

 Released To QA

 

**After** QA deploys a build into their environment, the QA defects in the resolved state are updated by the QA lead to have their status be "Released to QA", so testers know to validate the fix.  QA will be responsible for flipping the state from Resolved to Released to QA

 Resolved

 Released To Dev

 

Defects opened by development need to be validated and closed by development in most cases.  QA does monitor this queue and if it is determined that QA should validate a development defect then they will change the state to "Release to QA". 

 Released to Dev

 Verified

 

 After a developer has verified a defect that's been released to them, they will change the state to "Verified"

 Verified

 Closed

 

 After a defect opened by a developer has been marked as "Verified", it should then be moved into the state "Closed"

 Released to QA

 Failed

 

QA still sees the defect in the latest build and sets the defect status to Failed.  They also put in comments and attach documentation to the defect to further explain the issue and how to reproduce it.  They reassign the defect to the developer who had delivered the fix.  The responsible organization should be set to Galileo Dev.

 Failed

 Open

 

Assigned resource sets the state to "Work in Progress" and begins to investigate the issues.

 Failed

 Released To QA

 

Development is still unable to reproduce the defect in their environment and after further collaboration with QA, concludes the defect is indeed fixed. Development should set the owner of the defect back to the "Created By" resource and set the responsible organization to Galileo QA.

**Note:** Not having access to the same type of environment is not a valid reason
to say cannot reproduce the defect.
