# Microsoft Graph API Example

## Description
This solution shows how to interact with the Microsoft Graph API with Linx. The solution does the following:
- Does OAuth Authentication
- Get a list of users
- Get information on a specific user
- Get a list of calendars for a user
- Get a list of events on a calendar
- Create a new event

## Usage
### Functions

All Functions have an AccessToken input parameter, thus the Access Token must be retrieved with the GetToken function first

- GetToken: Get an authentication token for use in all other functions (OAuth2)
- ListUsers: Retrieve a list of all users
- GetUser: Retrieve a specific user based on a passed-in User ID
- ListCalendars: Retrieve a list of all calendars for a specific user ID
- ListEvents: Retrieve a list of all events for a specific user ID and calendar ID
- CreateEvent: Create a new event for a specified user and calendar. An event type is passed in to create this event.

### Try it out
Select the TestAddandListEvents function, add in your TenantID, ClientSecret and ClientID along with relevant User and calendar IDs (where required), click Debug and click Start. 

### Use it in your own Linx solution
Copy the relevant function along with its types folder to your solution and call it from anywhere.

### Notes
In order for the solution to work correctly, you must ensure that the correct permissions are applied on your Azure/Graph instance. 

## Contributing

For questions please ask the [Linx community](https://linx/software/community) or use the [Slack channel](https://linxsoftware.slack.com/archives/C01FLBC1XNX). 

## License

[MIT](https://github.com/linx-software/template-repo/blob/main/LICENSE.txt)
