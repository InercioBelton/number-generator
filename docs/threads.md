# Changes the size of the thread-pool

Changes the size of the Thread-pool used to process the Random Number Requests. Maximum supported value should be 10. Minimum value should be 1. 

**URL** : `/threads`

**Example**: `http://127.0.0.1:8080/number-generator/api/threads` 

**Method** : `PUT`

**Data**

Query param `size`: int

## Success Response

**Code** : `200 OK`

**Example**

````json

{
    "code": 200,
    "description": "Thread pool size was successfully changed to 8",
    "message": "SUCCESS"
}

````

