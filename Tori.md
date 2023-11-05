### Fully Dressed Use Case

|Use Case Section|Comments|
|:---|:---|
|Story|As a vehicle owner in a northeastern state, I want to renew my vehicle registration online through my state's RMV, so that I can easily complete my registration renewal and payment.|
|Use Case Title|Renew Vehicle Registration Online|
|Story Owner|The RMV|
|Story Creator|The RMV IT Team|
|Revisions and Approvals|Version 1.0, RMV, Initial Draft|
|Stakeholders and Interests|RMV <br> Vehicle Owners|
|Scope, context, and background|Online Vehicle Registration Renewal: The current state of vehicle registration renewal occuring through traditional means, either in person or through mail, is no longer practical given the expanding amount of registrations and the related information for each vehicle registrant. The new RMV online system simplifies and streamlines the vehicle registration renewal process. Vehicle owners will receive a notification prior to their renewal due date, which will outline their renewal options. The online option to renew will involve verifying vehicle information, reporting changes and making a payment. The system will also be able to hand other registration-related capabilities such as such as web-based new vehicle registration for dealerships, production of replacement documents, and management reporting. |
|Dependencies|**Assumes:** <br> Vehicle owners will have access to internet <br> Vehicle owners will have access to a valid credit card for their payment|
|Actor Role(s)|Vehicle owner renewing their vehicle registration <br> The RMV acessing vehicle registration data|
|Precondition(s)|Vehicle owner has internet access <br> Vehicle owner has a valid credit card <br> Vehicle owner has received a renewal notifiaction|
|Success Guarantee|The vehicle owner renews their vehicle registration online, and the payment they provide is processed|
|Minimal Guarantee|The online system will give the vehicle owner an error message when they can't complete the renewal, and then the system returns to its prior state|
|Trgger(s)|Vehicle owner chooses to renew online after receiving a renewal notification|
|Main Scenario|1. Vehicle owner receives their renewal notification. <br> 2. Vehicle owner chooses the online renewal option. <br> 3. Vehicle owner visits the RMV website. <br> 4. Vehicle owner enter the code they received from their notification. <br> 5. The system gets the vehicle owner to verify vehicle information. <br> a. Vehicle reports any changes if they have happened. <br> 6. Vehicle owner makes their payment with a credit card. <br> 7. The system processes the payment and renews the vehicle registration.
|Alternative Scenarios or Extensions|**Alternative Scenario 1:** If the login code fails, an error message is generated for the vehicle owner and they are returned to the landing screen. **Alternative Scenario 2:** If the payment method fails, an error message is generated that prompts the vehicle owner to provide an alternative payment. **Alternative Scenario 3:** If the system is unable to verify the vehicle information, an error message is generated and the system will prompt the vehicle owner to review the vehicle information.|
|Acceptance Criteria|Minimum Viable Solution must-haves: <br> - If the vehicle owner code is incorrect, the system must generate an error message and return to the landing page <br> - Vehicle owner must be able to verify their correct vehicle information <br> - Vehicle owner must be allows to report changes if needed and the system must save those changes <br> - The vehicle owner payment method must be secure and the system must sucessfully process the transaction|
|Test Cases|**Test Registration of following features:** <br> - Enter valid/invalid code from renewal notifiction <br> - Verify vehicle information <br> - Report vehicle changes <br> - Report vehicle changes without verification occuring <br> - Make payment with valid/invalid credit card|
|Exclusions/Out-of-Scope Items|Ability to handle other payment methods that aren't credit card <br> Reporting of complex changes outside the scope of vehicle verification|
|Assumptions|All vehicle owners will have access to internet <br> All vehicle owners will have a valid credit card for payment|
|Non-functional Requirements|A user-friendly interface for the website <br> Vehicle information is secure and not acessible to outside systems <br> Payment information is secure and not accessible to outside systems|
|Story Details, Open Issues, and Conversions|Determine protocol for sharing informaton with outside systems like law enforcement agencies|