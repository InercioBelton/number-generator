# Cancels a random number request

 Cancels a Random Number Request that is pending

**URL** : `/{requestId}/cancel`

**Example**: `http://127.0.0.1:8080/number-generator/api/1d429f39-4aee-4238-a8d9-baa57eb0726e/cancel`

**Method** : `PUT`

**Data**

Path param `requestId`: String

## Success Response

**Code** : `200 OK`

 

**Example**

````json

{
    "code": 200,
    "description": "Request with ID 1d429f39-4aee-4238-a8d9-baa57eb0726e was canceled successfully",
    "message": "SUCCESS"
}

````

