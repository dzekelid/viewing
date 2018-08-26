{
  "info": {
    "name": "Dezrez Edit whether the vendor feedback for the viewing has been reviewed.",
    "_postman_id": "9bf022b5-6706-4684-aea9-7b74abe070a6",
    "description": "Edit whether the vendor feedback for the viewing has been reviewed..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Marks",
      "item": [
        {
          "id": "deeb3aa6-2445-46b8-bf93-ad5487d9208b",
          "name": "List_DeleteFeedbackFollowUpListFilterByid",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/list/feedbackfollowups/filters/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
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
            "description": "Marks feedback follow up list filter as deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d88dc89-5665-46e6-a00e-e564254b8f82"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "d609c93e-b807-456a-a1fa-41685a73ba94",
          "name": "Viewing_EditFeedbackNotifiedByviewingFeedbackIdByvendorNotifiedIdBytypeBynotifiedDateBynegIds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/viewing/:viewingFeedbackId/editfeedbacknotified"
              ],
              "query": [
                {
                  "key": "negIds",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "notifiedDate",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "vendorNotifiedId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "viewingFeedbackId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Edit that the feedback for a viewing was notified to the vendor.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "59a226fe-c50a-48ea-8d7a-aefee722ac39"
            }
          ]
        },
        {
          "id": "edf6bfb3-3b17-408f-9842-e0f9e5f6213f",
          "name": "Viewing_EditFeedbackReviewedByviewingFeedbackIdBymarkAsReviewed",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/viewing/:viewingFeedbackId/editfeedbackreviewed"
              ],
              "query": [
                {
                  "key": "markAsReviewed",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "viewingFeedbackId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
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
            "description": "Edit whether the vendor feedback for the viewing has been reviewed.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bd52ce8-754e-4275-8499-0626a4adc2dd"
            }
          ]
        }
      ]
    }
  ]
}