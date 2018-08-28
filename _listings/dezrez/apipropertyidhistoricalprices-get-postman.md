{
  "info": {
    "name": "Dezrez Get historical prices for a property by its Id",
    "_postman_id": "16476000-6802-4336-a1fa-94397bd75fd2",
    "description": "Get historical prices for a property by its id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Historical",
      "item": [
        {
          "id": "401baa74-e33d-42d5-8514-77f9797f6fcf",
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
              "id": "7117158e-0573-4c3c-8b7f-de5d17f10e8b"
            }
          ]
        }
      ]
    }
  ]
}