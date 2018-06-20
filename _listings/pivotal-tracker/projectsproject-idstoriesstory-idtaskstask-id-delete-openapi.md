---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 0
info:
  title: Pivotal Tracker Delete Projects Project Stories Story Tasks Task
  description: Delete projects project stories story tasks task.
  version: 1.0.0
host: www.pivotaltracker.com
basePath: /services/v3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /projects/{PROJECT_ID}/stories/{STORY_ID}/tasks/{TASK_ID}:
    get:
      summary: Get Projects Project Stories Story Tasks Task
      description: Get projects project stories story tasks task.
      operationId: getProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
    put:
      summary: Put Projects Project Stories Story Tasks Task
      description: Put projects project stories story tasks task.
      operationId: putProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-put
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
    delete:
      summary: Delete Projects Project Stories Story Tasks Task
      description: Delete projects project stories story tasks task.
      operationId: deleteProjectsProjectStoriesStoryTasksTask
      x-api-path-slug: projectsproject-idstoriesstory-idtaskstask-id-delete
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
      - in: path
        name: TASK_ID
        description: The ID of the task
      responses:
        200:
          description: OK
      tags:
      - Projects
      - PROJECT
      - ID
      - Stories
      - STORY
      - ID
      - Tasks
      - TASK
      - ID
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---