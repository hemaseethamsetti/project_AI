# Authentication Service #
Project Code: AIOO1

Authentication Service is part of AI health Advisor. 
## Use Cases ##

### Use Case Diagram ###
![image](https://github.com/hemaseethamsetti/project_AI/assets/147400262/e1b945c5-fe4f-4feb-9f99-bcd348cf2ff2)






## User Stories ##
### AI001-001: Chat with AI ###
* Actor: Non Registered user
* Pre Condition: 

1. User should have a working email-id which is not already registered with  AI health Advisor website.

* Input:

1.  None

* Sequence:

1. User opens the website  and AI automatically greets and asks user to tell one specific health problem they have.
2. user can enter their questions in chat interface.
3. AI responds and chat continues.

* post condition: 

1.Page displays a message "Create an account to save coversation".

* Exceptions:

1. user can have only limited number of free trails.
2. After the limit has expired user should register.
3. Without registration user is not allowed to continue their chat with AI.

### AI001-002: Create an account ###

* Actor: Non Registered user
* Pre Condition:

1. User should have a working email-id which is not already registered with AI health Advisor website.

* Input:

1. Name of the User.
2. Working email id.
3. Preferred password with 8 characters (alphanumeric with at least one upper case and one lower case letter)

* Sequence:

1. User opens the webpage and click on 'Register'.
2. Registration page appears.
3. User supplies the name, a working email-id and the preferred password.
4. Page displays a message to check e-mail and prompts for activation code.
5. User enters the activation code.
6. Page displays success message and redirects to login page.

* Post Condition:

1. Page displays success message and the login page appears

* Exceptions:

1. Registration page re-appears with appropriate message if user enters invalid name or invalid email-ID or invalid password.
2. Registration page re-appears with appropriate message if the email-ID is already registered with Shopping website.
3. Registration page shows "resend" button, in case the activation code is not entered in the first 5 minutes after the mail has been sent.
4. Registration page will not show any special message if the email-ID is not reachable. It just prompts for activation code, as usual.

### AI001-003: Login with Inactive ID ###

* Actor: User with Inactive Email-ID

* Pre Condition:

1. User should have a registered Email ID and password with  AI health Advisor website.

* Input:

1. Email ID
2. Password

* Sequence:

1. User opens the webpage and click on ‘Login’
2. Login page appears
3. User supplies Email ID and password
4. Page indicates that the Email ID is yet to be activated.
4. Page displays a message to check email and prompt for activation code
5. User enters the activation code
6. Page displays success message and redirects to login page

* Post Condition:

1. Page displays a message ‘successfully activated and the login page appears

* Exceptions:

1. Login page re-appears with appropriate message if user enters invalid Email ID or password.
2. Prompt box re-appears with appropriate message if user enters invalid Activation Code.
3. Login page re-appears with appropriate message if user fails to enter valid Activation Code within 5 minutes.

### AI001-004: Login with Active Email ID ###

* Actor: User with Active Email ID 

* Pre Condition:

1. User should have activated the Email ID

* Input:

1. Email ID. 
2. Password.

* Sequence:
 
1. User opens login web page
2. User supplies his/her Email ID and Password
3. User click on login button
4. User home page appears

* Post Condition:

1. User home page appears with name of the user displayed.

* Exceptions:

1. Login page re-appears with appropriate message if user enters invalid Email ID or password.

### AI001-005 Reset Password ###

* Actor: User with Active Email ID 
 
* Pre Condition:

1. User should have an active Email ID with AI health Advisor website.

* Input:

1. Email ID

* Sequence:

1. User opens login page.
2. User clicks on forgot password button.
3. User enters Email ID
4. Page prompts for new password and clicks on "Reset Password"
4. Page displays a message to check email and prompt for activation code
5. User enters the activation code
6. Page displays success message and redirects to login page

* Post Condition:

1. User should be able to login with new credentials

* Exceptions:

1. Login page re-appears with appropriate message if user enters invalid Email-ID.
2. Prompt box re-appears with appropriate message if user enters invalid activation code.

### AI001-006 New conversation  ###

* Actor: User with Active Email ID

* Pre Condition:

1. User should have logged into  website

* Input:
1. None

* Sequence:

1. User click on "New conversation"
2. website loads the chat interface,displaying a greeting from the AI.
3. The AI prompts the user to enter their specific health problem.
4. The user types their health problem in the chat interface and submits it.
5. The Ai analyzes the question and send back response to the users.

* Post Condition:

1. User should be able to start a new conversation.

* Exceptions:

1. Not applicable.

### AI001-007 Conversations with cody ###

* Actor: User with Active Email ID

* Pre Condition:

1. User should have logged in to working Email ID.

* Input:

1. None


* Sequence: 

1. User clicks on particular question he asked under Conversation with cody during the conversation with ai.
2. page displays the entire chat or history related to that query .

* Post Condition:

1. Users should be able to view their conversations with AI according to the query he/she selected.

* Exceptions:
 
1. Not applicable


### AI001-008 Logout ###

* Actor: User with Active Email ID

* Pre Condition:

1. User should have logged in to working Email ID.

* Input:

1. None


* Sequence:

1. User click on Logout.
2. Page displays a message 'successfully Logout' and the login page appears.

* Post Condition:

1. Login screen appears
2. Back button or bookmarks fail to open any of the login-protected pages of the web app

* Exceptions:

1. Not Applicable


## Workflow ##

### Workflow Diagram ###
![image](https://github.com/hemaseethamsetti/project_AI/assets/147379636/0245f1ff-e6d7-42dd-9bac-6d0696e288d1)



