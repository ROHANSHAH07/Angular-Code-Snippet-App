# Code Snippet App

This is an Angular application for displaying and copying code snippets. It uses a JSON server to simulate a backend.

## Features

- Fetches code snippets from a JSON server.
- Displays the title and code for each snippet.
- Allows users to copy code to the clipboard.

## Prerequisites

- Node.js and npm installed on your system.
- Angular CLI installed globally:
  ```bash
  npm install -g @angular/cli
  ```
- JSON Server installed globally:
  ```bash
  npm install -g json-server
  ```

## Setup Instructions

1. Clone this repository or create a new Angular app:

   ```bash
   ng new code-snippet-app
   cd code-snippet-app
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Start the JSON Server:

   - Create a `db.json` file with the following content:
     ```json
     {
       "snippets": [
         {
           "id": 1,
           "title": "Hello World",
           "code": "console.log('Hello, World!');"
         },
         {
           "id": 2,
           "title": "Add Numbers",
           "code": "function add(a, b) { return a + b; }"
         }
       ]
     }
     ```
   - Run the server:
     ```bash
     json-server --watch db.json
     ```
   - The server will run at `http://localhost:3000`.

4. Run the Angular app:

   ```bash
   ng serve
   ```

5. Open the app in your browser at `http://localhost:4200`.

## How to Use

- The app fetches snippets from the JSON server.
- Click on the copy icon next to a snippet to copy it to your clipboard.

## Scripts

- `ng serve`: Run the Angular development server.
- `json-server --watch db.json`: Start the JSON server.

## Dependencies

- Angular CLI
- JSON Server

## Author

Your Name
