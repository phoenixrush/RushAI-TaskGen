# RushAI-TaskGen
Project Name: RushAI TaskGen

Description:
RushAI TaskGen is a small developer productivity tool that uses generative AI to turn a natural language goal (e.g., “Launch a landing page for my business in 2 weeks”) into a structured task list organized into Kanban-style statuses: To Do, In Progress, and Done.

The program demonstrates how a software engineer can use generative AI to:

Generate Bash commands and regex patterns to automate setup and validation

Generate efficient database queries for storing and retrieving tasks

Generate classes and unit tests from requirements

Refactor existing code for readability and maintainability

Core Flow:

User inputs a goal or project description.

The program calls an AI helper (e.g., OpenAI / other LLM) via a TaskGenAI class to generate:

Task titles

Priorities

Suggested order / dependencies

Tasks are stored in a simple SQLite database and represented as objects (Task, KanbanBoard).

User can list tasks by status (To Do / In Progress / Done) and update status as they work.

Unit tests validate the core logic (creating tasks, updating status, validation, etc.), and some of the tests are AI-generated.
