---
title: /movies/:id
position_number: 1.3
type: get
description: Get Movie
parameters:
  - name:
    content:
content_markdown: |-
  Returns a specific movie from your collection
left_code_blocks:
  - code_block: |-
      $.get("http://api.myapp.com/movies/3", {
        token: "YOUR_APP_KEY",
      }, function(data) {
        alert(data);
      });
    title: jQuery
    language: javascript
right_code_blocks:
  - code_block: |2-
      {
        "id": 3,
        "title": "Match Point",
        "score": 4.3,
        "dateAdded": "5/1/2015"
      }
    title: Response
    language: json
  - code_block: |2-
      {
        "error": true,
        "message": "Movie doesn't exist"
      }
    title: Error
    language: json
---
