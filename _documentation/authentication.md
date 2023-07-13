---
title: Authentication
position_number: 2
parameters:
  - name:
    content:
content_markdown: |-
  This is a public API and does not require a key to access requests.
  
left_code_blocks:
  - code_block:
    title:
    language:
right_code_blocks:
  - code_block: |2-
       $.get("http://api.myapp.com/books/", { "token": "YOUR_APP_KEY"}, function(data) {
         alert(data);
       });
    title: JQuery
    language: javascript
  - code_block: |2-
       curl http://api.myapp.com/books?token=YOUR_APP_KEY
    title: Curl
    language: bash
---