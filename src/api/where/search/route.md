---
layout: page
title: Route Search API
---

Search for a route based on its name.

## Sample Request

[http://api.pugetsound.onebusaway.org/api/where/search/route.json?input=crystal&key=TEST](http://api.pugetsound.onebusaway.org/api/where/search/route.json?input=crystal&key=TEST)

## Sample Response

    {
        "code": 200,
        "currentTime": 1674233501267,
        "data": {
            "limitExceeded": false,
            "list": [
                {
                    "agencyId": "1",
                    "color": "727d84",
                    "description": "",
                    "id": "1_DC1",
                    "longName": "CRYSTAL CITY-L'ENFANT PL SHUTTLE",
                    "shortName": "DC1",
                    "textColor": "000000",
                    "type": 3,
                    "url": ""
                }
            ],
            "outOfRange": false,
            "references": {
                ...
            }
        },
        "text": "OK",
        "version": 2
    }

## Request Parameters

* `input` - the string to search for, encoded directly in the URL:
    * `http://api.pugetsound.onebusaway.org/api/where/search/route.json?input=[INPUT GOES HERE]`
* `maxCount` - the max number of results to return. Defaults to 20.