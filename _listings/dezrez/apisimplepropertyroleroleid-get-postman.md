{
  "info": {
    "name": "Dezrez Get a property with an associated role by their Id's",
    "_postman_id": "933ca783-92a1-4900-b6cc-d5d1176ce9d6",
    "description": "Get a property with an associated role by their id's.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "f8949a77-dd42-456c-8fea-53de4dc59022",
          "name": "AccountingSystem_GetOfficeAccounts",
          "request": {
            "url": "http://api.dezrez.com/api/accountingsystem/officeaccounts",
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
            "description": "Get list of office accounts associated with the accounting system."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30f75a13-30c5-49b3-bf99-d41c0facc6a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Returns",
      "item": [
        {
          "id": "cb1a2060-2452-4da9-a483-3d3542f7947f",
          "name": "DocumentGeneration_GetLetterTemplateByletterTemplateId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/documentgeneration/lettertemplate/:letterTemplateId"
              ],
              "variable": [
                {
                  "id": "letterTemplateId",
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
            "description": "Returns a list of lettertemplates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f934e8e-ba6e-4d5e-a0a0-e11bcb74ae87"
            }
          ]
        },
        {
          "id": "88e9b4d4-170c-4335-b2f6-235deecd0b20",
          "name": "DocumentGeneration_GetPrintableMergeTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/mergetemplates",
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
            "description": "Returns a list of lettertemplates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "09108857-c0ee-42a2-bf05-2792d8ad4a59"
            }
          ]
        },
        {
          "id": "deb69bf9-be48-4ffb-aaf2-e49109ca2748",
          "name": "DocumentGeneration_GetUnusedMergeTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/unusedmergetemplates",
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
            "description": "Returns a list of lettertemplates associated to this agency that are not currently used in any envelope templates."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4f52506-89a9-48d2-a7f6-d04db1041985"
            }
          ]
        },
        {
          "id": "0791c47e-4952-4eae-97c6-87bbc6e98a42",
          "name": "DocumentGeneration_GetTemplatesUsingAnalyticsByanalyticsId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/documentgeneration/templatesusinganalytics/:analyticsId"
              ],
              "variable": [
                {
                  "id": "analyticsId",
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
            "description": "Returns a list of lettertemplates associated to this agency and to a particular google analyitics campaign."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "049ffdcf-402d-414a-a587-5e00c11ba61b"
            }
          ]
        },
        {
          "id": "0e9241f6-2fca-4240-8d8b-3c74c4a5dc87",
          "name": "DocumentGeneration_GetPrintableInsertableTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/insertabletemplates",
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
            "description": "Returns a list of insertable templates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c7dbea3-9ac5-405d-8b10-7eca455c5191"
            }
          ]
        },
        {
          "id": "b203ddc6-ae1b-4dd5-bfd7-552f73786de3",
          "name": "DocumentGeneration_GetPrintableHeaderTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/headertemplates",
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
            "description": "Returns a list of header templates associated to this agency with their associated brand info."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b4b7e650-b1c1-4978-8fe6-b737171c3bdd"
            }
          ]
        },
        {
          "id": "02dc9267-eaa2-42a1-99b4-2c7879abf296",
          "name": "DocumentGeneration_GetEnvelopeTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/envelopetemplates",
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
            "description": "Returns a list of envelope templates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd3aae66-4986-4c50-aba2-d7775209b237"
            }
          ]
        },
        {
          "id": "489e9af5-4163-4c30-8252-75de2b79e369",
          "name": "DocumentGeneration_GetEnvelopeTemplatePacks",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/envelopetemplatepacks",
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
            "description": "Returns a list of envelope template packs associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7b36a65-deb1-42fe-918e-52ca67437aec"
            }
          ]
        },
        {
          "id": "91e12f72-9fa7-4d1e-aa37-b5f9100e5528",
          "name": "DocumentGeneration_GetEnvelopeTemplatePackTypesByinUseOnly",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/envelopetemplatepacktypes?inUseOnly=%7B%7D",
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
            "description": "Returns a list of envelope template packs associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "00df3116-61b8-4549-8dd7-0f7f58b0dbf6"
            }
          ]
        },
        {
          "id": "5f9030f7-c16a-4380-8926-b261a170012b",
          "name": "DocumentGeneration_GetEmailTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/emailtemplates",
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
            "description": "Returns a list of email templates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f9c4b35e-81b9-4f3c-a757-ec2a86bcf1e6"
            }
          ]
        },
        {
          "id": "558dd3ca-cdc6-4d36-94fe-bc8bc4baab44",
          "name": "DocumentGeneration_GetTemplatesBytemplateType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/documentgeneration/templates/:templateType"
              ],
              "variable": [
                {
                  "id": "templateType",
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
            "description": "Returns a list of mergable templates for any type associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30467541-b88e-4062-95b5-7ce79613969e"
            }
          ]
        },
        {
          "id": "5e2229bc-1422-4af8-8732-2006ea433a9c",
          "name": "DocumentGeneration_GetSmsTemplates",
          "request": {
            "url": "http://api.dezrez.com/api/documentgeneration/smstemplates",
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
            "description": "Returns a list of sms templates associated to this agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50e2c473-b95c-4dc8-8e9c-d3f9138c310c"
            }
          ]
        }
      ]
    },
    {
      "name": "Live",
      "item": [
        {
          "id": "0d0eb6bb-316b-4a9d-a832-ad7d630804cd",
          "name": "Portal_GetLivePortalInformationRecordsForRoleByroleId",
          "request": {
            "url": "http://api.dezrez.com/api/admin/portal/getportaluploadsforrole?roleId=%7B%7D",
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
            "description": "Get all the live portal uploads associated with a property marketing role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "be5f26ee-3de3-4542-941c-431d2daa6228"
            }
          ]
        }
      ]
    },
    {
      "name": "Of",
      "item": [
        {
          "id": "2ca61c5e-e216-4f1e-ab8b-fcf8d9085491",
          "name": "Property_ValuationsByidBypageSizeBypageNumber",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/property/:id/valuations"
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
            "description": "Get all of the valuations associated to the current owner of the property.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "94c997b6-ab08-460e-a273-0cc20047dca0"
            }
          ]
        },
        {
          "id": "2d382734-f51e-4b2a-b0a7-cd5ce62c0962",
          "name": "Role_OffersByidBypageSizeBypageNumberByexcludeDrafts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/role/:id/offers"
              ],
              "query": [
                {
                  "key": "excludeDrafts",
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
            "description": "Get all of the offers associated to the current property marketing role.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7f1713f5-d847-4c6d-b3e9-d055c252f057"
            }
          ]
        },
        {
          "id": "dd84c3d4-7b99-4785-88b2-d8cb539cd70c",
          "name": "Role_ViewingsByidBypageSizeBypageNumberByexcludeDrafts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/role/:id/viewings"
              ],
              "query": [
                {
                  "key": "excludeDrafts",
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
            "description": "Get all of the viewings associated to the current property marketing role.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b33f6984-2312-4e67-9b17-7ecad9e6e1f5"
            }
          ]
        }
      ]
    },
    {
      "name": "Basic",
      "item": [
        {
          "id": "5316299d-0adb-4cd1-83a4-8d30a603f836",
          "name": "Role_OffersBasicByid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/role/:id/offersbasic"
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
            "description": "Get a basic list of offers associated to the current property marketing role.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a43aaa42-73ec-4614-bd55-5dbc014ca745"
            }
          ]
        }
      ]
    },
    {
      "name": "Property",
      "item": [
        {
          "id": "a8af2ad9-8105-489c-b596-0abd8bb3bbae",
          "name": "SimplePropertyRole_GetByroleId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/simplepropertyrole/:roleId"
              ],
              "variable": [
                {
                  "id": "roleId",
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
            "description": "Get a property with an associated role by their id's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1f277438-a587-4160-9e81-e6197391302e"
            }
          ]
        }
      ]
    }
  ]
}