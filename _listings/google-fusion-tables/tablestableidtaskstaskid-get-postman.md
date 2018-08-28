{
  "info": {
    "name": "Google Fusion Tables API Get Task",
    "_postman_id": "d24daafc-37eb-417c-8650-2d3eb1bbcd32",
    "description": "Retrieves a specific task by its ID.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Task",
      "item": [
        {
          "id": "f9e0e966-5503-4b10-ae79-7608581cac63",
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
              "id": "7f450228-eb98-40c8-9a92-52a113dd9ab1"
            }
          ]
        },
        {
          "id": "1b796def-f9ea-4136-8f95-5cdbdeda0aba",
          "name": "fusiontables.task.get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves a specific task by its ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b7f2b2fb-6640-4646-a51b-77e068ddd527"
            }
          ]
        },
        {
          "id": "0274f60f-04d8-4a33-a928-e5a1a3fd22ed",
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
              "id": "313bf113-e87c-49f4-bd0b-897ce164b59f"
            }
          ]
        }
      ]
    }
  ]
}