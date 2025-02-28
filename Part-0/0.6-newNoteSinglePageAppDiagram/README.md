# [{() => fs} Fullstack Open Part 0](https://fullstackopen.com/en/part0/fundamentals_of_web_apps)

# 0.6 New note in Single page app diagram
Create a diagram depicting the situation where the user creates a new note using the single-page version of the app.

```mermaid
sequenceDiagram
participant browser
participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: Payload that contains the created resource
    deactivate server

    Note right of browser: The browser executes the callback function that renders the notes
```