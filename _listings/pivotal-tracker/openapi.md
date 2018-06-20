---
swagger: "2.0"
x-collection-name: Pivotal Tracker
x-complete: 1
info:
  title: Pivotal Tracker
  description: access-and-manipulate-agile-project-management-data-including-projects-stories-and-tasks-
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
  /projects/{PROJECT_ID}/stories/{STORY_ID}/tasks:
    get:
      summary: Get Projects Project Stories Story Tasks
      description: Get projects project stories story tasks.
      operationId: getProjectsProjectStoriesStoryTasks
      x-api-path-slug: projectsproject-idstoriesstory-idtasks-get
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
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
    post:
      summary: Post Projects Project Stories Story Tasks
      description: Post projects project stories story tasks.
      operationId: postProjectsProjectStoriesStoryTasks
      x-api-path-slug: projectsproject-idstoriesstory-idtasks-post
      parameters:
      - in: path
        name: PROJECT_ID
        description: The ID of the project
      - in: path
        name: STORY_ID
        description: The ID of the story
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
---