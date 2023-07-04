# 0.6: New note in Single page app diagram

## A diagram depicting the situation where the user creates a new note using the single-page version of the app.

```mermaid
sequenceDiagram

    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: POST REQUEST
    deactivate server

    Note right of browser: The browser starts executing the JavaScript code that fetches the JSON from the server.

    Note right of browser: The browser stays on the same page, and it sends no further HTTP requests.

```
