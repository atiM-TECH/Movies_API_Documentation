---
title: /movies
position_number: 1.1
type: post
description: Create Movie
parameters:
  - name: title
    content: The title for the movie
  - name: score
    content: The movie's score between 0 and 10
content_markdown: |-
  The movie will automatically be added to your list
  {: .success}

  Adds a movie to your collection.
left_code_blocks:
  - code_block: |-
      $.post("http://api.myapp.com/movies/", {
        "token": "YOUR_APP_KEY",
        "title": "Match Point",
        "score": 4.3
      }, function(data) {
        alert(data);
      });
    title: jQuery
    language: javascript
right_code_blocks:
  - code_block: |-
      {
        "id": 3,
        "title": "Match Point",
        "score": 4.3,
        "dateAdded": "5/1/2015"
      }
    title: Response
    language: json
  - code_block: |-
      {
        "error": true,
        "message": "Invalid score"
      }
    title: Error
    language: json
---
