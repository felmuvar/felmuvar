# Test Plan

**Author**: \<CS 6300Team 02\>


| *Version* | *Description*       | 
| ----------|:-------------------:|
| *V1*      | *Initial version: First iteration of the Test Plan*   |

## 1 Testing Strategy

### 1.1 Overall strategy

Verification activities will be performed to ensure that all requirements are met for the GoBowl android app. The verification activities that will be performed are unit testing and system testing. The main focus will be on performing acceptance testing. The team will assigned two members to develop and execute the corresponding test procedures.

### 1.2 Test Selection

Part of the verification effort will be to use unit tests. The other type of verification is BlackBox testing taking into account all the main features of the GoBowl android app.

### 1.3 Adequacy Criterion

The quality of test cases will be gauged by code coverage from Unit Testing and successful acceptance testings.

### 1.4 Bug Tracking

We will be using Github’s integrated issue tracking to track bugs and enhancements. We will consider “bugs” any issues found during our system testing. Enhancement will be defined as features that will enhance the user experience but are not covered on the requirements

### 1.5 Technology

We’re going to use the Junit framework and GitHub’s Issue Tracking to perform and track the verification effort.

## 2 Test Cases

The system test cases below are grouped together in Test Suites corresponding to each main functional feature 

**Test Suite#1: Adding a Customer**

- _Test Case#1: Adding a Customer_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu. | Customer and Manager Portal are shown. |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:
- Add Customer
- Edit Customer Info
- Print Customer Card
 |   |   |   |   |   |
| Step 3: Select the Add CustomerOption. | The gui displays the following text fields:
- First Name
- Last Name
- Email
 |   |   |   |   |   |
| Step 4: Complete the text field with appropriate data. | Text fields accept the input of the customer without any issues. |   |   |   |   |   |
| Step 5: Select the Done button. | Customer should be added and displayed on customer screen. |   |   |   |   |
 |

- _Test Case#2: Software checks that the user has an entered a proper email_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu. | Customer and Manager Portal are shown. |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:
- Add Customer
- Edit Customer Info
- Print Customer Card
 |   |   |   |   |   |
| Step 3: Select the Add CustomerOption. | The gui displays the following text fields:
- First Name
- Last Name
- Email
 |   |   |   |   |   |
| Step 4: Add the First and Last name of the customer. | Text fields accept the input of the customer without any issues. |   |   |   |   |   |
| Step 5: Add an email address without the &quot;@&quot; character and select the &quot;Done&quot; button. | The software should notify the customer that the systems needs a proper email address. |   |   |   |   |   |

- _Test Case#3: Software checks for blank test fields_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu. | Customer and Manager Portal are shown. |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:
- Add Customer
- Edit Customer Info
- Print Customer Card
 |   |   |   |   |   |
| Step 3: Select the Add CustomerOption. | The gui displays the following text fields:
- First Name
- Last Name
- Email
 |   |   |   |   |   |
| Step 4: Complete just two of the text fields with appropriate data. | Text fields accept the input of the customer without any issues. |   |   |   |   |   |
| Step 5: Select the &quot;Done&quot; button. | The software should notify the user that it needs all the text fields to be completed. |   |   |   |   |   |

**Test Suite#2: Editing a Customer**

- _Test Case#1: Editing a Customer_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:
- Add Customer
- Edit Customer Info
- Print Customer Card
 |   |   |   |   |   |
| Step 3: Select the Edit Customer Info Option | The gui displays the following text fields:
- First Name
- Last Name
- Email
 |   |   |   |   |   |
| Step 4: Edit the Customer information | The customer is able to erase and update customer information.. |   |   |   |   |   |
| Step 5: Select the Done button. | Customer information should be updated. |   |   |   |   |   |

- _Test Case#2: Software checks for blank test fields_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu. | Customer and Manager Portal are shown. |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:
- Add Customer
- Edit Customer Info
- Print Customer Card
 |   |   |   |   |   |
| Step 3: Select the Edit CustomerOption. | The gui displays the following text fields:
- First Name
- Last Name
- Email
 |   |   |   |   |   |
| Step 4: Erase one of the text fields from the Customer information. | The user is able to delete text on any text field. |   |   |   |   |   |
| Step 5: Select the &quot;Done&quot; button. | The software should notify the user that it needs all the text fields to be completed. |   |   |   |   |   |

**Test Suite#3: Print a Customer Card**

