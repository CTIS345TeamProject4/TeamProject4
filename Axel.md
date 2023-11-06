### Fully Dressed Use Case

|Use Case Section|Comments|
|:---|:---|
|Story|As a vehicle owner located in a northeaster state, I want to be able to complete my vehicle's registration renewal through my state's online RMV services in order to save time and effort. |
|Use Case Title|RMV Vehicle Registration Renewal - Online|
|Story Owner|(RMV) Registery of Motor Vehicles|
|Story Creator|RMV Software Engineers/IT team|
|Revisions and Approvals|Version 1.0, Inital Draft|
|Stakeholders and Interests|RMV <br> Northeastern State Vehicle Owners|
|Scope, context, and background|In today's society, technology has increased the availability to complete services online, reducing human labor and time consumption. The RMV is trying to migrate towards this approach, allowing customers to update and pay services, specifically vehicle registration renewal, through online means.|
|Dependencies|**Assumes:** <br> Northeastern State Vehicle Owners have an online code & sign on access to the website <br> Vehicle Owners must have internet access <br> Vehicle Owner has valid credit card information & sufficient funds in their account <br> RMV has access to the data uploaded by Vehicle Owners|
|Actor Role(s)|Vehicle Owner renewing their vehicle's registration <br> RMV that approves/denies renewal request|
|Precondition(s)|Vehicle owner has vehicle registered previously through the RMV <br> Vehicle owner recieved renewal code <br> Vehicle owner has sufficient funds on credit card account <br> Vehicle owner has internet access|
|Success Guarantee|Vehicle owner is able to access the website, access their vehicle registration renewal form, put in their payment information, and receive a confirmation message saying that their renewal order was a success.|
|Minimal Guarantee|An attempt to renew the owner's vehicle registration is made, but for for some reason, (invalid vehicle title, insufficient funds) the system cannot process the payment, an error message notifies the owner and then the website returns to the previous screen.|
|Trigger(s)|Vehicle owner recieves vehicle registration renewal code 2 months prior to their vehicle's registration expiration date.|
|Main Scenario|1. Vehicle owner receives registration renewal code. <br> 2. Vehicle owner accesses the RMV website and logs in using their renewal code. <br> 3. Vehicle owner enters the code they were given, and then their vehicle information and what service they want (registration renewal). <br> 4. Update any new information about their vehicle. <br> a. Report any changes to the vehicle. <br> b. Report if no longer legal owner of the vehicle. <br> 5. Vehicle owner proceeds to the payment method & input their credit card information. <br> 6. The system processes the payment and either accepts or denies the request. <br> 7. Vehicle owner receives approval confirmation message.|
|Alternative Scenarios or Extensions|**Alternative Scenario 1:** The vehicle owner fails to login to the website using the code that was sent, prompting the website to return to the login page.**Alternative Scenario 2:** Vehicle owner's card gets rejected, and the system prompts the user to use another payment method. **Alternative Scenario 3:** User's request fails to go through, and the website sends an alert message saying that an error occurred, and to check if all of the information is correct.|
|Acceptance Criteria|If code does not work, send a new email giving the customer a new code for their login. <br> Vehicle owner must be able to verify vehicle information and update it if needed. <br> Vehicle owner's payment method must go through, and if it doesn't, the system will reject the renewal request.|
|Test Cases|Enter code provided by RMV <br> verify/update vehicle information <br> Payment must be valid/sufficient funds.|
|Exclusions/Out-of-Scope Items|Cash payments <br> Vehicle is out of comission|
|Assumptions|Vehicle owner received a renewal code. <br> Vehicle owner has access to the internet. <br> Vehicle owner has a credit card with sufficent funds.|
|Non-functional Requirements|UI with easy to undestand interface for the renewal procedure. <br> Vehicle information is accurate & updatable. <br> Payment method is kept confidential and secure. |
|Story Details, Open Issues, and Conversions|Need to determine how much of the driver's information is necessary to complete the renewal information. (SSN?)|