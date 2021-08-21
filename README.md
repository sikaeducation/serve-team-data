# Serve Team Data

Using the included `.csv` dataset:

* Build a web server in `app.js`.
* Return the entire collection as JSON for `GET` requests to the `/teams` path of the server.
* Return an individual item as JSON for `GET` requests for the id of a player, such as `/teams/4`.
* Return an error message as JSON for `GET` requests for resources that doesn't exist, such as `/`, `/100`, and `/forty-five`.
* The server should include appropriate CORS headers on all responses.
* Deploy the server.

## Examples

A data list should look like this:

```
{
    "data": [{
        "id": 1,
        "firstAttribute": "firstValue",
        "secondAttribute": "secondValue"
    },{
        "id": 2,
        "firstAttribute": "firstValue",
        "secondAttribute": "secondValue"
    }]
}
```

A data item should look like this:

```
{
    "data": {
        "id": 1,
        "firstAttribute": "firstValue",
        "secondAttribute": "secondValue"
    }
}
```

An error should look like this:

```
{
    "error": {
        "message": "No record found!"
    }
}
```
