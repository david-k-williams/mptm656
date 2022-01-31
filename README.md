# MPTM 656 - Cloud Computing & Virtual Data
david k. williams
## Module 3 Excercise
### Use Case
A digital banking customer wants to transfer $1,000 from their checking account to their savings account. 

### Narrative
The user is authenticated to access the mobile application through integration with Okta. The user initiates the flow to transfer $1,000 from their check account to their savings account. An API request is kicked off from the mobile application to the API gateway. The API gateway routes two requests: one request to update the banking core and one request to update the audit database. On the success of the update in the banking core, the API returns a success message with updated balances. The mobile application renders a success message and displays the newly available balances for the user's check and savings accounts.

### Key Component Decisions
- Azure is the general cloud provider
- Okta, a SaaS solution, is the Identity Provider (IdP) integrated via SDK in the mobile application
- OpenAPI Banking is leveraged with an API first Banking-Core-as-a-Service solution
### Component Diagram for Mobile Banking Application - Account Transfer Flow
![Alt text](exports\png\module-3-diagram.png)
this file was generated using plantUML
