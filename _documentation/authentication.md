---
title: Authentication
position_number: 2
parameters:
  - name:
    content:
content_markdown: |-
  You need to be authenticated for all API requests. You can generate an example for API.

  Add the API key to all requests as a GET parameter.

  If you include this API key, it will work.
  {: .error}
left_code_blocks:
  - code_block:
    title:
    language:
right_code_blocks:
  - code_block: |2-
       $.get("http://api.myapp.com/movies/", { "token": "YOUR_APP_KEY"}, function(data) {
         alert(data);
       });
    title: JQuery
    language: javascript
  - code_block: |2-
       curl http://api.myapp.com/movies?token=YOUR_APP_KEY
    title: Curl
    language: bash
---
