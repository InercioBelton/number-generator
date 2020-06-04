# Changes the minumum request duration

Changes the minimum allowed random number generation request duration 

**URL** : `/random`

 

**Method** : `PUT`

**Data**

Query param `time`: long

## Success Response

**Code** : `200 OK`

 

**Example**

````json

{
    "code": 200,
    "description": "Minimum random number generation request durantion was successfully changed to 35",
    "message": "SUCCESS"
}

````

