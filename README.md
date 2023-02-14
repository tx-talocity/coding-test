# coding-assignment

The coding assignment can be done in any language of your choice or as specified by the interviewer.

- You are given a list of projects. Each project contains an ID and name as description. See example below 

```
{
"id" : 456,
"name" : "Django"
}
```
- The projects can be stored in any data store of your choice. It could be a relational/nosql database, it could be a data structure harcoded in the code or anything that you prefer.

## Detailed Requirements

- Accept requests for the GET /projects/:id endpoint, where id is the value passed in the URL. If the ID value is not set or is empty in the URL, the server responds back with the status code 400 and the JSON message {"message" : "BAD REQUEST"}.

- If the ID is valid, filter the projects list based on the ID passed as input to the endpoint such that project id matched the input passed. The server sends a JSON response back with the filtered project data, along with the status code 200.

- If the ID is valid but no matching projects are found for the ID, the server responds with the status code 404.

- If the request to the web server contains a route other than /projects, the server responds back with the status code 404.

- Make sure that the server is listening for requests on port 8000. External tools will not be able to be connected to any port other than 8000.

- You can use either DJango or Flask for code.
