---
title: Errors
position_number: 3
parameters:
  - name:
    content:
content_markdown: |-
  | Code | Name | Description |
  | --- | --- | --- |
  | 200 | OK | Success |
  | 201 | Created | Creation Successful |
  | 400 | Bad Request | We could not process that action |
  | 403 | Forbidden | We couldn't authenticate you |
  | 202 | Accepted | Accept for processing |
  | 401 | Unauthorized | Require user authentication |

  All errors will return JSON in the following format:
left_code_blocks:
  - code_block: |-
      {
        "error": true,
        "message": "error message here"
      }
    title: Response
    language: json
right_code_blocks:
  - code_block:
    title:
    language:
---
