browser->server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note
server-->browser: status code 302
browser->server: HTTP POST https://studies.cs.helsinki.fi/exampleapp/new_note location
server-->browser: /notes
note over browser:
browser reloads the Notes page
causes three more HTTP requests
end note
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.css
server-->browser: main.css
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js
server-->browser: main.js
browser->server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/main.js
server-->browser: data.json

note over browser:
that renders notes to display
end note