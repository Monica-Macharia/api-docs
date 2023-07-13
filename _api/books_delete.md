---
title: /carts/:id
position_number: 1.5
type: delete
description: Deletes a product
parameters:
  - name:
    content:
content_markdown: |-
  Deletes a product in your collection.
left_code_blocks:
  - code_block: |-
      fetch(http://127.0.0.1:3000/carts/30, {
        method: "DELETE",
        headers: {
          "Content-Type": "application/json",
        },
      });
    title: React
    language: javascript
right_code_blocks:
  - code_block: |2-
      {
        
      }
    title: Response
    language: json
  - code_block: |2-
      {
        "error": true,
        "message": "Product doesn't exist"
      }
    title: Error
    language: json
---

