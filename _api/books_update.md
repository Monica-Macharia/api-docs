---
title: /carts/:id
position_number: 1.4
type: put
description: Update a product
parameters:
  - name: image
    content: The image of the product
  - name: name
    content: The name of the product
  - name: category
    content: The category of the product
  - name: description
    content: The description of the product
  - name: price
    content: The price of the product
content_markdown: |-
  Update an existing product in your collection.
left_code_blocks:
  - code_block: |-
      $fetch("http://127.0.0.1:3000/carts/30", {
        method: 'PUT',
        headers:{
          'Content-Type':'application/json',
        },
        body: JSON.stringify({
          image: "http://unsplash.com",
          name: "dress",
          category: "dresses"
          description:"leather dress",
          price: 400          
        }),
      });
    title: React
    language: javascript
right_code_blocks:
  - code_block: |2-
      {
        "id": 30,
        "image": "http://unsplash.com",
        "name": "dress",
        "category": "dresses",
        "description": "leather dress"
        "price": 400,        
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