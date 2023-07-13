---
title: /carts/:id
position_number: 1.3
type: get
description: Get a Product
parameters:
  - name:
    content:
content_markdown: |-
  Returns a specific product from your collection
left_code_blocks:
  - code_block: |-
      fetch("http://127.0.0.1:3000/carts/30")
      .then((res) => res.json())
      .then((data) => {
        return data
      })
    title: React
    language: javascript
right_code_blocks:
  - code_block: |2-
      {
        "id": 30,
        "name": "coat",
        "category": "coats",
        "description": "leather coat"
        "price": 50,
        
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