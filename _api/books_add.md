---
title: /carts
position_number: 1.1
type: post
description: Create a new product
parameters:
  - name: image
    content: The image of the product
  - name: name
    content: The name of the product
  - name: description
    content: A short descrition of the product
  - name: price
    content: The price of the product
  - name: category
    content: The category of the product
  
  
content_markdown: |-
  The product will automatically be added to your product list
  {: .success}

  Adds a product to your collection.

 
left_code_blocks:
  - code_block: |-
      fetch("http://127.0.0.1:3000/carts", {
        method: 'POST',
        headers:{
          'Content-Type':'application/json',
        },
        body: JSON.stringify({
          image: "http://unsplash.com",
          name: "coat",
          category: "coats"
          description:"leather coat",
          price: 50,
          
        }),
      });
       
    title: React
    language: javascript
right_code_blocks:
  - code_block: |-
      {
        "id": 30,
        "image": "http://unsplash.com",
        "name": "coat",
        "category": "coats",
        "description": "leather coat",
        "price": "coat"
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


