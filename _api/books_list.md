---
title: /carts
position_number: 1.0
type: get
description: List all products
parameters:
  - name: 
    content: 
  - name: 
    content: 
content_markdown: |-
  

  Lists all the products you have access to. 
left_code_blocks:
  - code_block: |-
      fetch("http://127.0.0.1:3000/carts")
      .then((res) => res.json())
      .then((data) => {
        return data
      });
    title: React
    language: javascript
  -
right_code_blocks:
  - code_block: |2-
      [
        {
          "id": 41,
        "image": "https://images.unsplash.com/photo-1484327973588-c31f829103fe?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=873&q=80",
        "name": "Mini coat",
        "category": null,
        "description": "A white mini coat with a brown belt",
        "price": 30
        },        
      ]
    title: Response
    language: json
  - code_block: |2-
      {
        "error": true,
        "message": "Invalid url"
      }
    title: Error
    language: json
---