# BIGLYDROPSHIP API Documentation

##  Generating Token 

To import the dropship products in your website , you need to generate access token.

Access Token is generated to sync the products and to make sure the user is authorized.

**API** `http://www.dropship.biglytech.net/api/oauth/token`

**Method** : POST

### Request :

_Example_

```


  {
    "client_id"         :  1,
    "username"          :  "YourRegisterdEmailId",
    "client_secret"     :  "R0nc1QWmgM5sTrNoweovpOVWrA5Uf5LYp6sBCX80",
    "password"          : "your dropship password"

  }
```


### Response :


_Example_

```

{
    "token_type"        : "Bearer",
    "expires_in"        : 31535999,
    "access_token"  : "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiImp0aSI6IjgxMz",
    "refresh_token" : "def502006e0e3f4158d302d733"
}
```



## Sync Products

After generating Access Token , Sync the products to your website by hitting the API .

**API** `http://www.dropship.biglytech.net/api/sync`

**Method** : GET

### Response :

_Example_

```

{
    "categories": [
        {
            "id"            : 1,
            "name"      : "Rippin-Lebsack",
            "description"       : "",
            "meta_title"        : "",
            "meta_des"      : "",
            "meta_keywords" : "",
            "slug"          : "",
            "parent_id"     : null,
            "status"        : 1,
            "action"        : "create",
            "synced"        : null
        }
    ],
    "products"  : 
  [
    {
    "id": 1183,
    "name": "New Stylish Sporty Pulse Heart fan",
    "slug": "",
    "bdpin": "",
    "brand_id": 14,
    "model": "80855664A",
    "sku": "80855664A",
    "description": "Chronograph (Stopwatch) with split lap time for recording exercise time, Built-in sensor (sense finger prints)Pulse Sensor provides accurate heart rate requiring NO chest strap, Exercise Intensity input for Calories analyzing, Display current Time &amp; Calendar with Alarm and Hourly Chime function",
    "specification": "Built-in sensor (sense finger prints) Pulse Sensor provides accurate heart rate requiring NO chest strap",
    "weight": "66.00",
    "length": "77.00",
    "width": "99.00",
    "height": "88.00",
    "amount": "849.00",
    "quantity": 95,
    "status": 1,
    "source": "bigly",
    "source_id": null,
    "created_at": "2017-12-21 10:04:01",
    "updated_at": "2018-03-01 11:13:43",
    "min_price": "849.00",
    "max_price": "849.00",
    "shipping_charge": "100.00",
    "action": "create",
    "brand_name": "Importikah",
    "brand": {
      "id": 14,
      "name": "Importikah"
    },
    "categories": [
      {
        "id": 53,
        "name": "Health & Personal Care",
        "description": "",
        "meta_title": "",
        "meta_des": "",
        "meta_keywords": "",
        "slug": "",
        "parent_id": null,
        "status": 1
      }
    ],
    "media": [
      {
        "id": 447,
        "mime": "image/jpeg",
        "thumb": "media/thumb/1515233713-1c89fabbb2f430d57016b71ce56cf296-cute-baby-girl-clothes-cute-baby-outfits.jpg",
        "small": "media/small/1515233713-1c89fabbb2f430d57016b71ce56cf296-cute-baby-girl-clothes-cute-baby-outfits.jpg",
        "medium": "media/medium/1515233713-1c89fabbb2f430d57016b71ce56cf296-cute-baby-girl-clothes-cute-baby-outfits.jpg",
        "large": "http://localhost:8000/media/large/1515233713-1c89fabbb2f430d57016b71ce56cf296-cute-baby-girl-clothes-cute-baby-outfits.jpg",
        "caption": null,
        "default": 0,
        "check": "pending"
      },
      {
        "id": 448,
        "mime": "image/jpeg",
        "thumb": "media/thumb/1515233714-3d-clothes-model-free-download-kimonostyle-dress.jpg",
        "small": "media/small/1515233714-3d-clothes-model-free-download-kimonostyle-dress.jpg",
        "medium": "media/medium/1515233714-3d-clothes-model-free-download-kimonostyle-dress.jpg",
        "large": "http://localhost:8000/media/large/1515233714-3d-clothes-model-free-download-kimonostyle-dress.jpg",
        "caption": null,
        "default": 0,
        "check": "pending"
      },
      {
        "id": 449,
        "mime": "image/jpeg",
        "thumb": "media/thumb/1515233714-c1.jpeg",
        "small": "media/small/1515233714-c1.jpeg",
        "medium": "media/medium/1515233714-c1.jpeg",
        "large": "http://localhost:8000/media/large/1515233714-c1.jpeg",
        "caption": null,
        "default": 0,
        "check": "pending"
      },
      {
        "id": 450,
        "mime": "image/jpeg",
        "thumb": "media/thumb/1515233715-img-9519.jpg",
        "small": "media/small/1515233715-img-9519.jpg",
        "medium": "media/medium/1515233715-img-9519.jpg",
        "large": "http://localhost:8000/media/large/1515233715-img-9519.jpg",
        "caption": null,
        "default": 0,
        "check": "pending"
      }
    ],
    "attributes": [
      {
        "id": 1,
        "name": "Color",
        "pivot": {
          "product_id": 1183,
          "attribute_id": 1,
          "value": "red",
          "id": 8
        }
      }
    ]
  ]
}
```


## Orders

You can create an Order by requesting order id . 

**API** `http://www.dropship.biglytech.net/api/orders`

**Method** : POST

### Request :

_Example_

```

{
    "body" : {
        [
            "name": "Order_Key",
            "customer_id" : Billing_Id,
            "amount" : Total_Amount,
            "customer_note" : "Customer_Note",
            "shipping" : Shipping_Price,
            "billing" : Billing_Price,
            "products" : {
                [
                    "id" : Product_id,
                    "name" : "Product_Name",
                    "amount" : Amount,
                    "quantity" : Quantity,
                ],
            },
            "payment_method" : "cod/prepaid",
            "status" : "Placed/Completed/Dispatched/Shipped/Delivered"
        ]
    }
}
```


### Response : 

_Example_

```

{
  "order_id" : Order_Id 
}
```


I appreciate your feedback. If you find any issues you can contact on  +91-9718121389 .

## Thankyou

