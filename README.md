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

- GetToken: Get an authentication token for use in all other functions (OAuth2) - Pass in the TennantID, ClientID, Client Secret and Scope. 
- ListUsers: Retrieve a list of all users - Pass in the AccessToken
- GetUser: Retrieve a specific user based on a passed-in User ID - Pass in the AccessToken and UserID
- ListCalendars: Retrieve a list of all calendars for a specific user ID - Pass in the AccessToken and User ID
- ListEvents: Retrieve a list of all events for a specific user ID and calendar ID - Pass in the AccessToken, User ID and Callendar ID
- CreateEvent: Create a new event for a specified user and calendar. An event type is passed in to create this event - Pass in the AccessToken, User ID, Callendar ID and event details

### Try it out
Select the TestAddandListEvents function, add in your TenantID, ClientSecret and ClientID along with relevant User and calendar IDs (where required), click Debug and click Start. User and Calendar IDs can be retrieved by debugging to the ListUsers and ListCalendar functions. 

### Use it in your own Linx solution
Copy the relevant function along with its types folder to your solution and call it from anywhere.
Also note that you will need to create a setting for the MsGraphApiUrl - this is to facilitate easier switching when a new version of the API comes out. 

### Notes
In order for the solution to work correctly, you must ensure that the correct permissions are applied to your Azure/Graph instance. 

## Contributing

For questions, please ask the [Linx community](https://linx/software/community)

## License

[MIT](https://github.com/linx-software/template-repo/blob/main/LICENSE.txt)
