---
title: Errors
position_number: 3
parameters:
  - name:
    content:
content_markdown: |-
  | Code | Name | Description |
  | --- | --- | --- |
  | 400 | Bad Request | Requested operation not sucessful |
  | 400 | Invalid Body | The request format must be in JSON format |
  | 404 | Not Found| Resource not found |

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