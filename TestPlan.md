# Test Plan

**Author**: CS 6300Team 02


| Version | Description       |
| --------|:-----------------:|
| V1      | Initial version   |

## 1 Testing Strategy

### 1.1 Overall strategy

Verification activities will be performed to ensure that all requirements are met for the GoBowl Android app. The verification activities that will be performed are unit testing and system testing. The main focus will be on performing acceptance testing. The team will assign two members to develop and execute the corresponding test procedures.

### 1.2 Test Selection

Part of the verification effort will be to use unit tests. The other part of the verification effort will be to do BlackBox testing, taking into account the main features of the GoBowl Android app.

### 1.3 Adequacy Criterion

The quality of test cases will be gauged by code coverage from unit testing and successful acceptance tests.

### 1.4 Bug Tracking

We will be using Github’s integrated issue tracking to track bugs and enhancements. We will consider “bugs” any issues found during our system testing. Enhancement will be defined as features that will enhance the user experience but are not covered in the requirements.

### 1.5 Technology

We’re going to use the JUnit framework and GitHub’s issue tracking to perform and track the verification effort.

## 2 Test Cases

The system test cases below are grouped together in Test Suites corresponding to each main functional feature.

**Test Suite #1: Adding a Customer**

- _Test Case #1: Adding a Customer_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available 2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu on the upper left. | Manager Portal is shown. | Manager menu option is shown  | Pass  |   |   |   |
| Step 3:  Select the Manager Option | The GUI displays all the current customers and a button with _+_ symbol|  The app displayes a list with all current customers and gives the user the option to edit or add a customer| Pass  | 1  |   |  |
| Step 3: Press the _+_ button | The GUI displays the following text fields: _First Name_, _Last Name_ and _Email._ |The text fields are displayed |Pass | 1,3  |   |   |
| Step 4: Complete text fields with appropriate data | Text fields accept the input of the customer without any issues. | The Customer's data can be succesfully entered |Pass | 3  |   |   |
| Step 5: Select the Continue button | Customer should be added to the system and the screen should display the _Customer's name_, _Customer's email_, _Customer's ID_, _Print ID button_, and a _Done button_ | All the expected items are being displayed properly on the screen |Pass   |  4 |   |   |   |
| Step 6: Select the _Done_ button | Customer should be added to the system and the screen should display the name of the customer, the customer's ID and a link to print the ID Card |  Customer's information was added without any issues|Pass   |4   |   |   |   |

- _Test Case #2: Software check that the user has entered a proper email_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available 2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu on the upper left. | Manager Portal is shown. | Manager menu option is shown  | Pass  |   |   |   |
| Step 3:  Select the Manager Option | The GUI displays all the current customers and a button with _+_ symbol|  The app displayes a list with all current customers and gives the user the option to edit or add a customer| Pass  | 1  |   |  |
| Step 4: Press the _+_ button | The GUI displays the following text fields: _First Name_, _Last Name_ and _Email._ |The text fields are displayed |Pass | 1,3  |   |   |
| Step 5: Add the First Name and Last Name of the customer| Text fields accept the input of the customer without any issues. | The Customer's data can be succesfully entered |Pass | 3  |   |   |
| Step 6: Add an email address without the &quot;@&quot; character and then select the _Done_ button| The software should notify the user that the system needs a proper email address | The user can create a user without a proper email address|Fail| 3  | Bug#1  |   |

- _Test Case #3: Software checks for blank test fields_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available 2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu on the upper left. | Manager Portal is shown. | Manager menu option is shown  | Pass  |   |   |   |
| Step 3:  Select the Manager Option | The GUI displays all the current customers and a button with _+_ symbol|  The app displayes a list with all current customers and gives the user the option to edit or add a customer| Pass  | 1  |   |  |
| Step 4: Press the _+_ button | The GUI displays the following text fields: _First Name_, _Last Name_ and _Email._ |The text fields are displayed |Pass | 1,3  |   |   |
| Step 5: Complete just two of the text fields with appropriate data | Text fields accept the input of the customer without any issues. |   The user is able to enter data to any two text fields|  Pass |   |   |   |
| Step 6: Select the Done button | The software should notify the user that it needs all the text fields to be completed. |  The user is able to create a user with all the text fields left blank |  Fail | 3  | Bug#3  |   |   |

**Test Suite #2: Editing a Customer**

