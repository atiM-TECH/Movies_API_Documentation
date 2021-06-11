---
title: /movies/:id
position_number: 1.5
type: delete
description: Deletes a movie
parameters:
  - name:
    content:
content_markdown: |-
  Deletes a movie in your collection.
left_code_blocks:
  - code_block: |-
      $.ajax({
        "url": "http://api.myapp.com/movies/3",
        "type": "DELETE",
        "data": {
          "token": "YOUR_APP_KEY"
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
        "status": "deleted"
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
