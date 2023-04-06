# Users API
##### JSON Data Endpoints
- api.unnamedsandbox.com/users/:id/
Gets public user data from an ID in the URL paremeter. Requires a user ID and API key to access data.
Example of the data returned:
    ```json
    {
        _id: 1,
        username: "Example",
        administrator: false,
        about: "This is an example.",
        badges: [
            {
                title: "Example Badge",
                description: "This is an example."
            }
        ],
        friends: [],
        followers: [],
        following: [],
        worldVisits: 0,
        joinDate: "January 1 2000",
        lastOnline: "January 1 2023"
    }
    ```
- api.unnamedsandbox.com/users/:id/inventory/
Gets public inventory data from an ID in the URL parameter. Requires a user ID and api key to access data.
Example of the data returned:
    ```json
    [100, 123, 3320, 124123]
    ```
    The array contains the IDs' for the items in the user's inventory.
##### Image Data Endpoints
- api.unnamedsandbox.com/users/:id/image?type=headshot
Gets public image data from an ID in the url parameter. Requires a user ID and api key to access data.
Example of the data returned:
   ![alt text](out_headshot.png "Headshot")
- api.unnamedsandbox.com/users/:id/image?type=fullbody
Gets public image data from an ID in the url parameter. Requires a user ID and api key to access data.
Example of the data returned:
   ![alt text](out.png "Full Body")