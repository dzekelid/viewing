{
  "info": {
    "name": "Dezrez Record that the feedback for a Viewing was notified to the vendor.",
    "_postman_id": "bd9647e1-c56b-4e27-bd73-28092daada63",
    "description": "Record that the feedback for a viewing was notified to the vendor..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Marks",
      "item": [
        {
          "id": "474acec5-1ec2-4037-aded-dbbfe8a97ddd",
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
              "id": "05a4b7c4-f5ff-4319-880e-d5a68d2e4815"
            }
          ]
        }
      ]
    },
    {
      "name": "Edit",
      "item": [
        {
          "id": "c2cd9081-1325-4ae5-af0e-c0e277667ed9",
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
              "id": "984165b6-e030-4d59-8a3d-eef64d61c53f"
            }
          ]
        },
        {
          "id": "807443f8-4fe3-40a4-b8c9-52b139850ea0",
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
              "id": "84da758f-f47e-4220-ac53-ef76f284ef90"
            }
          ]
        }
      ]
    },
    {
      "name": "Record",
      "item": [
        {
          "id": "6849574b-508d-4030-8b9b-e7eb16328ae2",
          "name": "Viewing_FeedbackNotifiedByviewingFeedbackIdBytypeBynotifiedDateBynegIds",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/viewing/:viewingFeedbackId/feedbacknotified"
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
            "method": "POST",
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
            "description": "Record that the feedback for a viewing was notified to the vendor.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8790f2da-fc78-4ba7-b104-61e55930f965"
            }
          ]
        }
      ]
    }
  ]
}