- _Test Case #1: Editing a Customer_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available 2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu on the upper left. | Manager Portal is shown. | Manager menu option is shown  | Pass  |   |   |   |
| Step 3: Select the Manager option | A list of current customer should be display | The app displays the customer that have been added  | Pass  | 1  |   |   |
| Step 4: Select one of the customers| The GUI displays the following text fields: _First Name_, _Last Name_ and  _Email._ | The text fields are shown |  Pass |  3 |   | |
| Step 5: Edit the customer's information | The customer is able to erase and update customer information. | Text fields were editable  |   Pass|   3|   | There are no limits on the number of character or spaces  |
| Step 6: Select the Done button | Customer information should be updated. | The customer information was updated  |  Pass | 3  |   |   | | 


**Test Suite #3: Print a Customer Card**

- _Test Case #1: Print a Customer Card from the Edit Customer Screen (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available 2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 1:  Select the Manager Portal | The GUI displays a list of current available customers | the app displays all the available customers|  Pass | 1  |   |   |
| Step 2: Select one of the customers| The GUI displays the following text fields: _First Name_, _Last Name_ and  _Email._ | The text fields are shown |  Pass | 3  |   | |
| Step 3: Select the Print Customer Card button | Customer card should be printed with QR code. |  The app states that the card is printed |   Pass| 4  |   |   |  |

- _Test Case #2: Print a Customer Card from the Add Customer Screen (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available 2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu on the upper left. | Manager Portal is shown. | Manager menu option is shown  | Pass  |   |   |   |
| Step 3:  Select the Manager Option | The GUI displays all the current customers and a button with _+_ symbol|  The app displayes a list with all current customers and gives the user the option to edit or add a customer| Pass  | 1  |   |  |
| Step 4: Press the _+_ button | The GUI displays the following text fields: _First Name_, _Last Name_ and _Email._ |The text fields are displayed |Pass | 1,3  |   |   |
| Step 5: Complete text fields with appropriate data | Text fields accept the input of the customer without any issues. |  The expected outcome is met |Pass   |   |   |   |
| Step 6: Select the Continue button | Customer should be added and the screen should display the name of the customer, the customer's ID and a _print ID_ button | The app displays all the expected items  |  Pass |   |   |   |   |
| Step 7: Select _print ID_ button| Customer card should be printed with QR code | The app states that the card is being printed  | Pass  |4   |   |   |   |

**Test Suite#4: Lane Feature**

- _Test Case #1: System is able to scan QR IDs properly (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Have at least one Customer Cards available and the GoBowl app |   |   |   |   |   |   |
| Step 2:  Select the request lane view | The system prompts the customer to scan their customer card. |  The app prompts the user to scan the card. |Pass   | 6  |   | Simulated test as we don't have the needed camera  |
| Step 3: Place customer card under the camera | The system will scan the QR code and display the corresponding customer&#39;s name.|The name of the customer is displayed and the app ask for confirmation   | Pass  |  6 |   | Simulated test as we don't have the needed camera   |
| Step 4: Press the Continue button | The system displays a text field where the customer can enter the number of players. | The app displays the expected text field  | Pass  |  6 |   |   |   |

- _Test Case #2: System is able to assign a lane (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #1 2. Have 3 customer IDs |   |   |   |   |   |   |
| Step 2: Select two additional players and press continue| The app asks the user to scan the other player's card Ids |  The expected notification is shown | Pass  |   6|   |   |
| Step 3: Place customer card under the camera | The system will scan the QR code and display the corresponding customer&#39;s name. |The app displays the user's name and emails |  Pass |6  |  |Simulated test as we don't have the needed camera |
| Step 4: Press the Continue button | The system displays the assigned lane and players | The expected text is shown  | Pass |  6 |   |   |
| Step 5:  Press _Done_ after all players are displayed | The app should go back to the main page| The app show the home page | Pass  |   6|   |   |   |

- _Test Case #3: Checkout (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #2 successfully |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass | 7  |   |   |
| Step 3: Enter the assigned lane number | The app should allow the user to enter a proper value on the corresponding text field | The user is able to enter the lane number without any issues  | Pass  | 7  |   |   |
| Step 4: Select the Continue button | The system prompts the user to enter the scores of each player. | The app prompt the user for each player's score  | Pass  |   7|   |   |
| Step 5: Select a player | The app should display a controller that the user can easily scroll to find and set their scores. |  The expected controller is shown |Pass   | 7  |   |   |
| Step 6: Enter scores for the 3 players and press Continue | System should display the bill |  The expected outcome is met | Pass  |  7 |   |   |   |

