{
  "info": {
    "name": "Pivotal Tracker Delete Projects Project Stories Story Tasks Task",
    "_postman_id": "53bb4655-7702-4d10-8213-33f8d0e7d2d8",
    "description": "Delete projects project stories story tasks task.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "0b7d47eb-3de1-4b0d-8f0c-b6aa6b4c99e6",
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
              "id": "e1444fe9-dc81-4a9e-bbfd-69bd91035c1b"
            }
          ]
        },
        {
          "id": "c7fb5ae4-2b27-4f1c-a917-b6df0cd91fc9",
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
              "id": "117c2312-5fcc-44f9-86f5-1ed0daa133e1"
            }
          ]
        },
        {
          "id": "14abde6f-75d3-4511-9718-31430a7e8a44",
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
              "id": "829d891d-0907-4a7e-aa31-42ce70dd3b75"
            }
          ]
        }
      ]
    }
  ]
}