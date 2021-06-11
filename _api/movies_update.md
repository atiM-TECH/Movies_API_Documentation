---
title: /movies/:id
position_number: 1.4
type: put
description: Update movie
parameters:
  - name: title
    content: The title for the movie
  - name: score
    content: The movie's score between 0 and 10
content_markdown: |-
  Update an existing movie in your collection.
left_code_blocks:
  - code_block: |-
      $.ajax({
        "url": "http://api.myapp.com/movies/3",
        "type": "PUT",
        "data": {
          "token": "YOUR_APP_KEY",
          "score": 5.0,
          "title": "Joker"
        },
        "success": function(data) {
          alert(data);
        }
      });
    title: jQuery
    language: javascript
right_code_blocks:
  - code_block: |2-
      {
        "id": 3,
        "title": "Joker",
        "score": 5,
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
