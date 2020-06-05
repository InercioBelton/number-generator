# Get system usage statistics

Get system usage statistics:
* Maximum waiting time- the maximum time that has been spent to process a Random Request
* Minimum waiting time – the minimum time that has been spent to process a Random number request
* Total pending Requests – the total Random Number requests that are currently pending
 

**URL** : `/stats`

**Example**: `http://127.0.0.1:8080/number-generator/api/stats`  

**Method** : `GET`

## Success Response

**Code** : `200 OK`

 

**Example**

````json

{
    "maximumWaitingTime": "0 min, 42 sec, 42000 millis",
    "minimumWaitingTime": "0 min, 30 sec, 30005 millis",
    "totalPendingRequests": 0
}

````

