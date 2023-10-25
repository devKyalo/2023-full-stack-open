```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new-note-spa
    activate server
    server-->>browser: HTML document
    deactivate server
    Note right of browser: The POST request to the address new_note_spa contains the new note as JSON data containing both the content and date
```