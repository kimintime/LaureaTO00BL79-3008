
## Summary (Summarize the bug encountered concisely)
The New Project page https://gitlab.com/projects/new#blank_project contains a typo, inviting the user to `Create a black project` instead of `Create a blank project`.

## Steps to reproduce     
Follow procedures to `Create blank project` as per TS-3 Project.
Note the typo on the `NewProjectsUrl` page.

## What is the current bug behavior?
The bug is a typo, asking the user to create a black project.

## What is the expected correct behavior?
The user is expected to create a blank project.
     
## Relevant logs and/or screenshots
![Create black project](../Image/Bug_Project_create_blank.png)

Should be

![Create blank project](../Image/Bug_Screenshot.png)

## Possible fixes
The fix is just a simple spelling correction, of changing black to blank.

## Whom do you report/ Assign To/ Tags
/label ~bug ~needs-investigation /cc @project-manager /assign @qa-tester


## Priority
Suggestion, as it is not a coding error, or any logic issue, but it does need an adjustment.


      
