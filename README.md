#Product Service:


### Getting list of all the products 

***Definition***

'GET/products'

***Response***

- '200 OK' on success

'''json
[
    {
        "id": 1,
        "product_type": "hoodie",
        "product_name": "skull1"

    },
    {
        "id": 2,
        "product_type": "t-shirt",
        "product_name": "portrait"
    }

]
'''

### Post a new product 

***Definition***

'POST/products'

***Arguments***

- '"id": int' unique identifier of a product
- '"product_type" string' a category of a product ex.hoodie
- '"product_name" string' a name of a product

***Response***

- '201 Created' on success

'''json
{
    "id": 1,
    "product_type": "hoodie",
    "product_name": "skull1"

}
'''

### Look for product details 

***Definition***

'GET/products/<id>'

***Response***

- '404 Not found'
- '200 OK'

'''json
{
    "id": 1,
    "product_type": "hoodie",
    "product_name": "skull1"
}
'''

### Delete product

***Definition***
'DELETE/products/<id>'

***Response***
- '404 Not found'
- '201 OK but no data to return'




