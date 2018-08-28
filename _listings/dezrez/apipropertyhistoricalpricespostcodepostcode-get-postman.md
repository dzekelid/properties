{
  "info": {
    "name": "Dezrez Get historical prices for a property by its Id",
    "_postman_id": "9259b8ee-4938-4961-aaf9-6f47f68d43a2",
    "description": "Get historical prices for a property by its id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Historical",
      "item": [
        {
          "id": "fe5866eb-2683-45c5-b2c1-739e0b4e4403",
          "name": "HistoricalPrice_GetByPropertyIdByidBypageNumberBypageSize",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/:id/historicalprices"
              ],
              "query": [
                {
                  "key": "pageNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get historical prices for a property by its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "057d8a29-3aa0-467b-bd27-13d51061f093"
            }
          ]
        },
        {
          "id": "4f352800-023b-4e2f-abdd-b559bb9050e8",
          "name": "HistoricalPrice_GetByPostcodeBypostcodeBypropertyTypeBystyleTypeByleaseTypeBypageNumberBypageSize",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/historicalprices/postcode/:postcode"
              ],
              "query": [
                {
                  "key": "leaseType",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageNumber",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageSize",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "propertyType",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "styleType",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "postcode",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get historical prices for a property by its id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "60a3c5b4-f641-4dd3-a17d-ccbc27dd0f50"
            }
          ]
        }
      ]
    }
  ]
}