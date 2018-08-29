{
  "info": {
    "name": "Dezrez Edit that the feedback for a Viewing was notified to the vendor.",
    "_postman_id": "a31ee37a-9e3f-43a2-9111-20d4c0456b9f",
    "description": "Edit that the feedback for a viewing was notified to the vendor..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Marks",
      "item": [
        {
          "id": "d933e899-9559-4a88-b33a-1b5ba8b06e0e",
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
              "id": "e2978536-5593-4f04-857d-8667395f1acc"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "889d466c-aa4f-4260-8c11-9b6c11d0c0b7",
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
              "id": "7789e0aa-31f9-4567-90a7-cfbb62b2b851"
            }
          ]
        }
      ]
    }
  ]
}