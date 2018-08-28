{
  "info": {
    "name": "Google Fusion Tables API Get Tasks",
    "_postman_id": "9c9db849-7d8b-4f2d-a2ab-e99b74cc59dc",
    "description": "Retrieves a list of tasks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Task",
      "item": [
        {
          "id": "a0de1278-8d73-4b45-9654-766c4e119829",
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
              "id": "2ce0ad3e-377a-48c1-b3ff-11c436d407a1"
            }
          ]
        }
      ]
    }
  ]
}