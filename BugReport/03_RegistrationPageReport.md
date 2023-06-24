
## Summary
At user registration, the RegistrationUrl should redirect to a page asking the user to submit a code sent to email.
If the user clicks the back button to go back to RegistrationUrl and changes the email address and re-submits, it skips the security verifcation page entirely, with an error notifcation, "That was a bit too quick! Please resubmit." At this point, login with those credentials will fail as expected.

## Steps to reproduce     
Follow procedures for Register user with valid credentials per TS-2 Registration
Navigate back to the RegistrationUrl after submitting registration
Change email address to another valid Email
Resubmit registration form

## What is the current bug behavior?
The error notifcation is unclear. The user lands on the login page and skips the security verifcation page. The user might attempt this is if they change their mind about the email address. 

## What is the expected correct behavior?
The user should not see a login page where it appears to have been successful, with an error saying they have to 'resubmit.' The error is ambiguous.
     
## Relevant logs and/or screenshots
![Error message](<Screenshot 2023-06-24 at 13.56.08.png>)


## Possible fixes
Either adjust the routing to allow navigation back to the security verification page, to end on an error page stating that registration was not successful, or a less ambiguous error message, for example, "User registration failed, please try again." 

## Whom do you report/ Assign To/ Tags
/label ~bug ~needs-investigation /cc @project-manager /assign @qa-tester


## Priority
Suggestion


      
