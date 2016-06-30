Test Case#1: Adding a Customer

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2: Expand the menu. | Customer and Manager Portal are shown. |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:\*Add Customer\*\*Edit Customer Info\*\*Print Customer Card\* |   |   |   |   |   |
| Step 3: Select the Add CustomerOption. | The gui displays the following text fields:\*First Name\*\*Last Name\*\*Email\* |   |   |   |   |   |
| Step 4: Complete the text field with appropriate data. | Text fields accept the input of the customer without any issues. |   |   |   |   |   |
| Step 5: Select the Done button. | Customer should be added and displayed on customer screen. |   |   |   |   |   |

Test Suite#1: Manager Features

1. Test Case#2: Editing a Customer

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:\*Add Customer\*\*Edit Customer Info\*\*Print Customer Card\* |   |   |   |   |   |
| Step 3: Select the Edit Customer Info Option | The gui displays the following text fields:\*First Name\*\*Last Name\*\*Email\* |   |   |   |   |   |
| Step 4: Edit the Customer information | The customer is able to erase and update customer information.. |   |   |   |   |   |
| Step 5: Select the Done button. | Customer information should be updated. |   |   |   |   |   |

\*Test Suite#1: Manager Features\*

1. Test Case#3: Print a Customer Card

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Android Platform available2. GoBowl app downloaded |   |   |   |   |   |   |
| Step 2:  Select the Manager Portal | The gui displays the following options:\*Add Customer\*\*Edit Customer Info\*\*Print Customer Card\* |   |   |   |   |   |
| Step 3: Select the &quot;Edit the Customer Info&quot; Option | The screen should display the customer&#39;s information. |   |   |   |   |   |
| Step 5: Select the &quot;More&quot; option icon. | The screen should display a &quot;Print Customer Card&quot; option. |   |   |   |   |   |
| Step 4: Select the &quot;Print Customer Card&quot; button. | Customer card should be printed with QR code. |   |   |   |   |   |

\*Test Suite#2: Lane Feature\*

1. Test Case#4: System is able to scan a QR IDs properly.

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Have 1 Customer Cards available.2. Kiosk available |   |   |   |   |   |   |
| Step 2:  Select the request lane view. | The system prompts the customer to scan their customer card. |   |   |   |   |   |
| Step 3: Place customer card under the camera. | The system will scan the QR code and display the corresponding customer&#39;s name. |   |   |   |   |   |
| Step 4: Press the &quot;continue&quot; button. | The system displays a text field where the customer can enter the number of players. |   |   |   |   |   |

   5. Test Case#5: System is able to assign a lane

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1.Completed Test Case #42. Have 3 customer IDs |   |   |   |   |   |   |
| Step 2:  Select the request lane view. | The system prompts the customer to scan their customer card. |   |   |   |   |   |
| Step 3: Place customer card under the camera. | The system will scan the QR code and display the corresponding customer&#39;s name. |   |   |   |   |   |
| Step 4: Press the &quot;continue&quot; button. | The system displays a text field where the customer can enter the number of players. |   |   |   |   |   |
| Step 5: Enter 3 players and press the continue button. | The system should display prompt the other users to scan their customer cards.. |   |   |   |   |   |
| Step 6: Scan the three cards. | The system should display the name of the player added after each scan. |   |   |   |   |   |
| Step 7:  Press &quot;continue&quot; after all players are displayed. | The system should display the lane assigned and the players. |   |   |   |   |   |

6. Test Case#6: Checkout

| Test Case Steps | Expected Results | Actual Results | (Pass/Fail) | Req # | Issue ID | Comments |
| --- | --- | --- | --- | --- | --- | --- |
| Precondition: 1. Completed Test Case #5 successfully. |   |   |   |   |   |   |
| Step 2:  Select &quot;Checkout&quot; on the kiosk. | The system will ask the customer to confirm the lane that was assigned. |   |   |   |   |   |
| Step 3: Select the &quot;Continue&quot; button. | The system prompts the user to enter the scores of each player. |   |   |   |   |   |
| Step 4: Select a player | The name of the customer should be shown and a text field where the user can input the score should be available. |   |   |   |   |   |
| Step 5: Enter scores for the 3 players. | System should display the bill and prompt the user to scan their credit card. |   |   |   |   |   |