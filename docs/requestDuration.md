# Changes the minumum request duration

Changes the minimum allowed random number generation request duration 

**URL** : `/requestDuration`

**Example**: `http://127.0.0.1:8080/number-generator/api/requestDuration` 

**Method** : `PUT`

**Data**

Query param `time`: long

## Success Response

**Code** : `200 OK`

 

**Example**

````json

{
    "code": 200,
    "description": "Minimum random number generation request duration was successfully changed to 35",
    "message": "SUCCESS"
}

````

