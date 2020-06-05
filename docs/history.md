# Get list of generated random numbers

Returns a List of Generated Random Numbers. This includes the time that was taken to process
each random number.

**URL** : `/history`

**Example**: `http://127.0.0.1:8080/number-generator/api/history`

**Method** : `GET`

## Success Response

**Code** : `200 OK`

 

**Example**

````json

[
    {
        "generatedNumber": 334556547,
        "processingTime": "0 min, 33 sec, 33000 millis"
    },
    {
        "generatedNumber": 34232423423423,
        "processingTime": "0 min, 31 sec, 31000 millis"
    },
    {
        "generatedNumber": 5464567675668,
        "processingTime": "0 min, 42 sec, 42000 millis"
    },
    {
        "generatedNumber": 804162030458415521,
        "processingTime": "0 min, 30 sec, 30005 millis"
    }
]

````