- _Test Case#1: Print a Customer Card  (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:
- Add Customer
- Edit Customer Info
- Print Customer Card
 |   |   |   |   |   |
| Step 3: Select the &quot;Edit the Customer Info&quot; Option | The screen should display the customer&#39;s information. |   |   |   |   |   |
| Step 5: Select the &quot;More&quot; option icon. | The screen should display a &quot;Print Customer Card&quot; option. |   |   |   |   |   |
| Step 4: Select the &quot;Print Customer Card&quot; button. | Customer card should be printed with QR code. |   |   |   |   |   |

**Test Suite#4: Lane Feature**

- _Test Case#1: System is able to scan a QR IDs properly.(integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Have 1 Customer Cards available.2. Kiosk available |   |   |   |   |   |   |
| Step 2:  Select the request lane view. | The system prompts the customer to scan their customer card. |   |   |   |   |   |
| Step 3: Place customer card under the camera. | The system will scan the QR code and display the corresponding customer&#39;s name. |   |   |   |   |   |
| Step 4: Press the &quot;continue&quot; button. | The system displays a text field where the customer can enter the number of players. |   |   |   |   |   |

- _Test Case#2: System is able to assign a lane  (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1.Completed Test Case #42. Have 3 customer IDs |   |   |   |   |   |   |
| Step 2:  Select the request lane view. | The system prompts the customer to scan their customer card. |   |   |   |   |   |
| Step 3: Place customer card under the camera. | The system will scan the QR code and display the corresponding customer&#39;s name. |   |   |   |   |   |
| Step 4: Press the &quot;continue&quot; button. | The system displays a text field where the customer can enter the number of players. |   |   |   |   |   |
| Step 5: Enter 3 players and press the continue button. | The system should display prompt the other users to scan their customer cards. |   |   |   |   |   |
| Step 6: Scan the three cards. | The system should display the name of the player added after each scan. |   |   |   |   |   |
| Step 7:  Press &quot;continue&quot; after all players are displayed. | The system should display the lane assigned and the players. |   |   |   |   |   |

- _Test Case#3: Checkout  (Integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #5 successfully. |   |   |   |   |   |   |
| Step 2:  Select &quot;Checkout&quot; on the kiosk. | The system will ask the customer to confirm the lane that was assigned. |   |   |   |   |   |
| Step 3: Select the &quot;Continue&quot; button. | The system prompts the user to enter the scores of each player. |   |   |   |   |   |
| Step 4: Select a player | The name of the customer should be shown and a text field where the user can input the score should be available. |   |   |   |   |   |
| Step 5: Enter scores for the 3 players. | System should display the bill and prompt the user to scan their credit card. |   |   |   |   |   |

**Test Suite#5: Customer Card Scanning**

- _Test Case#1: System notifies the user if it&#39;s not able to scan a customer card.(integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Have 1 Customer Cards available.2. Kiosk available |   |   |   |   |   |   |
| Step 2:  Select the request lane view. | The system prompts the customer to scan their customer card. |   |   |   |   |   |
| Step 3: Place customer card under the camera with the QR ID pointed away from the camera. | The system will attempt to scan but then notify the user that&#39;s not able to find the customer card. |   |   |   |   |   |
| Step 4: Place customer card under the camera with the QR ID pointed towards the camera. | The system displays a text field where the customer can enter the number of players. |   |   |   |   |   |
| Step 5: Press the &quot;continue&quot; button. | The system displays a text field where the customer can enter the number of players. |   |   |   |   |   |

**Test Suite#6: Billing**

- _Test Case#1: System notifies the user if the credit card scanner throws an error.(integration Testing)_

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #1 and #2 from Test Suite#4 successfully.2. Organization&#39;s Credit Card. |   |   |   |   |   |   |
| Step 2:  Select &quot;Checkout&quot; on the kiosk. | The system will ask the customer to confirm the lane that was assigned. |   |   |   |   |   |
| Step 3: Select the &quot;Continue&quot; button. | The system prompts the user to enter the scores of each player. |   |   |   |   |   |
| Step 4: Select a player | The name of the customer should be shown and a text field where the user can input the score should be available. |   |   |   |   |   |
| Step 5: Enter scores for the 3 players. | System should display the bill and prompt the user to scan their credit card. |   |   |   |   |   |
| Step6: Scan a credit card incorrectly. | System should notify the user that the payment was not accepted and request the user to try again. |   |   |   |   |   |