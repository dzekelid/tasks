{
  "info": {
    "name": "Google Fusion Tables API Delete Task",
    "_postman_id": "4032b9a3-e947-4097-affa-1255f9aaa4d5",
    "description": "Deletes a specific task by its ID, unless that task has already started running.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Task",
      "item": [
        {
          "id": "d020a91c-029b-4b40-a494-603099f32341",
          "name": "fusiontables.task.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "fusiontables",
                "v2",
                "tables/:tableId/tasks"
              ],
              "query": [
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "startIndex",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "tableId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a list of tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a08f3eec-e378-4b8b-add8-7dfd2e082ca3"
            }
          ]
        },
        {
          "id": "bfe7a6b1-d5d6-4f1f-93df-704e01ae7345",
          "name": "fusiontables.task.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "fusiontables",
                "v2",
                "tables/:tableId/tasks/:taskId"
              ],
              "variable": [
                {
                  "id": "tableId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "taskId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a specific task by its ID, unless that task has already started running."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc91e2fb-6181-417e-90a3-26fe8c05bbae"
            }
          ]
        }
      ]
    }
  ]
}