- _Test Case #4: Selecting a random lane at checkout_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #2 successfully |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass | 7  |   |   |
| Step 3: Enter a random lane number | The app notify the user that the rental is not available | The user is notified when a lane rental is not avialable | Pass  |  7 |   |   |

- _Test Case #5: Selecting more than two additional players_
- 
| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #1 2. Have 3 customer IDs |   |   |   |   |   |   |
| Step 2: Select Four additional players and press continue| The app asks the user to scan the other player's card Ids |  The app creates an | Fail  |   6|   |   Bug#2 This failure was expected because there were only 3 test users created for our utility classes. Therefore as shown on the resolution table at the end of the test plan we considered this bug invalid|


- _Test Case #5: Selecting zero additional players_
- 
| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #1 2. Have 3 customer IDs |   |   |   |   |   |   |
| Step 2: Select Zero additional players| The app allow the user to enter the number of additional players without any issues | The expected outcome was occured | Pass  |   6|   |  |
| Step 3: Press the Continue button | The system displays the assigned lane and the sole player | The expected text is shown  | Pass|  6 |   |   |
| Step 5:  Press _Done_  | The app should go back to the main page| The app show the home page | Pass |   6|   |   |   |
**Test Suite #5: Billing**

- _Test Case #1: System notifies the user if the credit card scanner throws an error (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #1 and #2 from Suite #4  successfully |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass |   |   |   |
| Step 3: Enter the assigned lane number | The app should allow the user to enter a proper value on the corresponding text field | The user is able to enter the lane number without any issues  | Pass  |7   |   |   |
| Step 3: Select the Continue button | The system prompts the user to enter the scores of each player. | The app prompt the user for each player's score  | Pass  |   |   |   |
| Step 4: Select a player | The app should display a controller that the user can easily scroll to find and set their scores. |  The expected controller is shown |Pass   |   |   |   |
| Step 5: Enter scores for the 3 players and press Continue | System should display the bill |  The expected outcome is met | Pass  | 7,8  |   |   |   |
| Step 6: Enter the number of players that will be billed| System should display what each player will be billed. | The app splits the bill accuretaly between all the players | Pass  |  7 |   |   |   |
| Step 7: Press the _Confirm Split_ button| System should ask the players to swipe their credit cards. | The app prompts the user to swipe their cards| Pass  | 7  |   |   |   |
| Step 8: Swipe the credit cards| System should displaye if the charge was succefully for each swiped card| The app displays the last four digits of the credit cards and notifies the user if the charge was successful| Pass  | 7,9  |   |   |   |

- _Test Case #2: Splitting the bill more times than there are active players (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #1 and #2 from Suite #4  successfully |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass |   |   |   |
| Step 3: Enter the assigned lane number | The app should allow the user to enter a proper value on the corresponding text field | The user is able to enter the lane number without any issues  | Pass  |7   |   |   |
| Step 3: Select the Continue button | The system prompts the user to enter the scores of each player. | The app prompt the user for each player's score  | Pass  |   |   |   |
| Step 4: Select a player | The app should display a controller that the user can easily scroll to find and set their scores. |  The expected controller is shown |Pass   |   |   |   |
| Step 5: Enter scores for the 3 players and press Continue | System should display the bill |  The expected outcome is met | Pass  | 7,8  |   |   |   |
| Step 6: Enter Five as the number of players that will be billed| System should display the total bill divided by Five . | The app splits the bill accuretaly| Pass  |  7 |   |   |   |


- _Test Case #3: Sunday rate test(Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Change your device settings so that the date for testing falls ona Sunday 2. Completed Test Case #1 and #2 from Suite #4 successfully  |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass |   |   |   |
| Step 3: Enter the assigned lane number | The app should allow the user to enter a proper value on the corresponding text field | The user is able to enter the lane number without any issues  | Pass  |7   |   |   |
| Step 3: Select the Continue button | The system prompts the user to enter the scores of each player. | The app prompt the user for each player's score  | Pass  |   |   |   |
| Step 4: Select a player | The app should display a controller that the user can easily scroll to find and set their scores. |  The expected controller is shown |Pass   |   |   |   |
| Step 5: Enter scores for the 3 players and press Continue | System should display the bill |  The expected outcome is met | Pass  | 7,8  |   |   |   |
| Step 6: Check that the bill for the lane is $30| System should display the bill as $30. | The app displays the right amount for Sunday | Pass  |  7 |   |   |   |

