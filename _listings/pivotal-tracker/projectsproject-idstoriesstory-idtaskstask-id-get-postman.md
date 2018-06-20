{
  "info": {
    "name": "Pivotal Tracker Get Projects Project Stories Story Tasks Task",
    "_postman_id": "4f96d997-eec7-4175-a899-105ce8277bac",
    "description": "Get projects project stories story tasks task.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Projects",
      "item": [
        {
          "id": "a0c68570-7dc8-4ef4-9d75-c772882ac165",
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
              "id": "db5f8ca5-4a56-4120-bf49-b2d62f8e283f"
            }
          ]
        }
      ]
    }
  ]
}