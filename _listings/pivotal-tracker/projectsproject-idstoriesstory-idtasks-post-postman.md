{
  "info": {
    "name": "Pivotal Tracker Post Projects Project Stories Story Tasks",
    "_postman_id": "4f08e142-85f6-44dc-9a00-accea73e159b",
    "description": "Post projects project stories story tasks.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "ae59fea3-3131-4fb5-aea1-473d003c6052",
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
              "id": "58714857-c4ac-4185-8174-45a07fda0922"
            }
          ]
        },
        {
          "id": "6424ae18-c4e0-4b87-8037-c182ca4dcbd6",
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
              "id": "6f85100b-fe1d-468e-96d5-38e5f52dae11"
            }
          ]
        },
        {
          "id": "16fa27e1-36a7-4cea-a57e-3fb80bdf0507",
          "name": "deleteProjectsProjectStoriesStoryTasksTask",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete projects project stories story tasks task."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "170ad199-7cd0-42cb-b43a-e1a49fe13269"
            }
          ]
        },
        {
          "id": "5a17be46-e999-4b3a-80f9-2d48721e2162",
          "name": "getProjectsProjectStoriesStoryTasks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/tasks"
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
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get projects project stories story tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83cfbd39-9481-4ff1-b8ea-5690cc6879c5"
            }
          ]
        },
        {
          "id": "460e3402-e817-4320-8965-9b509559e1b5",
          "name": "postProjectsProjectStoriesStoryTasks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.pivotaltracker.com",
              "path": [
                "services",
                "v3",
                "projects/:PROJECT_ID/stories/:STORY_ID/tasks"
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
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Post projects project stories story tasks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e9c1f05-9549-40de-b4a8-95c00e65671f"
            }
          ]
        }
      ]
    }
  ]
}