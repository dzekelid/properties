{
  "info": {
    "name": "Plentymarkets Attach a property to a property group",
    "_postman_id": "62b0e981-48d1-4f22-9ab3-59a488aeeeaf",
    "description": "Attaches a property to a property group. The ID of the property and the ID of the property group must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mass",
      "item": [
        {
          "id": "39723aca-50f8-4620-8523-0346ca97c9e2",
          "name": "postRestPropertiesGroupsGroupProperties",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/properties/groups/:groupId/properties"
              ],
              "variable": [
                {
                  "id": "groupId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Mass attach propertyid and groupid collection into the pivot table.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2116fadf-3921-4ba6-8091-0fbc0361a7dc"
            }
          ]
        }
      ]
    },
    {
      "name": "Attach",
      "item": [
        {
          "id": "e08c400e-4529-4a61-b5fc-9e7e4dbb510a",
          "name": "postRestPropertiesGroupsGroupPropertiesProperty",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/properties/groups/:groupId/properties/:propertyId"
              ],
              "variable": [
                {
                  "id": "groupId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "propertyId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Attaches a property to a property group. The ID of the property and the ID of the property group must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dea8b110-e4c2-4b4d-8054-5b1677e4cb5c"
            }
          ]
        }
      ]
    }
  ]
}