- _Test Case #4: Wednesday rate test(Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Change your device settings so that the date for testing falls on Wednesday 2. Completed Test Case #1 and #2 from Suite #4 successfully  |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass |   |   |   |
| Step 3: Enter the assigned lane number | The app should allow the user to enter a proper value on the corresponding text field | The user is able to enter the lane number without any issues  | Pass  |7   |   |   |
| Step 3: Select the Continue button | The system prompts the user to enter the scores of each player. | The app prompt the user for each player's score  | Pass  |   |   |   |
| Step 4: Select a player | The app should display a controller that the user can easily scroll to find and set their scores. |  The expected controller is shown |Pass   |   |   |   |
| Step 5: Enter scores for the 3 players and press Continue | System should display the bill |  The expected outcome is met | Pass  | 7,8  |   |   |   |
| Step 6: Check that the bill for the lane is $10| System should display the bill as $10. | The app displays the right amount for Sunday | Pass  |  7 |   |   |   |

- _Test Case #5: M,T,TH,F from 9AM to 5PM rate test(Integration Testing)_

| Test Case Seps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Change your device settings so that the date for testing falls on Monday at 10AM  2. Completed Test Case #1 and #2 from Suite #4 successfully  |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass |   |   |   |
| Step 3: Enter the assigned lane number | The app should allow the user to enter a proper value on the corresponding text field | The user is able to enter the lane number without any issues  | Pass  |7   |   |   |
| Step 3: Select the Continue button | The system prompts the user to enter the scores of each player. | The app prompt the user for each player's score  | Pass  |   |   |   |
| Step 4: Select a player | The app should display a controller that the user can easily scroll to find and set their scores. |  The expected controller is shown |Pass   |   |   |   |
| Step 5: Enter scores for the 3 players and press Continue | System should display the bill |  The expected outcome is met | Pass  | 7,8  |   |   |   |
| Step 6: Check that the bill for the lane is $20| System should display the bill as $20. | The app displays the right amount for Sunday | Pass  |  7 |   |   |   |

- _Test Case #6: M,T,TH,F from 5PM to 12AM rate test(Integration Testing)_

| Test Case Seps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Change your device settings so that the date for testing falls on Friday at 9PM  2. Completed Test Case #1 and #2 from Suite #4 successfully  |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass |   |   |   |
| Step 3: Enter the assigned lane number | The app should allow the user to enter a proper value on the corresponding text field | The user is able to enter the lane number without any issues  | Pass  |7   |   |   |
| Step 3: Select the Continue button | The system prompts the user to enter the scores of each player. | The app prompt the user for each player's score  | Pass  |   |   |   |
| Step 4: Select a player | The app should display a controller that the user can easily scroll to find and set their scores. |  The expected controller is shown |Pass   |   |   |   |
| Step 5: Enter scores for the 3 players and press Continue | System should display the bill |  The expected outcome is met | Pass  | 7,8  |   |   |   |
| Step 6: Check that the bill for the lane is $25| System should display the bill as $25. | The app displays the right amount for Sunday | Pass  |  7 |   |   |   |

- _Test Case #7: VIP(Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Perfom a number of lane request followed by checkout until one of the test users spend more than $500 2. Completed Test Case #1 and #2 from Suite #4  successfully |   |   |   |   |   |   |
| Step 2:  Select Checkout on the main page | The system will ask the customer to confirm the lane that was assigned. | The sytem prompts the user for the lane the number  |  Pass |   |   |   |
| Step 3: Enter the assigned lane number | The app should allow the user to enter a proper value on the corresponding text field | The user is able to enter the lane number without any issues  | Pass  |7   |   |   |
| Step 3: Select the Continue button | The system prompts the user to enter the scores of each player. | The app prompt the user for each player's score  | Pass  |   |   |   |
| Step 4: Select a player | The app should display a controller that the user can easily scroll to find and set their scores. |  The expected controller is shown |Pass   |   |   |   |
| Step 5: Enter scores for the 3 players and press Continue | System should display the bill |  The expected outcome is met | Pass  | 7,8  |   |   |   |
| Step 6: Please verify that the VIP discount is being applied to the bill| VIP discount is shown and applied to the bill | The discount is shown and applied | Pass  |  7 |   |   |   |


