{
  "info": {
    "name": "Dezrez Assign InboundLead Todos to the predefined neg teams. e.g. Sales Valuers, Sales Viewings, Lettings Viewings etc etc",
    "_postman_id": "f7e76390-bbfc-4199-9030-5073c30764c5",
    "description": "Assign inboundlead todos to the predefined neg teams. e.g. sales valuers, sales viewings, lettings viewings etc etc.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Assign",
      "item": [
        {
          "id": "7b1ad41c-c7da-40b6-8fd3-94a345320f7f",
          "name": "DefaultToDo_AssignLeadsToOwningNegotiatorsBytoDoId",
          "request": {
            "url": "http://api.dezrez.com/api/todo/assignleadstoowningnegotiators?toDoId=%7B%7D",
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
            "description": "Assign inboundlead todos to the owning negotiators of the property.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43f35ef8-e3b4-471a-83bc-a1cd1a74c371"
            }
          ]
        },
        {
          "id": "2220937f-452c-4df2-83c5-1c732d777faa",
          "name": "DefaultToDo_AssignTaskToNegotiatorBytaskIdBynegotiatorId",
          "request": {
            "url": "http://api.dezrez.com/api/todo/assigntasktonegotiator?negotiatorId=%7B%7D&taskId=%7B%7D",
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
            "description": "Assign a task to a negotiator by its id.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8f54c3f3-0a9b-4af6-a747-123d5b459890"
            }
          ]
        },
        {
          "id": "6401475b-6a5f-49b2-aca3-285d5d5dc843",
          "name": "DefaultToDo_AssignLeadsToPredefinedTeamsBytoDoId",
          "request": {
            "url": "http://api.dezrez.com/api/todo/assignleadstopredefinedteams?toDoId=%7B%7D",
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
            "description": "Assign inboundlead todos to the predefined neg teams. e.g. sales valuers, sales viewings, lettings viewings etc etc."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3ac7cadc-ee4a-4489-911a-cbfbd5d8b65c"
            }
          ]
        }
      ]
    }
  ]
}