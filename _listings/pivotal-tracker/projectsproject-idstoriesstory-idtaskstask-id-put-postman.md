{
  "info": {
    "name": "Pivotal Tracker Put Projects Project Stories Story Tasks Task",
    "_postman_id": "0a23a18b-9312-4ead-9f48-02b203dece23",
    "description": "Put projects project stories story tasks task.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "e663cba9-2aa7-4b75-8828-e43f6d2c8cca",
          "name": "getProjectsProjectStoriesStoryTasksTask",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/tasks/:TASK_ID"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "STORY_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "TASK_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get projects project stories story tasks task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e9b016a-4c94-467b-aa79-13db0479b65d"
            }
          ]
        },
        {
          "id": "864829c9-0c38-431e-a57f-c18dfabae887",
          "name": "putProjectsProjectStoriesStoryTasksTask",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/tasks/:TASK_ID"
              ],
              "variable": [
                {
                  "id": "PROJECT_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "STORY_ID",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "TASK_ID",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Put projects project stories story tasks task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43a6fa83-121b-4f41-91d3-a196cd8bd1f3"
            }
          ]
        }
      ]
    }
  ]
}