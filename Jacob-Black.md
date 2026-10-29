Test ID: JB-01 Written by: Jacob Black Title: System does not reject username that is less than 8 characters 
Traces to: REQ-01 (A user can register with a unique username and a password of at least 8 characters.) 
Test type: Negative 
Preconditions: Logged out. On the log in/register page.
Test data:

Name: five (4 characters)
Password: 12345

Type the test data username into the username field
Type the test data password into the password field
Click Register
Expected result: An error message appears telling the user to submit a username with at least 8 characters. The account is not registered.
Actual result: Success message appeared. User is able to log in with that username and password. 
Status: Fail 
Severity: Minor
V or V: Verification

-

Test ID: JB-02 Written by: Jacob Black Title: System allows user to vote even when not logged in. 
Traces to: REQ-02 (A user can log in with their username and password. Only logged-in users can submit costumes or vote.) 
Test type: Security 
Preconditions: Logged out. On the vote page.
Test data:

Click Vote on any costume
Expected result: An error message appears telling the user to log in. The vote is not counted.
Actual result: Success message appeared. User is able to vote on any costume as long as they do not run out of votes
Status: Fail 
Severity: Major
V or V: Verification
