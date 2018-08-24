# BIGLYDROPSHIP API Documentation


# Contents
    1. Register
    2. Get Access Token
    3. Check through the access token 
    4. Get all the products in pagination . Per page 15 products
    5. Get Specific Product 
    6. To Delete the Product
    7. Update the Product
    8. Search the product through name and sku
    9. Add Product to Wishlist / Delete from WishList
    10. To Get all the orders
    11. To Order any product
    12. Add to cart API
    13. Delete product from Cart
    14. View All Cart Items of user
    15. Store Cart User Address
    16. Add Billing and Shiping Details  
    17. To View Users Billing and Shipping Address
    18. Update Shipping Address
    19. Delete Shipping Address
    20. Create order
    21. Contact Us
    22. My Orders
    23. Order Details
    24. Get Cancel Reasons
    25. Cancel Order
    26. My Profile
    27. Edit Profile
    28. Update Profile
    29. My WishLists
    30. Get Faqs
    31. Update Faqs
    32. Get all Notifications
    33. Check Profile Api
    34. View Bank Details of user
    35. Insert or Update Bank Details
    36. View Particular Query and its replies
    37. Reply on a query
    38. Get Setting Notification
    39. Update Notification Setting








##  Register through facebook (POST)

**API** `http://localhost:8000/api/login/fb`

**Method** : POST

### Request :

_Example_

```


{
    "access_token" : "EAAF6lwZAdOz8BAGf633RL6ZBEzBwJIaTm75mFQGZAyKM4uCN9BzVjnVrYtYLZB2J71YpJBjTqVN21xZBwddCHCAJgIfPq7qbePEE3CoW11K7k1oE6RIqLzoYYtKZAbzFCQx6291xqYzckQDWMSSAZAGO0mlUfsDgZCkP1SB8PqgQH1UeMSzIp9tPjoMbZBPZAQdHWP3sLsJEqLOK1zT3lP6wm2e7ysyZCYy6WsZD",
    "device_token" : "f5L9LXL2aOg:APA91bHfQaTRgzVjMWKUwQMdgNOiy96DA-C-4RXiFqT3DvWgsdPG6sIE_ZQccuJ04yz_9rFMZf4yAkX2lEX2n3FE7A0QPyTMbcwgwiGto4C5Qyj6GLBF3uuEJiEW86yWHl51YMMxLrkq",
    "device_type" : "ANDROID"
}

```


### Response :


_Example_

```
{
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6IjI3ODI5MDk4NDg4YzYxODIyZTM2ZTUzOGExMjBlMWI1OWJhNjVhMGIxMTBjODVlMmQ5OGNmNTY0NDUxNDJjNTJmNWNhZjkzMzk2OTA5MjIxIn0.eyJhdWQiOiIyNDYiLCJqdGkiOiIyNzgyOTA5ODQ4OGM2MTgyMmUzNmU1MzhhMTIwZTFiNTliYTY1YTBiMTEwYzg1ZTJkOThjZjU2NDQ1MTQyYzUyZjVjYWY5MzM5NjkwOTIyMSIsImlhdCI6MTUyODU0OTA0NiwibmJmIjoxNTI4NTQ5MDQ2LCJleHAiOjE1NjAwODUwNDYsInN1YiI6Ijk4OSIsInNjb3BlcyI6W119.Juftuv0kvw662XsR-8LEgx4ixlRmovy837YIg61i2vLHxumjb0JZ7lYNdMl_ktXHhzZBQB3wITDzDcBC8Awjv_MxkfcJ79UULX7FSRRBuKo5K0_pVFdjQmWPK9VSRA24TBc3upTnbzL_9Gj6lhxtrFma7DscBh_HGBFRYUskJl4H-3MJJ9JvCWFNjdjrHBiGNDXmSixzUlGZsO652PtpgY81TBXqOJ3yb1LrLZYyl5jDMXWWI3KfPKsCZSJWiyxowqNpYBYMa48-jCcqYPhbzaMORllWmgK5v2FLvLiJuQpXoZaUJ25k-MTljTuA0zt2cuAWot0a0PNIusDc6MoY8yBK16wRIA_mz5i4ZgkuPWdYtGC3oquSwwbTQ7gjeD0s2KMW5uGh-4P9HcDDMrNTdSgSj-CvwxNsfmXrbmQaEJCQieCr6gXHVfyo3oXVSjcnxhNbNUwj9-FEpLpPPfxfOw8Qj1woDNV-FRD89OQtH6sdbcXM0-akfyQT_sEJzjjHHZsd4_55pAk2nonLLFLJ8xxY0IPwPt0j0m5l3kDbBZvca2OEBPWUGs3GrIciDLltmTkcbg46_OHUrULBZ5spyK8IQZCGtwKb2f4HoG33PeU3yOZnYr0pJ2eDi8c3TMtQghGN_v-tjSj2zYo0nRF0hZvMxY16pA53S36iC3pbObg",
    "user": {
        "id": 989,
        "name": "Gunjan Kumar",
        "username": null,
        "email": "1618242761564460@facebook.com",
        "status": 1,
        "phone": "9039541384",
        "created_at": "May 24, 2018",
        "updated_at": "2018-06-09 18:26:50",
        "type": "client",
        "data": [
            {
                "user_id": 989,
                "name": "facebook.id",
                "value": "1618242761564460"
            },
            {
                "user_id": 989,
                "name": "tokens.fcm",
                "value": "f5L9LXL2aOg:APA91bHfQaTRgzVjMWKUwQMdgNOiy96DA-C-4RXiFqT3DvWgsdPG6sIE_ZQccuJ04yz_9rFMZf4yAkX2lEX2n3FE7A0QPyTMbcwgwiGto4C5Qyj6GLBF3uuEJiEW86yWHl51YMMxLrkq"
            },
            {
                "user_id": 989,
                "name": "tokens.fcm",
                "value": "f5L9LXL2aOg:APA91bHfQaTRgzVjMWKUwQMdgNOiy96DA-C-4RXiFqT3DvWgsdPG6sIE_ZQccuJ04yz_9rFMZf4yAkX2lEX2n3FE7A0QPyTMbcwgwiGto4C5Qyj6GLBF3uuEJiEW86yWHl51YMMxLrkq"
            },
            {
                "user_id": 989,
                "name": "tour",
                "value": "/dashboard,/orders,/products/import,/products/_,/products/_,/profile/company-information,/profile/bank-information,/orders/create,/products/_,/products,/products/_,/products/_,/products/_,/,/,/notification,/products/_,/products/_,/,/products/_"
            },
            {
                "user_id": 989,
                "name": "app_user",
                "value": "1"
            },
            {
                "user_id": 989,
                "name": "otp",
                "value": "4359"
            }
        ]
    },
    "mobile": 1
}

```
## Verify facebook mobile if mobile value is 0(POST)
**API** `http://localhost:8000/api/login/fb/mobile`

**Method** : POST

### Request :

_Example_

####Pass bearer access  token as header input(mandatory)

```
{
    "phone" : 9039541384
}
```
###Response : 

```
{
    "user": {
        "id": 989,
        "name": "Gunjan Kumar",
        "username": null,
        "email": "1618242761564460@facebook.com",
        "status": 1,
        "phone": "9039541384",
        "created_at": "May 24, 2018",
        "updated_at": "2018-06-09 18:26:50",
        "type": "client",
        "data": [
            {
                "user_id": 989,
                "name": "facebook.id",
                "value": "1618242761564460"
            },
            {
                "user_id": 989,
                "name": "tokens.fcm",
                "value": "f5L9LXL2aOg:APA91bHfQaTRgzVjMWKUwQMdgNOiy96DA-C-4RXiFqT3DvWgsdPG6sIE_ZQccuJ04yz_9rFMZf4yAkX2lEX2n3FE7A0QPyTMbcwgwiGto4C5Qyj6GLBF3uuEJiEW86yWHl51YMMxLrkq"
            },
            {
                "user_id": 989,
                "name": "tokens.fcm",
                "value": "f5L9LXL2aOg:APA91bHfQaTRgzVjMWKUwQMdgNOiy96DA-C-4RXiFqT3DvWgsdPG6sIE_ZQccuJ04yz_9rFMZf4yAkX2lEX2n3FE7A0QPyTMbcwgwiGto4C5Qyj6GLBF3uuEJiEW86yWHl51YMMxLrkq"
            },
            {
                "user_id": 989,
                "name": "tour",
                "value": "/dashboard,/orders,/products/import,/products/_,/products/_,/profile/company-information,/profile/bank-information,/orders/create,/products/_,/products,/products/_,/products/_,/products/_,/,/,/notification,/products/_,/products/_,/,/products/_"
            },
            {
                "user_id": 989,
                "name": "app_user",
                "value": "1"
            },
            {
                "user_id": 989,
                "name": "otp",
                "value": "4359"
            }
        ]
    },
    "otp": 2266
}
```

## Verify Otp (POST)

**API** `http://localhost:8000/api/verify`

**Method** : POST

### Request :

_Example_
```
{
    "otp" : 4359
}
```

###Response

```
{
    "status": "success"
}
```



## Register through Mobile Phone (Post)

**API** `http://localhost:8000/api/login/phone`

**Method** : POST

### Request :

_Example_
```
{
    "phone" : 7898888758,
    "device_token" : "f5L9LXL2aOg:APA91bHfQaTRgzVjMWKUwQMdgNOiy96DA-C-4RXiFqT3DvWgsdPG6sIE_ZQccuJ04yz_9rFMZf4yAkX2lEX2n3FE7A0QPyTMbcwgwiGto4C5Qyj6GLBF3uuEJiEW86yWHl51YMMxLrkq",
    "device_type" : "ANDROID"
}
```

###Response

```
{
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6ImVhYjg1NDNhMzcwMTFjZTQzOTRhNzhkZjU2MmUxNGJjYTk3YTg4MDQ3ZThhZTgzMjcxMjA2MzgyZTAwNDg0ZGJiYWMxM2IzZGY0NmQxMGJmIn0.eyJhdWQiOiIyNDYiLCJqdGkiOiJlYWI4NTQzYTM3MDExY2U0Mzk0YTc4ZGY1NjJlMTRiY2E5N2E4ODA0N2U4YWU4MzI3MTIwNjM4MmUwMDQ4NGRiYmFjMTNiM2RmNDZkMTBiZiIsImlhdCI6MTUyODU1MTAyNywibmJmIjoxNTI4NTUxMDI3LCJleHAiOjE1NjAwODcwMjcsInN1YiI6IjEwMTgiLCJzY29wZXMiOltdfQ.aIN6qkNWnhNWv0Kf4aO-Wl_lwJpQD5EuaWYYnx4iAc5cAPquQvuOqIfUQz1GCgsJ4F1r2WkCtCWzpF7PYLdkVvhoHLxWmruwaFU-2AtbBPD7pHQU7vqyuClmiQhwPT9V-Eza60JNMdGLd0KEuItezXEq-sA9uLAA-0sJZHyHfM7aQ4iL_JpzZPn-NF_R_uZnqgYsEWtO84MWv5nCV-vYiqo0GYmtwr67AVkVi_xORKEyxsMyAQRVTCWbVFOx9mRT-a7K97EZ64d8tJvtx-ikaD3tLTddXW0qGWh9ggsh3dJc5zQeYbstQdpOyIOW5PCx_39NZ8EApUNDp_7uc1Nd85c_ugqpfubU8TVdujRbEMzrzrh6fjLa4bLttIip_k-QkqbBb5JFTsBlG_wVWU9tncV5AxSu3ERjdhlIJ5xphJ_-eAhmddTqxtBhS0A6Pg_I5FZd1ljyZiyk9WEZi27OQNVYFyVKo_W9aIEwPmxjT1zGZvaMgO2wYy4y0zhmQIznvtIDbQVv9O6ozeTn3s5SIQxREf-GZx-W0WrOj9XklVLESQ7kdO4tFVdYkJKwHcdaMrQWCA8i5XAuUEfgaL9pxzYVGD2_ciFqrYEDCl1lR89MzVW5Sm3H4wvskQrCt2RxwNDsJAQ8TJYdEDzKwOhABjqiciSRZodsBIcCRkCb34k",
    "user": {
        "name": "",
        "email": "9039541384@app.com",
        "type": "client",
        "updated_at": "2018-06-09 19:00:21",
        "created_at": "Jun 09, 2018",
        "id": 1018,
        "data": [
            {
                "user_id": 1018,
                "name": "app_user",
                "value": "1"
            },
            {
                "user_id": 1018,
                "name": "app_user",
                "value": "1"
            },
            {
                "user_id": 1018,
                "name": "tokens.fcm",
                "value": ""
            },
            {
                "user_id": 1018,
                "name": "app_user",
                "value": "1"
            },
            {
                "user_id": 1018,
                "name": "tokens.fcm",
                "value": ""
            },
            {
                "user_id": 1018,
                "name": "otp",
                "value": "4513"
            }
        ]
    },
    "otp": 5997
}
```


<!-- 2 -->

## Get Access Token (POST)

**API** `http://localhost:8000/oauth/token`

**Method** : POST

### Request :

_Example_

```

{
    "grant_type"        : "password",
    "client_id"         :  217,
    "username"          :  "sakshikbc@gmail.com",
    "client_secret"     : "FIK35PvZ4R8DKukpp9dPWNfTVzFUnA7mEAXGoTQh",
    "password"          : "123456"

}

```


### Response :


_Example_

```

{
    "token_type": "Bearer",
    "expires_in": 31536000,
    "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6ImNhNmM5Yjg1ODQxNTM1OTBhZGU2YjEwMDdhYjk2ZTlkNDA3ODM1ZTIwMDUyNjc3NGY4NWY3NGI5NGVjNWQ3MTlhZTY4MTEzMWIyZWI0ZTFjIn0.eyJhdWQiOiIyMTciLCJqdGkiOiJjYTZjOWI4NTg0MTUzNTkwYWRlNmIxMDA3YWI5NmU5ZDQwNzgzNWUyMDA1MjY3NzRmODVmNzRiOTRlYzVkNzE5YWU2ODExMzFiMmViNGUxYyIsImlhdCI6MTUyMzk0NDkxMCwibmJmIjoxNTIzOTQ0OTEwLCJleHAiOjE1NTU0ODA5MTAsInN1YiI6Ijc1OSIsInNjb3BlcyI6W119.TvpWVFQUtWxbgHvVoXhucGPOPv_pdfPX7Um_6pmeAHb3SQHpWPAven9lTfYcRZfwqMjE7BREpUfrlqGYynrmd9Kt-ty7VThlXvxi3HnHex9kN32jXmMxZhfECtx_Qnf3yqD2Enxy8dKkrxQYcKIru5-PA5DVPVLJ5RtvuiDzpMdM6gJf3Q1AT0cifK0GRYvojz7h-AoGdHAFrem_ceYic8kFWvv32JDIIU3mKmGHZGhZhTGK_hC_FsA-WyT7x848335O3onV_qZOuinduzRf9pY-aH61tby7USztzCwEWal_G8gQRaXnk1YTM9bcnklOBz5avbXH-902hqv8PUfBvwjIErOW1ybntO-VgheDEGeVT8d2y03W0U_U1_luoWmkwscL992l2yR_2FYvJ9T-sr19VMUsYJvVrYHcSlFmwfvFCM0dpomOSw1dBGvi0DJ0LeEYpCyAbrMVEtWA2Zgxq02JD8O3yQDv1enatLohweZ0VXtQWeNud32Chg1keRSAOuVHku53VE5JAOe-lx4NIHL3JYKVFkmLEsYMu-8SN7D2xPmG6FWLSAlHy7fafpTWwNlX3GFJz94zk12TMqp1rQVbor0VA74Ux6olxZecbxaCcDbxBZY60kOCeyHtPw9KI5WpSUdRuOajpxI1cJwp2uan_OMziippju-YBRlYrgc",
    "refresh_token": "def502009071e244a1cd030848c50c5b4ff83d166fb153a0c6f455697d11d204537a4210bc650afcdbd22d0235fb5405ade3e69c58713c0c17d4d159107b1c61be2b9a8e043c722447bde73cf72b82391ab2b6d79c34fade3f12c3649e900b8b5368893e0db6932e0e1a62787f21844772a51b81cc36f1327d0ef3a65e563f6b5fe8d7e9878ecb0116f8b3fbd7620267fd1af3305944d008cc5299cdad8a3c87f462dd65ebc889d4a2b3b738c1a947c42da0b40167c210ab91dd3a84f9d830423dc45656314fc3484ab7c33ee07383b93828697e3527305c4e59f59de2f26b071399c571b65c7695a84e5466ef8ffb9d6c9b982ba908758fc82bb0178ac4b49a7bc260ab47707d32751f587d5809a4fda7badf625c9cab1d47c65b4b24eae454e4185f3d97ad453924466ed6bf0fda6e151e3cde75abd721b35a33bbc458ac34ba271a3d162badd9ace4c43e0be45ef9664ca2a0c98acf5e8d4b007357e9d022af7cc4"
}


```

<!-- 3 -->

##  Get the access token 

**API** `http://localhost:8000/api/user`

**Method** : GET

### Header 

```
{
“Authorization” :  “Bearer eyJ0eXAiOiJKV1QiLCJhbGciOiJSUzI1NiIsImp0aSI6IjFkNTkzMTY3ODFkMzczMjY1MWRkNTVmMzNhMWJlNTczNjJhMDU1YWRjNjgyOTI0ODFkNGEwYzhkMDk2ZGYzMjczODJjZTdlMzQ3MDI1MTdhIn0.eyJhdWQiOiIxIiwianRpIjoiMWQ1OTMxNjc4MWQzNzMyNjUxZGQ1NWYzM2ExYmU1NzM2MmEwNTVhZGM2ODI5MjQ4MWQ0YTBjOGQwOTZkZjMyNzM4MmNlN2UzNDcwMjUxN2EiLCJpYXQiOjE1MjM1MDk4ODcsIm5iZiI6MTUyMzUwOTg4NywiZXhwIjoxNTU1MDQ1ODg3LCJzdWIiOiI1MTAiLCJzY29wZXMiOltdfQ.OgZCUJtxeq2RDEkElHGXIjWrA5o18_aD9ST9HFkZeAr_y8qmVtlSQiARN46FAtPqvYj0KIuj8q5Ca1QTB6Uc158TwB-H7CsgO_MadHSBTUdbwCOLCkbZlTvNRAEeq5KzFQGsYdI-FBfymg38k_MA7xlrvvW1QyjxyVEsFtpXNhr_Gv03c8kPIENYTBhTHWY7F4mnfSCPeLSaoKCbawp6SGS-tADaU25js2SY_m8AUsOuPw9-q-kTNEtHMIumYF_qpKBZXDaT7BbQ9XaX-k-BYgtAvm4nH_ApUPHNsLXMGQZzihgv0RSjUYN7TYQEgb411wjB3H1nZlRT9FGwn12lDV5QXxPTzHLAwqf_G9o6ZjkJh30X1SZS2zmSXjqGLWfB7TRcwsLpIn8NR97XJSvuArOey2hmif9BEs4j_weK6zHcc6Z99HhMlIwMQtBYV6tijm5z2CeYAbRTfn8EG8L8HZsuHdZzxUh_vqmRGooqJ80mcNGJ_cq5yJ0uXb7ZVGWbNAcxUBpoAjYYBTCZY20BZEaci8ocqvbp5B-S2o1jxPLyJ3HiGHtn-QSl8yKBYxgTH5ew_OtJZJk657gxfo4dBcxmhHcgbrHLM5hBGi4rqaD10V2CxLEMioyABtMoaCQyiFtMWj3r35J9OmofyZs-UMPE6p2dLv9EKlsYFlMtBMI”
}

```


### Response :


_Example_

```

{
    "id": 510,
    "name": "client",
    "username": null,
    "email": "client@seller.com",
    "status": 1,
    "phone": "1234567890",
    "created_at": "2018-03-03 07:23:29",
    "updated_at": "2018-03-03 07:23:29",
    "type": "client"
}


```


<!-- 4 -->


## Get all the products in pagination . Per page 15 products

**API** `http://localhost:8000/api/products`

`http://localhost:8000/api/products?q=query&category[]=51&vendor[]=514&vendor[]=2&price_range=501-1000`

**Method** : GET

### Response :


_Example_

```

{
    "products": {
        "current_page": 1,
        "data": [
            {
                "id": 1011,
                "user_id": 2,
                "name": "sZEfgfr",
                "slug": "",
                "bdpin": "",
                "brand_id": 9,
                "model": "sdgdsgsd",
                "sku": "sdxg",
                "description": "jhgjhg",
                "specification": "srgsde",
                "weight": "15.00",
                "length": "55.00",
                "width": "55.00",
                "height": "5.00",
                "amount": "21.00",
                "quantity": 533,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-05-02 18:11:59",
                "updated_at": "2018-05-18 12:52:17",
                "min_price": "121.00",
                "max_price": "1200.00",
                "shipping_charge": "2.00",
                "attributes": [
                    {
                        "id": 16,
                        "value": "0000FF",
                        "quantity": null,
                        "price": null,
                        "name": "color",
                        "attr_id": 2,
                        "children": [
                            {
                                "id": 17,
                                "value": "50",
                                "quantity": 20,
                                "price": null,
                                "attr_id": 3,
                                "name": "size"
                            }
                        ]
                    }
                ],
                "isWishlist": true,
                "brand_name": "dsgesdge",
                "organization": {
                    "id": 2,
                    "user_id": 2,
                    "type_id": 0,
                    "name": "Ederno",
                    "logo": "http://s.bigly.io/logo/1520848354-mEbtXPl2agzy9vz.jpg",
                    "gst": "",
                    "incorporation_number": "",
                    "address": "N 21 , Above United Bank of India",
                    "introduction": "",
                    "created_at": "2018-03-01 07:36:47",
                    "updated_at": "2018-03-14 10:14:17",
                    "city": "Satna",
                    "state": "Madhya Pradesh",
                    "pincode": "485001",
                    "country": "India"
                },
                "categories": [],
                "user_product": {
                    "id": 1029,
                    "user_id": 510,
                    "product_id": 1011,
                    "name": null,
                    "amount": null,
                    "created_at": null,
                    "updated_at": null,
                    "description": ""
                },
                "media": [
                    {
                        "id": 4683,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/zkqr1y4lujen9ks-9htf1uw.jpg",
                        "small": "http://s.bigly.io/products/small/zkqr1y4lujen9ks-9htf1uw.jpg",
                        "medium": "http://s.bigly.io/products/medium/zkqr1y4lujen9ks-9htf1uw.jpg",
                        "large": "http://s.bigly.io/products/large/zkqr1y4lujen9ks-9htf1uw.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 1006,
                "user_id": 22,
                "name": "drgyrdy",
                "slug": "",
                "bdpin": "",
                "brand_id": 4,
                "model": "hdxyhd",
                "sku": "gsdrey",
                "description": "15hdxhrdfhj",
                "specification": "hdrfju",
                "weight": "15.00",
                "length": "51.00",
                "width": "515.00",
                "height": "51.00",
                "amount": "30.00",
                "quantity": 10,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-08 11:09:01",
                "updated_at": "2018-03-08 11:09:13",
                "min_price": "40.00",
                "max_price": "100.00",
                "shipping_charge": "10.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "edyrdf",
                "organization": {
                    "id": 9,
                    "user_id": 22,
                    "type_id": 2,
                    "name": "sxegfsdgy",
                    "logo": "",
                    "gst": "gersy",
                    "incorporation_number": "",
                    "address": "esrdyte",
                    "introduction": "grdy",
                    "created_at": "2018-03-08 11:07:22",
                    "updated_at": "2018-03-08 11:09:30",
                    "city": "Satna",
                    "state": "Madhya Pradesh",
                    "pincode": "485001",
                    "country": "India"
                },
                "categories": [
                    {
                        "id": 1,
                        "name": "Torphy-Schimmel",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": {
                    "id": 1014,
                    "user_id": 510,
                    "product_id": 1006,
                    "name": null,
                    "amount": null,
                    "created_at": null,
                    "updated_at": null,
                    "description": ""
                },
                "media": []
            },
            {
                "id": 2,
                "user_id": 2,
                "name": "Wunsch, Kerluke and Kuphal",
                "slug": "",
                "bdpin": "4c9d0997-baed-3284-827c-a0aa81b51bfb",
                "brand_id": null,
                "model": null,
                "sku": "26463d4a-d488-35b8-b61f-84d865a1e943",
                "description": "Alice, in a tone of the door that led into the court, by the hedge!' then silence, and then the puppy began a series of short charges at the March Hare said in an agony of terror. 'Oh, there goes.",
                "specification": "",
                "weight": "1648.00",
                "length": "1464.00",
                "width": "4143.00",
                "height": "4618.00",
                "amount": "68.00",
                "quantity": 16,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:54:50",
                "updated_at": "2018-03-01 10:54:50",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 23,
                        "name": "Ledner-Harber",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 32,
                        "name": "Denesik Group",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 27,
                        "name": "Emmerich-Schultz",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 3,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/technics/3",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/technics/3",
                        "large": "http://lorempixel.com/1280/720/technics/3",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 1008,
                "user_id": 514,
                "name": "deyhrdfyh",
                "slug": "",
                "bdpin": "",
                "brand_id": 6,
                "model": "hdxyhdxg",
                "sku": "dxgdxghdxhx",
                "description": "2 ",
                "specification": "dxryghdcfh",
                "weight": "58.00",
                "length": "23.00",
                "width": "26.00",
                "height": "26.00",
                "amount": "2.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-04-14 06:49:57",
                "updated_at": "2018-04-14 06:49:57",
                "min_price": "2.00",
                "max_price": "1212.00",
                "shipping_charge": "2.00",
                "attributes": [
                    {
                        "id": 8,
                        "value": "0000FF",
                        "quantity": null,
                        "price": null,
                        "name": "color",
                        "attr_id": 2,
                        "children": []
                    }
                ],
                "isWishlist": false,
                "brand_name": "rdxyrhrfthyrdf",
                "organization": {
                    "id": 12,
                    "user_id": 514,
                    "type_id": 0,
                    "name": "bla bla",
                    "logo": "",
                    "gst": "",
                    "incorporation_number": "",
                    "address": "",
                    "introduction": "",
                    "created_at": "2018-03-26 12:22:21",
                    "updated_at": "2018-03-26 12:22:21",
                    "city": "",
                    "state": "",
                    "pincode": "",
                    "country": ""
                },
                "categories": [
                    {
                        "id": 4,
                        "name": "Marquardt-Gleichner",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": []
            },
            {
                "id": 518,
                "user_id": 1,
                "name": "Hilll, Robel and Robel",
                "slug": "",
                "bdpin": "c1f676ee-e4e5-35df-81ff-ae01ce1d6240",
                "brand_id": null,
                "model": null,
                "sku": "815e6927-ac50-3860-bee5-b4119bfdf218",
                "description": "Dormouse,' the Queen merely remarking that a red-hot poker will burn you if you drink much from a bottle marked 'poison,' so Alice soon came upon a time she saw them, they were filled with cupboards.",
                "specification": "",
                "weight": "3075.00",
                "length": "6180.00",
                "width": "1486.00",
                "height": "2193.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:10",
                "updated_at": "2018-03-01 10:55:10",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 27,
                        "name": "Emmerich-Schultz",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 2430,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/fashion/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/fashion/9",
                        "large": "http://lorempixel.com/1280/720/fashion/9",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 2431,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/fashion/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/fashion/9",
                        "large": "http://lorempixel.com/1280/720/fashion/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2432,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nature/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nature/9",
                        "large": "http://lorempixel.com/1280/720/nature/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2433,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nature/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nature/9",
                        "large": "http://lorempixel.com/1280/720/nature/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2434,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/9",
                        "large": "http://lorempixel.com/1280/720/food/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2435,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nightlife/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nightlife/9",
                        "large": "http://lorempixel.com/1280/720/nightlife/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 558,
                "user_id": 1,
                "name": "Ortiz-Deckow",
                "slug": "",
                "bdpin": "df4d2981-4e4d-3158-8fae-650d1d6ec03e",
                "brand_id": null,
                "model": null,
                "sku": "c350c894-a72b-3d29-a420-acdcae752baf",
                "description": "SLUGGARD,\"' said the Pigeon; 'but I know I do!' said Alice very politely; but she heard a little timidly, for she was to eat or drink anything; so I'll just see what was going to say,' said the Mock.",
                "specification": "",
                "weight": "8514.00",
                "length": "9544.00",
                "width": "4807.00",
                "height": "405.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:11",
                "updated_at": "2018-03-01 10:55:11",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 2,
                        "name": "Rodriguez, Moore and Balistreri",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 28,
                        "name": "Lubowitz Group",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 2629,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nightlife/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nightlife/9",
                        "large": "http://lorempixel.com/1280/720/nightlife/9",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 2630,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nightlife/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nightlife/9",
                        "large": "http://lorempixel.com/1280/720/nightlife/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2631,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/transport/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/transport/9",
                        "large": "http://lorempixel.com/1280/720/transport/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2632,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/9",
                        "large": "http://lorempixel.com/1280/720/food/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2633,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/people/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/people/9",
                        "large": "http://lorempixel.com/1280/720/people/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 70,
                "user_id": 1,
                "name": "Aufderhar, Ebert and Lind",
                "slug": "",
                "bdpin": "682f25bd-8112-3397-9078-c73fcf6f16fb",
                "brand_id": null,
                "model": null,
                "sku": "49d45dcc-4460-31f2-b5e3-72a7fab8ff4f",
                "description": "White Rabbit interrupted: 'UNimportant, your Majesty means, of course,' he said to herself how she would keep, through all her coaxing. Hardly knowing what she did, she picked her way into a pig,'.",
                "specification": "",
                "weight": "9471.00",
                "length": "4698.00",
                "width": "3972.00",
                "height": "955.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:54:52",
                "updated_at": "2018-03-01 10:54:52",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 41,
                        "name": "West Inc",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 10,
                        "name": "Ondricka, Sanford and Frami",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 48,
                        "name": "Tremblay-Pollich",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 292,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/fashion/1",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/fashion/1",
                        "large": "http://lorempixel.com/1280/720/fashion/1",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 293,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/business/1",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/business/1",
                        "large": "http://lorempixel.com/1280/720/business/1",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 294,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/transport/1",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/transport/1",
                        "large": "http://lorempixel.com/1280/720/transport/1",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 295,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nature/1",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nature/1",
                        "large": "http://lorempixel.com/1280/720/nature/1",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 296,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/technics/1",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/technics/1",
                        "large": "http://lorempixel.com/1280/720/technics/1",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 297,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nature/1",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nature/1",
                        "large": "http://lorempixel.com/1280/720/nature/1",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 853,
                "user_id": 1,
                "name": "Zieme, Toy and Koss",
                "slug": "",
                "bdpin": "36d8595d-a6e5-3262-a0a6-7bc8a0383c77",
                "brand_id": null,
                "model": null,
                "sku": "021e3bc6-e57e-39e5-8251-ca8b8100e45f",
                "description": "Hatter, and, just as well as she wandered about in a melancholy tone. 'Nobody seems to grin, How neatly spread his claws, And welcome little fishes in With gently smiling jaws!' 'I'm sure those are.",
                "specification": "",
                "weight": "6606.00",
                "length": "9820.00",
                "width": "1038.00",
                "height": "8509.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:23",
                "updated_at": "2018-03-01 10:55:23",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 6,
                        "name": "Maggio Ltd",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 30,
                        "name": "Zieme, McClure and Kling",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 24,
                        "name": "Dicki-Wilkinson",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 3977,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/fashion/4",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/fashion/4",
                        "large": "http://lorempixel.com/1280/720/fashion/4",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 3978,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nightlife/4",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nightlife/4",
                        "large": "http://lorempixel.com/1280/720/nightlife/4",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 3979,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/business/4",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/business/4",
                        "large": "http://lorempixel.com/1280/720/business/4",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 3980,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/fashion/4",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/fashion/4",
                        "large": "http://lorempixel.com/1280/720/fashion/4",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 3981,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/business/4",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/business/4",
                        "large": "http://lorempixel.com/1280/720/business/4",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 605,
                "user_id": 1,
                "name": "Skiles-Pagac",
                "slug": "",
                "bdpin": "f5516865-f210-3c39-8135-a8290e9d3579",
                "brand_id": null,
                "model": null,
                "sku": "ca043d81-e0d4-3e48-b5bd-8d044ee42a9b",
                "description": "Why, I haven't been invited yet.' 'You'll see me there,' said the Gryphon: and Alice looked at poor Alice, and she said this last remark. 'Of course they were', said the March Hare. The Hatter was.",
                "specification": "",
                "weight": "1536.00",
                "length": "8702.00",
                "width": "3703.00",
                "height": "2798.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:13",
                "updated_at": "2018-03-01 10:55:13",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 27,
                        "name": "Emmerich-Schultz",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 35,
                        "name": "Hackett PLC",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 2860,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/technics/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/technics/6",
                        "large": "http://lorempixel.com/1280/720/technics/6",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 2861,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/business/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/business/6",
                        "large": "http://lorempixel.com/1280/720/business/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 948,
                "user_id": 1,
                "name": "Swaniawski-Schimmel",
                "slug": "",
                "bdpin": "c3fff733-b3d4-32bf-b7f2-89e642724e35",
                "brand_id": null,
                "model": null,
                "sku": "9e2a1bb1-fa96-3014-a694-9ea7fbd5b725",
                "description": "Alice in a shrill, passionate voice. 'Would YOU like cats if you could keep it to half-past one as long as I do,' said the White Rabbit hurried by--the frightened Mouse splashed his way through the.",
                "specification": "",
                "weight": "8817.00",
                "length": "2756.00",
                "width": "6722.00",
                "height": "7104.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:27",
                "updated_at": "2018-03-01 10:55:27",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 6,
                        "name": "Maggio Ltd",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 14,
                        "name": "Koepp and Sons",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 4390,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/people/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/people/9",
                        "large": "http://lorempixel.com/1280/720/people/9",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 4391,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/transport/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/transport/9",
                        "large": "http://lorempixel.com/1280/720/transport/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4392,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nature/9",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nature/9",
                        "large": "http://lorempixel.com/1280/720/nature/9",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 457,
                "user_id": 1,
                "name": "Corwin LLC",
                "slug": "",
                "bdpin": "7ab957a1-4eb7-3c8b-916e-0f54c654dee7",
                "brand_id": null,
                "model": null,
                "sku": "e5b80f67-383a-3c70-af48-468dabae35bb",
                "description": "I shall be late!' (when she thought to herself what such an extraordinary ways of living would be so easily offended!' 'You'll get used up.' 'But what did the Dormouse again, so that by the way to.",
                "specification": "",
                "weight": "3675.00",
                "length": "7926.00",
                "width": "1370.00",
                "height": "7825.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:08",
                "updated_at": "2018-03-01 10:55:08",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 44,
                        "name": "Wunsch Inc",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 17,
                        "name": "Denesik-Ondricka",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 2121,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/technics/8",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/technics/8",
                        "large": "http://lorempixel.com/1280/720/technics/8",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 734,
                "user_id": 1,
                "name": "Heidenreich-Bergstrom",
                "slug": "",
                "bdpin": "425eb529-8675-3b2c-9a57-2e437e55ed5a",
                "brand_id": null,
                "model": null,
                "sku": "17e4d9b3-0725-3df4-b74f-bac06c8f049d",
                "description": "I'm a deal faster than it does.' 'Which would NOT be an advantage,' said Alice, whose thoughts were still running on the floor, and a pair of white kid gloves while she was a large cauldron which.",
                "specification": "",
                "weight": "9703.00",
                "length": "753.00",
                "width": "7834.00",
                "height": "2975.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:18",
                "updated_at": "2018-03-01 10:55:18",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 16,
                        "name": "Macejkovic-Bradtke",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 3450,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/5",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/5",
                        "large": "http://lorempixel.com/1280/720/food/5",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 3451,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/5",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/5",
                        "large": "http://lorempixel.com/1280/720/food/5",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 3452,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/transport/5",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/transport/5",
                        "large": "http://lorempixel.com/1280/720/transport/5",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 3453,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/5",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/5",
                        "large": "http://lorempixel.com/1280/720/food/5",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 3454,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/business/5",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/business/5",
                        "large": "http://lorempixel.com/1280/720/business/5",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 495,
                "user_id": 1,
                "name": "Ernser Ltd",
                "slug": "",
                "bdpin": "94c18842-7c84-3b9c-96e0-4e539a314525",
                "brand_id": null,
                "model": null,
                "sku": "6f3747b6-bc5d-3d45-b741-48960b6d58c4",
                "description": "It means much the most confusing thing I ever was at the March Hare. Alice was more hopeless than ever: she sat on, with closed eyes, and half believed herself in a voice sometimes choked with sobs.",
                "specification": "",
                "weight": "3052.00",
                "length": "2462.00",
                "width": "4274.00",
                "height": "813.00",
                "amount": "10.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:09",
                "updated_at": "2018-03-01 10:55:09",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 15,
                        "name": "Lubowitz, Borer and Harvey",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 2314,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/technics/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/technics/6",
                        "large": "http://lorempixel.com/1280/720/technics/6",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 2315,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nightlife/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nightlife/6",
                        "large": "http://lorempixel.com/1280/720/nightlife/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2316,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nightlife/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nightlife/6",
                        "large": "http://lorempixel.com/1280/720/nightlife/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2317,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/6",
                        "large": "http://lorempixel.com/1280/720/food/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2318,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/6",
                        "large": "http://lorempixel.com/1280/720/food/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2319,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/6",
                        "large": "http://lorempixel.com/1280/720/food/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2320,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nature/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nature/6",
                        "large": "http://lorempixel.com/1280/720/nature/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 2321,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/people/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/people/6",
                        "large": "http://lorempixel.com/1280/720/people/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 19,
                "user_id": 1,
                "name": "Walsh-Tremblay",
                "slug": "",
                "bdpin": "be6dfa77-c510-3aa7-a491-59400ac316d5",
                "brand_id": null,
                "model": null,
                "sku": "1b527b67-f35b-3c22-b46b-31071c6f8e4c",
                "description": "And yet I wish I had our Dinah here, I know who I WAS when I was sent for.' 'You ought to be an advantage,' said Alice, 'because I'm not Ada,' she said, by way of keeping up the other, saying, in a.",
                "specification": "",
                "weight": "7186.00",
                "length": "5202.00",
                "width": "1195.00",
                "height": "8243.00",
                "amount": "11.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:54:50",
                "updated_at": "2018-03-01 10:54:50",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 5,
                        "name": "Jacobi-Jakubowski",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 76,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/transport/10",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/transport/10",
                        "large": "http://lorempixel.com/1280/720/transport/10",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 77,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/sports/10",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/sports/10",
                        "large": "http://lorempixel.com/1280/720/sports/10",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 78,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/fashion/10",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/fashion/10",
                        "large": "http://lorempixel.com/1280/720/fashion/10",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 275,
                "user_id": 1,
                "name": "Klein, Pacocha and Goodwin",
                "slug": "",
                "bdpin": "61608489-f887-3a82-ae82-c6c2927101de",
                "brand_id": null,
                "model": null,
                "sku": "0dde4136-caea-3771-bd6d-6a8faf58c383",
                "description": "Mouse had changed his mind, and was beating her violently with its eyelids, so he did,' said the March Hare and the King said to the Dormouse, and repeated her question. 'Why did you call him.",
                "specification": "",
                "weight": "2651.00",
                "length": "3142.00",
                "width": "5753.00",
                "height": "1469.00",
                "amount": "11.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:55:00",
                "updated_at": "2018-03-01 10:55:00",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "isWishlist": false,
                "brand_name": "",
                "organization": null,
                "categories": [
                    {
                        "id": 15,
                        "name": "Lubowitz, Borer and Harvey",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 10,
                        "name": "Ondricka, Sanford and Frami",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 4,
                        "name": "Marquardt-Gleichner",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ],
                "user_product": null,
                "media": [
                    {
                        "id": 1250,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/transport/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/transport/6",
                        "large": "http://lorempixel.com/1280/720/transport/6",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 1251,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/people/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/people/6",
                        "large": "http://lorempixel.com/1280/720/people/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 1252,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/technics/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/technics/6",
                        "large": "http://lorempixel.com/1280/720/technics/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 1253,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/people/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/people/6",
                        "large": "http://lorempixel.com/1280/720/people/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 1254,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/sports/6",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/sports/6",
                        "large": "http://lorempixel.com/1280/720/sports/6",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            }
        ],
        "from": 1,
        "last_page": 67,
        "next_page_url": "http://localhost:8000/api/products?page=2",
        "path": "http://localhost:8000/api/products",
        "per_page": 15,
        "prev_page_url": null,
        "to": 15,
        "total": 1003
    },
    "top_selling_products": [
        {
            "id": 1011,
            "user_id": 2,
            "name": "sZEfgfr",
            "slug": "",
            "bdpin": "",
            "brand_id": 9,
            "model": "sdgdsgsd",
            "sku": "sdxg",
            "description": "jhgjhg",
            "specification": "srgsde",
            "weight": "15.00",
            "length": "55.00",
            "width": "55.00",
            "height": "5.00",
            "amount": "21.00",
            "quantity": 533,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-05-02 18:11:59",
            "updated_at": "2018-05-18 12:52:17",
            "min_price": "121.00",
            "max_price": "1200.00",
            "shipping_charge": "2.00",
            "product_id": 1011,
            "total": 23,
            "attributes": [
                {
                    "id": 16,
                    "value": "0000FF",
                    "quantity": null,
                    "price": null,
                    "name": "color",
                    "attr_id": 2,
                    "children": [
                        {
                            "id": 17,
                            "value": "50",
                            "quantity": 20,
                            "price": null,
                            "attr_id": 3,
                            "name": "size"
                        }
                    ]
                }
            ],
            "isWishlist": true,
            "brand_name": "dsgesdge",
            "organization": {
                "id": 2,
                "user_id": 2,
                "type_id": 0,
                "name": "Ederno",
                "logo": "http://s.bigly.io/logo/1520848354-mEbtXPl2agzy9vz.jpg",
                "gst": "",
                "incorporation_number": "",
                "address": "N 21 , Above United Bank of India",
                "introduction": "",
                "created_at": "2018-03-01 07:36:47",
                "updated_at": "2018-03-14 10:14:17",
                "city": "Satna",
                "state": "Madhya Pradesh",
                "pincode": "485001",
                "country": "India"
            },
            "categories": [],
            "user_product": {
                "id": 1029,
                "user_id": 510,
                "product_id": 1011,
                "name": null,
                "amount": null,
                "created_at": null,
                "updated_at": null,
                "description": ""
            },
            "media": [
                {
                    "id": 4683,
                    "mime": "image/jpeg",
                    "thumb": "http://s.bigly.io/products/thumb/zkqr1y4lujen9ks-9htf1uw.jpg",
                    "small": "http://s.bigly.io/products/small/zkqr1y4lujen9ks-9htf1uw.jpg",
                    "medium": "http://s.bigly.io/products/medium/zkqr1y4lujen9ks-9htf1uw.jpg",
                    "large": "http://s.bigly.io/products/large/zkqr1y4lujen9ks-9htf1uw.jpg",
                    "caption": null,
                    "default": 0,
                    "check": "pending"
                }
            ]
        },
        {
            "id": 1006,
            "user_id": 22,
            "name": "drgyrdy",
            "slug": "",
            "bdpin": "",
            "brand_id": 4,
            "model": "hdxyhd",
            "sku": "gsdrey",
            "description": "15hdxhrdfhj",
            "specification": "hdrfju",
            "weight": "15.00",
            "length": "51.00",
            "width": "515.00",
            "height": "51.00",
            "amount": "30.00",
            "quantity": 10,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-03-08 11:09:01",
            "updated_at": "2018-03-08 11:09:13",
            "min_price": "40.00",
            "max_price": "100.00",
            "shipping_charge": "10.00",
            "product_id": 1006,
            "total": 2,
            "attributes": [],
            "isWishlist": false,
            "brand_name": "edyrdf",
            "organization": {
                "id": 9,
                "user_id": 22,
                "type_id": 2,
                "name": "sxegfsdgy",
                "logo": "",
                "gst": "gersy",
                "incorporation_number": "",
                "address": "esrdyte",
                "introduction": "grdy",
                "created_at": "2018-03-08 11:07:22",
                "updated_at": "2018-03-08 11:09:30",
                "city": "Satna",
                "state": "Madhya Pradesh",
                "pincode": "485001",
                "country": "India"
            },
            "categories": [
                {
                    "id": 1,
                    "name": "Torphy-Schimmel",
                    "description": "",
                    "meta_title": "",
                    "meta_des": "",
                    "meta_keywords": "",
                    "slug": "",
                    "parent_id": null,
                    "status": 1
                }
            ],
            "user_product": {
                "id": 1014,
                "user_id": 510,
                "product_id": 1006,
                "name": null,
                "amount": null,
                "created_at": null,
                "updated_at": null,
                "description": ""
            },
            "media": []
        }
    ],
    "filter": {
        "categories": [
            {
                "name": "Auer-Doyle",
                "id": 26,
                "media": {
                    "id": 71001,
                    "mime": "",
                    "thumb": "http://s.bigly.io/categories/1528375861-3CvrjzDmZUxfR8j.jpg",
                    "small": null,
                    "medium": null,
                    "large": null,
                    "caption": null,
                    "default": 0,
                    "check": "pending"
                }
            },
            {
                "name": "bag",
                "id": 51,
                "media": null
            },
            {
                "name": "Carroll-Runolfsdottir",
                "id": 20,
                "media": null
            },
            {
                "name": "Carroll-Swaniawski",
                "id": 19,
                "media": null
            },
            {
                "name": "Deckow Ltd",
                "id": 25,
                "media": null
            },
            {
                "name": "Denesik Group",
                "id": 32,
                "media": null
            },
            {
                "name": "Denesik-Ondricka",
                "id": 17,
                "media": null
            },
            {
                "name": "Dicki-Wilkinson",
                "id": 24,
                "media": null
            },
            {
                "name": "Emmerich-Schultz",
                "id": 27,
                "media": null
            },
            {
                "name": "Fahey Group",
                "id": 37,
                "media": null
            },
            {
                "name": "Ferry-Larkin",
                "id": 47,
                "media": null
            },
            {
                "name": "Gerlach, Ward and Grimes",
                "id": 21,
                "media": null
            },
            {
                "name": "Glover Group",
                "id": 33,
                "media": null
            },
            {
                "name": "Gutmann-McCullough",
                "id": 39,
                "media": null
            },
            {
                "name": "Hackett PLC",
                "id": 35,
                "media": null
            },
            {
                "name": "Hegmann Ltd",
                "id": 36,
                "media": null
            },
            {
                "name": "Hyatt, Maggio and Russel",
                "id": 31,
                "media": null
            },
            {
                "name": "Jacobi-Jakubowski",
                "id": 5,
                "media": null
            },
            {
                "name": "Johnston-Kuhn",
                "id": 12,
                "media": null
            },
            {
                "name": "Kautzer-Goyette",
                "id": 3,
                "media": null
            },
            {
                "name": "Koepp and Sons",
                "id": 14,
                "media": null
            },
            {
                "name": "Langosh, Jast and Ferry",
                "id": 7,
                "media": null
            },
            {
                "name": "Ledner-Harber",
                "id": 23,
                "media": null
            },
            {
                "name": "Lubowitz Group",
                "id": 28,
                "media": null
            },
            {
                "name": "Lubowitz, Borer and Harvey",
                "id": 15,
                "media": null
            },
            {
                "name": "Lynch, Jast and Osinski",
                "id": 34,
                "media": null
            },
            {
                "name": "Macejkovic-Bradtke",
                "id": 16,
                "media": null
            },
            {
                "name": "Maggio Ltd",
                "id": 6,
                "media": null
            },
            {
                "name": "Marquardt-Gleichner",
                "id": 4,
                "media": null
            },
            {
                "name": "Mills-Kihn",
                "id": 49,
                "media": null
            },
            {
                "name": "Nienow, McClure and Kris",
                "id": 13,
                "media": null
            },
            {
                "name": "Ondricka, Sanford and Frami",
                "id": 10,
                "media": null
            },
            {
                "name": "Reichert PLC",
                "id": 43,
                "media": null
            },
            {
                "name": "Rice PLC",
                "id": 8,
                "media": null
            },
            {
                "name": "Rodriguez, Moore and Balistreri",
                "id": 2,
                "media": null
            },
            {
                "name": "Schowalter, Yost and Fisher",
                "id": 46,
                "media": null
            },
            {
                "name": "Senger and Sons",
                "id": 29,
                "media": null
            },
            {
                "name": "Simonis PLC",
                "id": 50,
                "media": null
            },
            {
                "name": "Spencer Group",
                "id": 42,
                "media": null
            },
            {
                "name": "Stracke PLC",
                "id": 11,
                "media": null
            },
            {
                "name": "Stracke, Fadel and Rau",
                "id": 40,
                "media": null
            },
            {
                "name": "Thiel Group",
                "id": 22,
                "media": null
            },
            {
                "name": "Torphy-Schimmel",
                "id": 1,
                "media": null
            },
            {
                "name": "Tremblay-Pollich",
                "id": 48,
                "media": null
            },
            {
                "name": "West Inc",
                "id": 41,
                "media": null
            },
            {
                "name": "White, Boyer and Kuhlman",
                "id": 9,
                "media": null
            },
            {
                "name": "Wiza-Doyle",
                "id": 18,
                "media": null
            },
            {
                "name": "Wunsch Inc",
                "id": 44,
                "media": null
            },
            {
                "name": "Wunsch-Waters",
                "id": 45,
                "media": null
            },
            {
                "name": "Zieme, McClure and Kling",
                "id": 30,
                "media": null
            }
        ],
        "suppliers": [
            {
                "name": "seller",
                "id": 1
            },
            {
                "name": "vendor",
                "id": 2
            },
            {
                "name": "Miss Shaina Casper",
                "id": 22
            },
            {
                "name": "test",
                "id": 514
            }
        ]
    },
    "responseCode": 200,
    "responseMessage": "Succesfull"
}
```

<!-- 5 -->

## Get Specific Product 

**API** `http://localhost:8000/api/products/1011`

**Method** : GET


### Response :


_Example_

```
{
    "product": {
        "id": 15,
        "user_id": 1,
        "name": "TT Bags Unisex Backpacks Blue Color With laptop Compartment",
        "slug": "",
        "bdpin": "",
        "brand_id": 1,
        "model": "BAG17s",
        "sku": "BAG17s",
        "description": "Built for fast moving pursuits, the TT Backpack holds all your essential for long day on a trail. It is robust backpack proving protection, It comes equipped with a large padded pocket, internal and external accessory pouches which zip for extra security Comfort was also no sacrifice in the design of this backpack. To ensure that you keep going on your journey throughout the day, the TT bags has two padded adjustable shoulder straps and a padded back panel. You will hardly know you are wearing it! And when you finally stop to take a rest, this backpack will securely stand upright to ensure none of your products are damaged when you set it down.",
        "specification": "Model Number\tBAG17s\r\nItem Height\t15 Centimeters\r\nItem Length\t20 Centimeters\r\nItem Width\t5 Centimeters\r\nVolume Capacity\t20 Liters\r\nItem Weight\t430 Grams\r\nMaterial\tPolyester\r\nSpecial Features\tZip Closure, Shoulder Strap, Laptop Compartment\r\nClosure\tZipper\r\nInner Material\tSatin\r\nStrap\tAdjustable\r\nWarranty Type\tManufacturer",
        "weight": "500.00",
        "length": "40.00",
        "width": "20.00",
        "height": "30.00",
        "amount": "399.00",
        "quantity": 20,
        "status": 1,
        "source": "bigly",
        "source_id": null,
        "created_at": "2017-11-18 19:20:27",
        "updated_at": "2018-05-08 23:02:20",
        "min_price": "399.00",
        "max_price": "1299.00",
        "shipping_charge": "75.00",
        "brand_name": "TT BAGS",
        "brand": {
            "id": 1,
            "name": "TT BAGS"
        },
        "organization": null,
        "categories": [
            {
                "id": 100,
                "name": "Luggage & Bags - Backpacks",
                "description": "",
                "meta_title": "",
                "meta_des": "",
                "meta_keywords": "",
                "slug": "",
                "parent_id": null,
                "status": 1
            }
        ],
        "attributes": [],
        "user": {
            "id": 1,
            "name": "TT Bags",
            "username": null,
            "email": "ttbags5@gmail.com",
            "status": 1,
            "phone": "9810795886",
            "created_at": "Nov 18, 2017",
            "updated_at": "2018-02-12 16:17:36",
            "type": "vendor"
        },
        "rating": null,
        "media": [
            {
                "id": 21,
                "mime": "image/jpeg",
                "thumb": "media/thumb/1511013060-17-1.jpg",
                "small": "media/small/1511013060-17-1.jpg",
                "medium": "media/medium/1511013060-17-1.jpg",
                "large": "http://localhost:8000/media/large/1511013060-17-1.jpg",
                "caption": null,
                "default": 0,
                "check": "pending"
            },
            {
                "id": 22,
                "mime": "image/jpeg",
                "thumb": "media/thumb/1511013061-17-2.jpg",
                "small": "media/small/1511013061-17-2.jpg",
                "medium": "media/medium/1511013061-17-2.jpg",
                "large": "http://localhost:8000/media/large/1511013061-17-2.jpg",
                "caption": null,
                "default": 0,
                "check": "pending"
            },
            {
                "id": 23,
                "mime": "image/jpeg",
                "thumb": "media/thumb/1511013062-17-3.jpg",
                "small": "media/small/1511013062-17-3.jpg",
                "medium": "media/medium/1511013062-17-3.jpg",
                "large": "http://localhost:8000/media/large/1511013062-17-3.jpg",
                "caption": null,
                "default": 0,
                "check": "pending"
            },
            {
                "id": 24,
                "mime": "image/jpeg",
                "thumb": "media/thumb/1511013063-17-4.jpg",
                "small": "media/small/1511013063-17-4.jpg",
                "medium": "media/medium/1511013063-17-4.jpg",
                "large": "http://localhost:8000/media/large/1511013063-17-4.jpg",
                "caption": null,
                "default": 0,
                "check": "pending"
            },
            {
                "id": 25,
                "mime": "image/jpeg",
                "thumb": "media/thumb/1511013064-17-5.jpg",
                "small": "media/small/1511013064-17-5.jpg",
                "medium": "media/medium/1511013064-17-5.jpg",
                "large": "http://localhost:8000/media/large/1511013064-17-5.jpg",
                "caption": null,
                "default": 0,
                "check": "pending"
            }
        ],
        "user_product": {
            "id": 35849,
            "user_id": 759,
            "product_id": 15,
            "name": "yo",
            "amount": "222.00",
            "created_at": null,
            "updated_at": null,
            "description": ""
        }
    },
    "isWishlist": false
}

```


<!-- 6 -->

## To Delete the product (DELETE)


**API** `http://localhost:8000/api/products/11`

**Method** : DELETE

### Request :

_Example_

```
{
    "user_id" : 510,
    "name": "Beeee-Watsica"
}

```


### Response :


_Example_

```

{
    1
}


```

<!-- 7 -->

## To update the product (PUT)


**API** `http://localhost:8000/api/products/1007`

**Method** : DELETE

### Request :

_Example_

```
{
    "user_id" : 510,
    "name": "cfdsgvd",
    "amount" : 54
}


```


### Response :


_Example_

```

{
    "user_id": 510,
    "product_id": "1007",
    "name": "cfdsgvd",
    "amount": 54,
    "updated_at": "2018-04-17 06:11:16",
    "created_at": "2018-04-17 06:11:16",
    "id": 1030
}



```


<!-- 8 -->

## Search the product through name and sku


**API** `localhost:8000/api/search?data=Keebler`
**API** `http://dropship.bigly.io/api/search?data=pro&&page=3`

**Method** : GET


### Response :


_Example_

```

{
    "current_page": 1,
    "data": [
        {
            "id": 16,
            "name": "Keebler and Sons",
            "slug": "",
            "bdpin": "ff65b07e-5662-3228-a30e-eae9416354e1",
            "brand_id": null,
            "model": null,
            "sku": "ae482e49-f59e-3c04-a24f-6e46b0867839",
            "description": "Lory positively sakshi to tell them something more. 'You promised to tell you--all I know is, it would be grand, certainly,' said Alice, and sighing. 'It IS a Caucus-race?' said Alice; 'you needn't.",
            "specification": null,
            "weight": "2210.00",
            "length": "6968.00",
            "width": "1199.00",
            "height": "2914.00",
            "amount": "51.00",
            "quantity": 0,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-03-01 10:54:50",
            "updated_at": "2018-03-01 10:54:50",
            "min_price": "0.00",
            "max_price": "0.00",
            "shipping_charge": "0.00",
            "brand_name": "",
            "brand": null,
            "categories": [
                {
                    "name": "Hyatt, Maggio and Russel"
                },
                {
                    "name": "Stracke PLC"
                },
                {
                    "name": "White, Boyer and Kuhlman"
                }
            ]
        },
        {
            "id": 29,
            "name": "Keebler-Baumbach",
            "slug": "",
            "bdpin": "d75a0b24-0b0e-3929-8334-32e94530208b",
            "brand_id": null,
            "model": null,
            "sku": "da295074-7ed2-3ec9-b8be-00960db66b85",
            "description": "Alice was not an encouraging opening for a good deal to come down the hall. After a minute or two, which gave the Pigeon in a court of justice before, but she gained courage as she ran; but the.",
            "specification": null,
            "weight": "652.00",
            "length": "7336.00",
            "width": "3303.00",
            "height": "9357.00",
            "amount": "53.00",
            "quantity": 0,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-03-01 10:54:51",
            "updated_at": "2018-03-01 10:54:51",
            "min_price": "0.00",
            "max_price": "0.00",
            "shipping_charge": "0.00",
            "brand_name": "",
            "brand": null,
            "categories": [
                {
                    "name": "Wunsch-Waters"
                }
            ]
        },
        {
            "id": 156,
            "name": "Brown, Keebler and Jacobi",
            "slug": "",
            "bdpin": "8841fe38-6bc3-3486-8518-15890d3ce33a",
            "brand_id": null,
            "model": null,
            "sku": "dbe74dc6-1446-38a3-a0d6-6b023a1c28ca",
            "description": "Duck and a Dodo, a Lory and an Eaglet, and several other curious creatures. Alice led the way, was the White Rabbit interrupted: 'UNimportant, your Majesty means, of course,' he said do. Alice.",
            "specification": null,
            "weight": "4360.00",
            "length": "9897.00",
            "width": "5539.00",
            "height": "9109.00",
            "amount": "29.00",
            "quantity": 0,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-03-01 10:54:56",
            "updated_at": "2018-03-01 10:54:56",
            "min_price": "0.00",
            "max_price": "0.00",
            "shipping_charge": "0.00",
            "brand_name": "",
            "brand": null,
            "categories": [
                {
                    "name": "Wiza-Doyle"
                }
            ]
        },
        {
            "id": 262,
            "name": "Keebler PLC",
            "slug": "",
            "bdpin": "6562faa3-7e48-3a3b-926a-999c4e07d3c5",
            "brand_id": null,
            "model": null,
            "sku": "90733f2d-65fe-3a0f-9df5-bbb4dbfcf05a",
            "description": "Alice, rather alarmed at the Queen, in a tone of delight, and rushed at the great puzzle!' And she tried the effect of lying down on the slate. 'Herald, read the accusation!' said the Gryphon, 'that.",
            "specification": null,
            "weight": "5193.00",
            "length": "4666.00",
            "width": "7041.00",
            "height": "3814.00",
            "amount": "43.00",
            "quantity": 0,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-03-01 10:55:00",
            "updated_at": "2018-03-01 10:55:00",
            "min_price": "0.00",
            "max_price": "0.00",
            "shipping_charge": "0.00",
            "brand_name": "",
            "brand": null,
            "categories": [
                {
                    "name": "Koepp and Sons"
                },
                {
                    "name": "Glover Group"
                },
                {
                    "name": "Tremblay-Pollich"
                }
            ]
        },
        {
            "id": 512,
            "name": "Keebler-Kutch",
            "slug": "",
            "bdpin": "4226a69b-4896-32c3-85c9-0770122a703a",
            "brand_id": null,
            "model": null,
            "sku": "de04fdce-645a-32df-871f-2ac43f2eb537",
            "description": "The Cat's head began fading away the time. Alice had no idea how to set about it; if I'm not used to come out among the bright eager eyes were nearly out of the Queen's voice in the other. In the.",
            "specification": null,
            "weight": "8073.00",
            "length": "2504.00",
            "width": "2850.00",
            "height": "9525.00",
            "amount": "24.00",
            "quantity": 0,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-03-01 10:55:10",
            "updated_at": "2018-03-01 10:55:10",
            "min_price": "0.00",
            "max_price": "0.00",
            "shipping_charge": "0.00",
            "brand_name": "",
            "brand": null,
            "categories": [
                {
                    "name": "Spencer Group"
                }
            ]
        },
        {
            "id": 579,
            "name": "Keebler-Pacocha",
            "slug": "",
            "bdpin": "5b17491d-992a-333d-8105-c8ebd7a133b9",
            "brand_id": null,
            "model": null,
            "sku": "06a7206c-0ca4-364c-849d-b736c1723d87",
            "description": "Mouse was speaking, so that by the officers of the crowd below, and there they lay sprawling about, reminding her very earnestly, 'Now, Dinah, tell me your history, she do.' 'I'll tell it her,' said.",
            "specification": null,
            "weight": "1696.00",
            "length": "8309.00",
            "width": "4582.00",
            "height": "4392.00",
            "amount": "34.00",
            "quantity": 0,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-03-01 10:55:12",
            "updated_at": "2018-03-01 10:55:12",
            "min_price": "0.00",
            "max_price": "0.00",
            "shipping_charge": "0.00",
            "brand_name": "",
            "brand": null,
            "categories": [
                {
                    "name": "Koepp and Sons"
                },
                {
                    "name": "Lynch, Jast and Osinski"
                },
                {
                    "name": "Wiza-Doyle"
                }
            ]
        }
    ],
    "from": 1,
    "last_page": 1,
    "next_page_url": null,
    "path": "http://localhost:8000/api/search",
    "per_page": 15,
    "prev_page_url": null,
    "to": 6,
    "total": 6
}
 




```



<!-- 9 -->

## Add WishList  or Delete ( POST ) 

**API** `http://localhost:8000/api/wishlist`

**Method** : POST

### Request :

_Example_

```
{
    "user_id" : 510,
    "product_id" : 1007
}


```


### Response :


_Example_

```

{
    "name": "Product",
    "wishlist": {
        "user_id": 510,
        "product_id": 1007,
        "updated_at": "2018-04-17 09:27:40",
        "created_at": "2018-04-17 09:27:40",
        "id": 10,
        "product": {
            "id": 1007,
            "name": "Product",
            "slug": "",
            "bdpin": "",
            "brand_id": 5,
            "model": "xgrfv",
            "sku": "szdgvxdhxd",
            "description": "<p>this is a great product</p>",
            "specification": "rtfgjhnc",
            "weight": "100.00",
            "length": "50.00",
            "width": "2.00",
            "height": "22525.00",
            "amount": "50.00",
            "quantity": 20,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-03-26 12:24:04",
            "updated_at": "2018-04-16 09:05:04",
            "min_price": "100.00",
            "max_price": "1000.00",
            "shipping_charge": "10.00",
            "brand_name": "fhdxcrhgcfgh",
            "brand": {
                "id": 5,
                "name": "fhdxcrhgcfgh"
            }
        }
    },
    "status": "Added to your wishlist"
}




```


<!-- 10 -->


## To get all the Orders


**API** `http://localhost:8000/api/orders`

**Method** : GET

### Response :

_Example_

```
{
    "current_page": 1,
    "data": [
        {
            "id": 98,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_BeaR3GHG1aW5eC3c",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-03 10:45:00",
            "updated_at": "2018-03-03 10:45:03",
            "status": "cancelled",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 99,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_zHqx6oauo1QuGnGu",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-03 10:47:16",
            "updated_at": "2018-03-03 10:47:16",
            "status": "placed",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 100,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_19QlPF9aDfbKuc2V",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-03 11:11:43",
            "updated_at": "2018-03-03 11:11:47",
            "status": "cancelled",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 101,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_YBsaWKJFx4iuNok0",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-03 11:12:14",
            "updated_at": "2018-03-03 11:12:14",
            "status": "placed",
            "price": "1500.00",
            "payment_method": "cod"
        },
        {
            "id": 102,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_KKg4ghvuMxSmZhY0",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-03 11:12:43",
            "updated_at": "2018-03-03 11:12:57",
            "status": "cancelled",
            "price": "1500.00",
            "payment_method": "cod"
        },
        {
            "id": 103,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_aKGbBHFLDxnAb4MZ",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-05 08:48:45",
            "updated_at": "2018-03-05 08:48:45",
            "status": "placed",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 104,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_34lC2g7nZw73tfQL",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-05 08:59:43",
            "updated_at": "2018-03-05 09:19:08",
            "status": "",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 105,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_GKLRvZogmdUdTjCM",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-05 09:27:12",
            "updated_at": "2018-03-05 09:27:12",
            "status": "placed",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 106,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_hTOFtWIke0eDkxlU",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-05 09:29:46",
            "updated_at": "2018-03-05 09:29:48",
            "status": "",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 107,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_1NFBrHEg8QoWoCqJ",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-05 09:30:14",
            "updated_at": "2018-03-05 09:31:45",
            "status": "",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 108,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_xUyrl00VgGSk2qSn",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-06 08:54:46",
            "updated_at": "2018-03-06 08:54:46",
            "status": "placed",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 109,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_OIZybPuLx490LAsJ",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-06 09:33:34",
            "updated_at": "2018-03-06 09:48:45",
            "status": "",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 110,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_IZumwmn1hS6qGcP0",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-06 09:40:26",
            "updated_at": "2018-03-06 09:40:26",
            "status": "placed",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 111,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_ZyUAOiJLdtPJkaui",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-06 09:51:32",
            "updated_at": "2018-03-06 09:51:35",
            "status": "",
            "price": "3000.00",
            "payment_method": "cod"
        },
        {
            "id": 112,
            "user_id": 510,
            "client_id": 510,
            "name": "DS_Order_ERglNzjPH0ijV6pf",
            "invoice": "",
            "amount": "300.00",
            "created_at": "2018-03-06 09:51:53",
            "updated_at": "2018-03-06 09:51:55",
            "status": "",
            "price": "3000.00",
            "payment_method": "cod"
        }
    ],
    "from": 1,
    "last_page": 4,
    "next_page_url": "http://localhost:8000/api/orders?page=2",
    "path": "http://localhost:8000/api/orders",
    "per_page": 15,
    "prev_page_url": null,
    "to": 15,
    "total": 50
}



```

<!-- 11 -->

## To Order any product (POST)


**API** `http://localhost:8000/api/orders`

**Method** : POST

### Request :

_Example_

```
{
      "first_name" : "sakshi",
      "last_name" : "kbc",
      "email" : "sakshi@gmail.com",
      "mobile" : "1234565789",
      "address_line_1" : "N 21 , Above United Bank of India",
      "address_line_2" : "N 21 , Above United Bank of India",
      "city" : "Satna",
      "state" : "Madhya Pradesh",
      "pincode" : "485001",
      "country" : "India",
      "payment_method" : "cod",
      "sameadd" : "Sameadd",
      "shipping_first_name" : "sakshi",
      "shipping_last_name" : "kbc",
      "shipping_address1" : "N 21 , Above United Bank of India",
      "shipping_address2" : "N 21 , Above United Bank of India",
      "shipping_city" : "Satna",
      "shipping_pincode" : "485001",
      "shipping_country" : "India",
      "shipping_state" : "Madhya Pradesh",
      "sku" : "szdgvxdhxd",
      "quantity" : "1",
      "shipping_charge" : "10.00",
      "products" : [
        {
                    "id" : 1007,
                    "name" : "Product",
                    "amount" : 50,
                    "quantity" : 10
        }
        
                ],
      "name": "Product",
      "amount" : 54
}



```


### Response :


_Example_

```

{
    "user_id": 510,
    "client_id": 1,
    "name": "Product",
    "price": 54,
    "amount": "50.00",
    "status": "placed",
    "payment_method": "cod",
    "updated_at": "2018-04-19 11:57:36",
    "created_at": "2018-04-19 11:57:36",
    "id": 167
}


```


<!-- 12 -->

## Add to cart API (POST)


**API** `http://localhost:8000/api/addToCart`

**Method** : POST

### Request :

_Example_

```
{
    "user_id" : 510,
    "product_id" : 1011,
    "quantity" : 10,
    "editedAmount" : 50,
    "paymentMode" : "COD",
    "size" : 50,
    "color" : "blue",
    "type" : "cart"
}

```


### Response :


_Example_

```
{
    "cart": {
        "id": 52,
        "user_id": 759,
        "product_id": 1011,
        "attribute_id": 0,
        "quantity": 10,
        "amount": 50,
        "payment_mode": "COD",
        "status": 1,
        "type": "cart",
        "created_at": "2018-05-22 15:43:22",
        "updated_at": "2018-05-22 15:43:22",
        "product": {
            "id": 1011,
            "user_id": 19,
            "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
            "slug": "",
            "bdpin": "",
            "brand_id": 12,
            "model": "RCH15 103",
            "sku": "RCH15 103",
            "description": "Right Choice Girls-Ladies-Laptop Sholder Handbags Material : P.U - Colour :Black - Type : Casual Dimensions L X H X W (cm) : 47 x 29 x 12 (cm) Strap Type &amp; Closure Type : Belt-Zip Capacity &amp; Pockets : 2 kg-6+1 mobile pocket Warranty : 12 month On Manufacturing Defect With Replacement.",
            "specification": "\r\n\r\nWomen handbag laptop slot with velcro fastener\r\n\r\n",
            "weight": "450.00",
            "length": "47.00",
            "width": "29.00",
            "height": "12.00",
            "amount": "456.00",
            "quantity": 10,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2017-12-28 14:46:27",
            "updated_at": "2018-02-23 11:17:46",
            "min_price": "456.00",
            "max_price": "1299.00",
            "shipping_charge": "75.00",
            "brand_name": "Right Choice Bags",
            "brand": {
                "id": 12,
                "name": "Right Choice Bags"
            },
            "organization": {
                "id": 13,
                "user_id": 19,
                "type_id": 0,
                "name": "Right Choice Bags",
                "logo": "http://s.bigly.io/logo/1523474088-yTmwG6zmSXM6yAA.jpg",
                "gst": "36AJPPA8431P1ZO",
                "incorporation_number": "",
                "address": "12-1-487/b/11/51/9 huda colony\r\nasifnagar\r\nhyderabad TELANGANA\r\nIndia 500028",
                "introduction": "ECommerce",
                "created_at": "2017-12-28 14:25:05",
                "updated_at": "2018-04-12 00:44:48",
                "city": "hyderabad",
                "state": "TELANGANA",
                "pincode": "500028",
                "country": "India"
            },
            "media": [
                {
                    "id": 4883,
                    "mime": "image/jpeg",
                    "thumb": "media/thumb/1514625166-1.jpg",
                    "small": "media/small/1514625166-1.jpg",
                    "medium": "media/medium/1514625166-1.jpg",
                    "large": "http://localhost:8000/media/large/1514625166-1.jpg",
                    "caption": null,
                    "default": 0,
                    "check": "pending"
                },
                {
                    "id": 4884,
                    "mime": "image/jpeg",
                    "thumb": "media/thumb/1514625172-2.jpg",
                    "small": "media/small/1514625172-2.jpg",
                    "medium": "media/medium/1514625172-2.jpg",
                    "large": "http://localhost:8000/media/large/1514625172-2.jpg",
                    "caption": null,
                    "default": 0,
                    "check": "pending"
                },
                {
                    "id": 4885,
                    "mime": "image/jpeg",
                    "thumb": "media/thumb/1514625173-3.jpg",
                    "small": "media/small/1514625173-3.jpg",
                    "medium": "media/medium/1514625173-3.jpg",
                    "large": "http://localhost:8000/media/large/1514625173-3.jpg",
                    "caption": null,
                    "default": 0,
                    "check": "pending"
                },
                {
                    "id": 4886,
                    "mime": "image/jpeg",
                    "thumb": "media/thumb/1514625174-4.jpg",
                    "small": "media/small/1514625174-4.jpg",
                    "medium": "media/medium/1514625174-4.jpg",
                    "large": "http://localhost:8000/media/large/1514625174-4.jpg",
                    "caption": null,
                    "default": 0,
                    "check": "pending"
                },
                {
                    "id": 4887,
                    "mime": "image/jpeg",
                    "thumb": "media/thumb/1514625175-5.jpg",
                    "small": "media/small/1514625175-5.jpg",
                    "medium": "media/medium/1514625175-5.jpg",
                    "large": "http://localhost:8000/media/large/1514625175-5.jpg",
                    "caption": null,
                    "default": 0,
                    "check": "pending"
                },
                {
                    "id": 4888,
                    "mime": "image/jpeg",
                    "thumb": "media/thumb/1514625175-6.jpg",
                    "small": "media/small/1514625175-6.jpg",
                    "medium": "media/medium/1514625175-6.jpg",
                    "large": "http://localhost:8000/media/large/1514625175-6.jpg",
                    "caption": null,
                    "default": 0,
                    "check": "pending"
                }
            ]
        }
    },
    "responseMessage": "Product has been successfully Added",
    "responseCode": 200
}


```

<!-- 13 -->

## Delete Product from Cart 


**API** `http://localhost:8000/api/cart/3`

**Method** : DELETE


### Response :


_Example_

```

{
    "cart": {
        "id": 6,
        "user_id": 510,
        "product_id": 1007,
        "quantity": 1,
        "size": null,
        "color": null,
        "status": 1,
        "type": null,
        "created_at": "2018-04-20 08:01:23",
        "updated_at": "2018-04-20 08:01:23"
    },
    "responseCode": 200,
    "responseMessage": "Deleted From Cart"
}


```

<!-- 14 -->

##  View All the cart items of user 


**API** `http://localhost:8000/api/cart/user/510`

**Method** : GET


### Response :


_Example_

```

{
    "cart": [
        {
            "id": 1,
            "user_id": 510,
            "product_id": 1007,
            "quantity": 1,
            "size": null,
            "color": null,
            "status": 1,
            "type": null,
            "created_at": "2018-04-20 07:16:24",
            "updated_at": "2018-04-20 07:16:24",
            "product": {
                "id": 1007,
                "name": "Product",
                "slug": "",
                "bdpin": "",
                "brand_id": 5,
                "model": "xgrfv",
                "sku": "szdgvxdhxd",
                "description": "<p>this is a great product</p>",
                "specification": "rtfgjhnc",
                "weight": "100.00",
                "length": "50.00",
                "width": "2.00",
                "height": "22525.00",
                "amount": "50.00",
                "quantity": 20,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-26 12:24:04",
                "updated_at": "2018-04-16 09:05:04",
                "min_price": "100.00",
                "max_price": "1000.00",
                "shipping_charge": "10.00",
                "brand_name": "fhdxcrhgcfgh",
                "brand": {
                    "id": 5,
                    "name": "fhdxcrhgcfgh"
                },
                "organization": {
                    "id": 12,
                    "user_id": 514,
                    "type_id": 0,
                    "name": "bla bla",
                    "logo": "",
                    "gst": "",
                    "incorporation_number": "",
                    "address": "",
                    "introduction": "",
                    "created_at": "2018-03-26 12:22:21",
                    "updated_at": "2018-03-26 12:22:21",
                    "city": "",
                    "state": "",
                    "pincode": "",
                    "country": ""
                }
            },
            "media": [
                {
                    "id": 2,
                    "mime": "",
                    "thumb": "http://lorempixel.com/270/220/business/2",
                    "small": null,
                    "medium": "http://lorempixel.com/480/360/business/2",
                    "large": "http://lorempixel.com/1280/720/business/2",
                    "caption": null,
                    "default": 1,
                    "check": "pending"
                }
            ]
        }
    ],
    "responseMessage": "Successfull",
    "responseCode": 200
}




```

<!-- 15 -->

## Store Cart User Address 


**API** `http://localhost:8000/api/cart/address`

**Method** : POST

### Request :

_Example_

```
{
    "user_id": 510,
    "name" : "sakshi",
    "email" : "yo@gmail.com",
    "mobile" : "1234567890",
    "address" : "tggggawyhrfgbeyshgfraegegea",
    "street" : "10 , 1bgdddddddddddddb",
    "colony" : "uygsfukrg",
    "city"  :"city",
    "state" : "fsuyf",
    "landmark" : "sgfyuesgtes",
    "pincode" : 421848,
    "country" : "India",
    "type" : "shipping"
    
}


```


### Response :


_Example_

```

{
    "user_id": 510,
    "name": "sakshi",
    "email": "yo@gmail.com",
    "mobile": "1234567890",
    "address": "tggggawyhrfgbeyshgfraegegea",
    "street": "10 , 1bgdddddddddddddb",
    "colony": "uygsfukrg",
    "city": “erfer”,
    "state": "fsuyf",
    "landmark": "sgfyuesgtes",
    "pincode": 421848,
    "country": "India",
    "type": "shipping",
    "updated_at": "2018-04-20 11:17:21",
    "created_at": "2018-04-20 11:17:21",
    "id": 1
}




```

<!-- 16 -->

## Add Billing Details or Shipping Detail


**API** `http://localhost:8000/api/cart/address`

**Method** : POST

### Request :

_Example_

```
{
    "user_id": 510,
    "name" : "sakshi",
    "email" : "yo@gmail.com",
    "mobile" : "1234567890",
    "address" : "tggggawyhrfgbeyshgfraegegea",
    "street" : "10 , 1bgdddddddddddddb",
    "colony" : "uygsfukrg",
    "state" : "fsuyf",
    "landmark" : "sgfyuesgtes",
    "pincode" : 421848,
    "country" : "India",
    "type" : "SHIPPING"

}



```


### Response :


_Example_

```

{
    "address": {
        "user_id": 510,
        "name": "sakshi",
        "email": "yo@gmail.com",
        "mobile": "1234567890",
        "address": "tggggawyhrfgbeyshgfraegegea",
        "street": "10 , 1bgdddddddddddddb",
        "colony": "uygsfukrg",
        "city": null,
        "state": "fsuyf",
        "landmark": "sgfyuesgtes",
        "pincode": 421848,
        "country": "India",
        "type": "SHIPPING",
        "updated_at": "2018-04-21 10:28:14",
        "created_at": "2018-04-21 10:28:14",
        "id": 3
    },
    "responseMessage": "Added Successfully",
    "responseCode": 200
}





```



<!-- 17 -->

##  To View Users Billing and Shipping Address



**API** `http://localhost:8000/api/cart/address/510`

**Method** : GET

### Response :


_Example_

```

{
    "shippingAddress": [
        {
            "id": 1,
            "user_id": 510,
            "name": "sakshi",
            "email": "yo@gmail.com",
            "mobile": "1234567890",
            "address": "tggggawyhrfgbeyshgfraegegea",
            "street": "10 , 1bgdddddddddddddb",
            "colony": "uygsfukrg",
            "city": null,
            "state": "fsuyf",
            "landmark": "sgfyuesgtes",
            "pincode": "421848",
            "country": "India",
            "type": "shipping",
            "status": 1,
            "created_at": "2018-04-20 11:17:21",
            "updated_at": "2018-04-20 11:17:21"
        },
        {
            "id": 3,
            "user_id": 510,
            "name": "sakshi",
            "email": "yo@gmail.com",
            "mobile": "1234567890",
            "address": "tggggawyhrfgbeyshgfraegegea",
            "street": "10 , 1bgdddddddddddddb",
            "colony": "uygsfukrg",
            "city": null,
            "state": "fsuyf",
            "landmark": "sgfyuesgtes",
            "pincode": "421848",
            "country": "India",
            "type": "SHIPPING",
            "status": 1,
            "created_at": "2018-04-21 10:28:14",
            "updated_at": "2018-04-21 10:28:14"
        }
    ],
    "responseStatus": 200,
    "responseMessage": "Cart Address Found"
}






```

<!-- 18 -->

##  To Update Users Shipping Address



**API** `http://localhost:8000/api/cart/510/address/3`

**Method** : PUT

### Request :


_Example_
```
{
    "name" : "sanjay",
    "email" : "yo@gmail.com",
    "mobile" : "1234567890",
    "address" : "tggggawyhrfgbeyshgfraegegea",
    "street" : "10 , 1bgdddddddddddddb",
    "colony" : "uygsfukrg",
    "city" : "vbycgsvafyk",
    "state" : "fsuyf",
    "landmark" : "sgfyuesgtes",
    "pincode" : 421848,
    "country" : "India",
    "type" : "SHIPPING"
}
```

### Response

```
{
    "shippingAddress": 1,
    "responseStatus": 200,
    "responseMessage": "Cart Address Updated"
}
```

<!-- 19 -->

##  Delete Users Shipping Address



**API** `http://localhost:8000/api/cart/510/address/3`

**Method** : Delete

### Response :


_Example_

```
{
    "cart": {
        "id": 3,
        "user_id": 510,
        "name": "sanjay",
        "email": "yo@gmail.com",
        "mobile": "1234567890",
        "address": "tggggawyhrfgbeyshgfraegegea",
        "street": "10 , 1bgdddddddddddddb",
        "colony": "uygsfukrg",
        "city": "vbycgsvafyk",
        "state": "fsuyf",
        "landmark": "sgfyuesgtes",
        "pincode": "421848",
        "country": "India",
        "type": "SHIPPING",
        "status": 1,
        "created_at": "2018-04-21 10:28:14",
        "updated_at": "2018-05-05 18:04:47"
    },
    "responseCode": 200,
    "responseMessage": "Address Deleted"
}
```

<!-- 20 -->

##  Create Order


**API** `http://localhost:8000/api/addToOrder/{cart_id}`

**Method** : Post

### Request :


_Example_

```
{
    "quantity": 10,
    "payment_id" : "hvfdxkj",
    "address_id" : 2
}
```

### Response :

```
{
    "order": {
        "user_id": 510,
        "name": "DS_Order_QRSYyjKZGiznuI5H",
        "price": 210,
        "amount": "21.00",
        "status": "placed",
        "payment_method": "COD",
        "updated_at": "2018-05-07 16:56:06",
        "created_at": "2018-05-07 16:56:06",
        "id": 196
    },
    "item": {
        "order_id": 196,
        "product_id": 1011,
        "name": "sZEfgfr",
        "quantity": 10,
        "amount": 50,
        "status": "placed",
        "attribute_id": 17,
        "shipping_charge": "2.00",
        "id": 82
    },
    "payment": true
}
```


<!-- 21 -->

##  Contact Us


**API** `http://localhost:8000/api/contact`

**Method** : Post

### Request :


_Example_

```
{
    "subject" : "sfgsgras",
    "message": "ayhdgef"
}
```


### Response :

```
{
    "subject": "sfgsgras",
    "message": "ayhdgef",
    "email": "client@seller.com",
    "status": "open",
    "updated_at": "2018-05-09 11:50:48",
    "created_at": "2018-05-09 11:50:48",
    "id": 113
}
```

<!-- 22 -->

##  My Orders


**API** `http://localhost:8000/api/orders/user/510`

**Method** : Get

### Response :


_Example_

```
{
    "orders": [
        {
            "id": 286,
            "order_id": 298,
            "product_id": 1011,
            "attribute_id": 0,
            "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
            "quantity": 10,
            "amount": 456,
            "organization_id": 0,
            "status": "completed",
            "shipment_id": "",
            "shipping_charge": "75.00",
            "transfer_price": "456.00",
            "order": {
                "id": 298,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_pZEbNCshjO0OWSc2",
                "invoice": "",
                "amount": "456.00",
                "created_at": "2018-05-29 11:00:05",
                "updated_at": "2018-05-29 11:00:05",
                "status": "placed",
                "price": "4560.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 1011,
                "user_id": 19,
                "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
                "slug": "",
                "bdpin": "",
                "brand_id": 12,
                "model": "RCH15 103",
                "sku": "RCH15 103",
                "description": "Right Choice Girls-Ladies-Laptop Sholder Handbags Material : P.U - Colour :Black - Type : Casual Dimensions L X H X W (cm) : 47 x 29 x 12 (cm) Strap Type &amp; Closure Type : Belt-Zip Capacity &amp; Pockets : 2 kg-6+1 mobile pocket Warranty : 12 month On Manufacturing Defect With Replacement.",
                "specification": "\r\n\r\nWomen handbag laptop slot with velcro fastener\r\n\r\n",
                "weight": "450.00",
                "length": "47.00",
                "width": "29.00",
                "height": "12.00",
                "amount": "456.00",
                "quantity": 10,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2017-12-28 14:46:27",
                "updated_at": "2018-02-23 11:17:46",
                "min_price": "456.00",
                "max_price": "1299.00",
                "shipping_charge": "75.00",
                "brand_name": "Right Choice Bags",
                "brand": {
                    "id": 12,
                    "name": "Right Choice Bags"
                },
                "media": [
                    {
                        "id": 4883,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625166-1.jpg",
                        "small": "media/small/1514625166-1.jpg",
                        "medium": "media/medium/1514625166-1.jpg",
                        "large": "http://localhost:8000/media/large/1514625166-1.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4884,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625172-2.jpg",
                        "small": "media/small/1514625172-2.jpg",
                        "medium": "media/medium/1514625172-2.jpg",
                        "large": "http://localhost:8000/media/large/1514625172-2.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4885,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625173-3.jpg",
                        "small": "media/small/1514625173-3.jpg",
                        "medium": "media/medium/1514625173-3.jpg",
                        "large": "http://localhost:8000/media/large/1514625173-3.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4886,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625174-4.jpg",
                        "small": "media/small/1514625174-4.jpg",
                        "medium": "media/medium/1514625174-4.jpg",
                        "large": "http://localhost:8000/media/large/1514625174-4.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4887,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-5.jpg",
                        "small": "media/small/1514625175-5.jpg",
                        "medium": "media/medium/1514625175-5.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-5.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4888,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-6.jpg",
                        "small": "media/small/1514625175-6.jpg",
                        "medium": "media/medium/1514625175-6.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-6.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": null
        },
        {
            "id": 288,
            "order_id": 300,
            "product_id": 1011,
            "attribute_id": 0,
            "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
            "quantity": 10,
            "amount": 456,
            "organization_id": 0,
            "status": "completed",
            "shipment_id": "",
            "shipping_charge": "75.00",
            "transfer_price": "456.00",
            "order": {
                "id": 300,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_f34AUIqKvGKPX2Jg",
                "invoice": "",
                "amount": "456.00",
                "created_at": "2018-05-29 11:26:36",
                "updated_at": "2018-05-29 11:26:36",
                "status": "placed",
                "price": "4560.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 1011,
                "user_id": 19,
                "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
                "slug": "",
                "bdpin": "",
                "brand_id": 12,
                "model": "RCH15 103",
                "sku": "RCH15 103",
                "description": "Right Choice Girls-Ladies-Laptop Sholder Handbags Material : P.U - Colour :Black - Type : Casual Dimensions L X H X W (cm) : 47 x 29 x 12 (cm) Strap Type &amp; Closure Type : Belt-Zip Capacity &amp; Pockets : 2 kg-6+1 mobile pocket Warranty : 12 month On Manufacturing Defect With Replacement.",
                "specification": "\r\n\r\nWomen handbag laptop slot with velcro fastener\r\n\r\n",
                "weight": "450.00",
                "length": "47.00",
                "width": "29.00",
                "height": "12.00",
                "amount": "456.00",
                "quantity": 10,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2017-12-28 14:46:27",
                "updated_at": "2018-02-23 11:17:46",
                "min_price": "456.00",
                "max_price": "1299.00",
                "shipping_charge": "75.00",
                "brand_name": "Right Choice Bags",
                "brand": {
                    "id": 12,
                    "name": "Right Choice Bags"
                },
                "media": [
                    {
                        "id": 4883,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625166-1.jpg",
                        "small": "media/small/1514625166-1.jpg",
                        "medium": "media/medium/1514625166-1.jpg",
                        "large": "http://localhost:8000/media/large/1514625166-1.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4884,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625172-2.jpg",
                        "small": "media/small/1514625172-2.jpg",
                        "medium": "media/medium/1514625172-2.jpg",
                        "large": "http://localhost:8000/media/large/1514625172-2.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4885,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625173-3.jpg",
                        "small": "media/small/1514625173-3.jpg",
                        "medium": "media/medium/1514625173-3.jpg",
                        "large": "http://localhost:8000/media/large/1514625173-3.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4886,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625174-4.jpg",
                        "small": "media/small/1514625174-4.jpg",
                        "medium": "media/medium/1514625174-4.jpg",
                        "large": "http://localhost:8000/media/large/1514625174-4.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4887,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-5.jpg",
                        "small": "media/small/1514625175-5.jpg",
                        "medium": "media/medium/1514625175-5.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-5.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4888,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-6.jpg",
                        "small": "media/small/1514625175-6.jpg",
                        "medium": "media/medium/1514625175-6.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-6.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 17,
                "user_id": 759,
                "order_id": 288,
                "name": "sakshi",
                "email": null,
                "mobile": "1234567890",
                "address": "tggggawyhrfgbeyshgfraegegea",
                "street": "10 , 1bgdddddddddddddb",
                "colony": "uygsfukrg",
                "city": "vbycgsvafyk",
                "state": "fsuyf",
                "landmark": "sgfyuesgtes",
                "pincode": "421848",
                "country": "India",
                "type": null,
                "status": 1,
                "created_at": "2018-05-17 16:57:55",
                "updated_at": "2018-05-17 16:57:55"
            }
        },
        {
            "id": 289,
            "order_id": 301,
            "product_id": 1011,
            "attribute_id": 0,
            "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
            "quantity": 10,
            "amount": 456,
            "organization_id": 0,
            "status": "completed",
            "shipment_id": "",
            "shipping_charge": "75.00",
            "transfer_price": "456.00",
            "order": {
                "id": 301,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_soYn4OfM1Df0JLsg",
                "invoice": "",
                "amount": "456.00",
                "created_at": "2018-05-29 11:43:40",
                "updated_at": "2018-05-29 11:43:40",
                "status": "placed",
                "price": "4560.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 1011,
                "user_id": 19,
                "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
                "slug": "",
                "bdpin": "",
                "brand_id": 12,
                "model": "RCH15 103",
                "sku": "RCH15 103",
                "description": "Right Choice Girls-Ladies-Laptop Sholder Handbags Material : P.U - Colour :Black - Type : Casual Dimensions L X H X W (cm) : 47 x 29 x 12 (cm) Strap Type &amp; Closure Type : Belt-Zip Capacity &amp; Pockets : 2 kg-6+1 mobile pocket Warranty : 12 month On Manufacturing Defect With Replacement.",
                "specification": "\r\n\r\nWomen handbag laptop slot with velcro fastener\r\n\r\n",
                "weight": "450.00",
                "length": "47.00",
                "width": "29.00",
                "height": "12.00",
                "amount": "456.00",
                "quantity": 10,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2017-12-28 14:46:27",
                "updated_at": "2018-02-23 11:17:46",
                "min_price": "456.00",
                "max_price": "1299.00",
                "shipping_charge": "75.00",
                "brand_name": "Right Choice Bags",
                "brand": {
                    "id": 12,
                    "name": "Right Choice Bags"
                },
                "media": [
                    {
                        "id": 4883,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625166-1.jpg",
                        "small": "media/small/1514625166-1.jpg",
                        "medium": "media/medium/1514625166-1.jpg",
                        "large": "http://localhost:8000/media/large/1514625166-1.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4884,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625172-2.jpg",
                        "small": "media/small/1514625172-2.jpg",
                        "medium": "media/medium/1514625172-2.jpg",
                        "large": "http://localhost:8000/media/large/1514625172-2.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4885,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625173-3.jpg",
                        "small": "media/small/1514625173-3.jpg",
                        "medium": "media/medium/1514625173-3.jpg",
                        "large": "http://localhost:8000/media/large/1514625173-3.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4886,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625174-4.jpg",
                        "small": "media/small/1514625174-4.jpg",
                        "medium": "media/medium/1514625174-4.jpg",
                        "large": "http://localhost:8000/media/large/1514625174-4.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4887,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-5.jpg",
                        "small": "media/small/1514625175-5.jpg",
                        "medium": "media/medium/1514625175-5.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-5.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4888,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-6.jpg",
                        "small": "media/small/1514625175-6.jpg",
                        "medium": "media/medium/1514625175-6.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-6.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 18,
                "user_id": 796,
                "order_id": 289,
                "name": "Gunjan Kumar",
                "email": null,
                "mobile": "7290918926",
                "address": "B block",
                "street": "Gali No:8",
                "colony": "Gali No:8",
                "city": "New Delhi",
                "state": "Delhi",
                "landmark": "New Ashok Nagar Metro",
                "pincode": "110096",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-17 17:20:25",
                "updated_at": "2018-05-17 17:20:25"
            }
        },
        {
            "id": 290,
            "order_id": 302,
            "product_id": 1011,
            "attribute_id": 0,
            "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
            "quantity": 10,
            "amount": 456,
            "organization_id": 0,
            "status": "completed",
            "shipment_id": "444563302",
            "shipping_charge": "75.00",
            "transfer_price": "456.00",
            "order": {
                "id": 302,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_Sgrh097wDXLo3M8i",
                "invoice": "",
                "amount": "456.00",
                "created_at": "2018-05-29 12:03:08",
                "updated_at": "2018-05-29 12:03:08",
                "status": "placed",
                "price": "4560.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 1011,
                "user_id": 19,
                "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
                "slug": "",
                "bdpin": "",
                "brand_id": 12,
                "model": "RCH15 103",
                "sku": "RCH15 103",
                "description": "Right Choice Girls-Ladies-Laptop Sholder Handbags Material : P.U - Colour :Black - Type : Casual Dimensions L X H X W (cm) : 47 x 29 x 12 (cm) Strap Type &amp; Closure Type : Belt-Zip Capacity &amp; Pockets : 2 kg-6+1 mobile pocket Warranty : 12 month On Manufacturing Defect With Replacement.",
                "specification": "\r\n\r\nWomen handbag laptop slot with velcro fastener\r\n\r\n",
                "weight": "450.00",
                "length": "47.00",
                "width": "29.00",
                "height": "12.00",
                "amount": "456.00",
                "quantity": 10,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2017-12-28 14:46:27",
                "updated_at": "2018-02-23 11:17:46",
                "min_price": "456.00",
                "max_price": "1299.00",
                "shipping_charge": "75.00",
                "brand_name": "Right Choice Bags",
                "brand": {
                    "id": 12,
                    "name": "Right Choice Bags"
                },
                "media": [
                    {
                        "id": 4883,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625166-1.jpg",
                        "small": "media/small/1514625166-1.jpg",
                        "medium": "media/medium/1514625166-1.jpg",
                        "large": "http://localhost:8000/media/large/1514625166-1.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4884,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625172-2.jpg",
                        "small": "media/small/1514625172-2.jpg",
                        "medium": "media/medium/1514625172-2.jpg",
                        "large": "http://localhost:8000/media/large/1514625172-2.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4885,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625173-3.jpg",
                        "small": "media/small/1514625173-3.jpg",
                        "medium": "media/medium/1514625173-3.jpg",
                        "large": "http://localhost:8000/media/large/1514625173-3.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4886,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625174-4.jpg",
                        "small": "media/small/1514625174-4.jpg",
                        "medium": "media/medium/1514625174-4.jpg",
                        "large": "http://localhost:8000/media/large/1514625174-4.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4887,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-5.jpg",
                        "small": "media/small/1514625175-5.jpg",
                        "medium": "media/medium/1514625175-5.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-5.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4888,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-6.jpg",
                        "small": "media/small/1514625175-6.jpg",
                        "medium": "media/medium/1514625175-6.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-6.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 19,
                "user_id": 796,
                "order_id": 290,
                "name": "Gunjan Kumar",
                "email": null,
                "mobile": "7290918926",
                "address": "B block",
                "street": "Gali No:8",
                "colony": "Gali No:8",
                "city": "New Delhi",
                "state": "Delhi",
                "landmark": "New Ashok Nagar Metro",
                "pincode": "110096",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-17 17:24:26",
                "updated_at": "2018-05-17 17:24:26"
            }
        },
        {
            "id": 291,
            "order_id": 303,
            "product_id": 1011,
            "attribute_id": 0,
            "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
            "quantity": 10,
            "amount": 456,
            "organization_id": 0,
            "status": "completed",
            "shipment_id": "541009303",
            "shipping_charge": "75.00",
            "transfer_price": "456.00",
            "order": {
                "id": 303,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_cT52P5zToRKF91Wq",
                "invoice": "",
                "amount": "456.00",
                "created_at": "2018-05-29 12:20:32",
                "updated_at": "2018-05-29 12:20:32",
                "status": "placed",
                "price": "4560.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 1011,
                "user_id": 19,
                "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
                "slug": "",
                "bdpin": "",
                "brand_id": 12,
                "model": "RCH15 103",
                "sku": "RCH15 103",
                "description": "Right Choice Girls-Ladies-Laptop Sholder Handbags Material : P.U - Colour :Black - Type : Casual Dimensions L X H X W (cm) : 47 x 29 x 12 (cm) Strap Type &amp; Closure Type : Belt-Zip Capacity &amp; Pockets : 2 kg-6+1 mobile pocket Warranty : 12 month On Manufacturing Defect With Replacement.",
                "specification": "\r\n\r\nWomen handbag laptop slot with velcro fastener\r\n\r\n",
                "weight": "450.00",
                "length": "47.00",
                "width": "29.00",
                "height": "12.00",
                "amount": "456.00",
                "quantity": 10,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2017-12-28 14:46:27",
                "updated_at": "2018-02-23 11:17:46",
                "min_price": "456.00",
                "max_price": "1299.00",
                "shipping_charge": "75.00",
                "brand_name": "Right Choice Bags",
                "brand": {
                    "id": 12,
                    "name": "Right Choice Bags"
                },
                "media": [
                    {
                        "id": 4883,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625166-1.jpg",
                        "small": "media/small/1514625166-1.jpg",
                        "medium": "media/medium/1514625166-1.jpg",
                        "large": "http://localhost:8000/media/large/1514625166-1.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4884,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625172-2.jpg",
                        "small": "media/small/1514625172-2.jpg",
                        "medium": "media/medium/1514625172-2.jpg",
                        "large": "http://localhost:8000/media/large/1514625172-2.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4885,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625173-3.jpg",
                        "small": "media/small/1514625173-3.jpg",
                        "medium": "media/medium/1514625173-3.jpg",
                        "large": "http://localhost:8000/media/large/1514625173-3.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4886,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625174-4.jpg",
                        "small": "media/small/1514625174-4.jpg",
                        "medium": "media/medium/1514625174-4.jpg",
                        "large": "http://localhost:8000/media/large/1514625174-4.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4887,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-5.jpg",
                        "small": "media/small/1514625175-5.jpg",
                        "medium": "media/medium/1514625175-5.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-5.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4888,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-6.jpg",
                        "small": "media/small/1514625175-6.jpg",
                        "medium": "media/medium/1514625175-6.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-6.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 20,
                "user_id": 759,
                "order_id": 291,
                "name": "sakshi",
                "email": null,
                "mobile": "1234567890",
                "address": "tggggawyhrfgbeyshgfraegegea",
                "street": "10 , 1bgdddddddddddddb",
                "colony": "uygsfukrg",
                "city": "vbycgsvafyk",
                "state": "fsuyf",
                "landmark": "sgfyuesgtes",
                "pincode": "421848",
                "country": "India",
                "type": null,
                "status": 1,
                "created_at": "2018-05-17 17:29:01",
                "updated_at": "2018-05-17 17:29:01"
            }
        },
        {
            "id": 292,
            "order_id": 304,
            "product_id": 1011,
            "attribute_id": 0,
            "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
            "quantity": 10,
            "amount": 456,
            "organization_id": 0,
            "status": "placed",
            "shipment_id": "249727304",
            "shipping_charge": "75.00",
            "transfer_price": "456.00",
            "order": {
                "id": 304,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_HZUm9tG9SoWRC9Vj",
                "invoice": "",
                "amount": "456.00",
                "created_at": "2018-05-29 12:23:51",
                "updated_at": "2018-05-29 12:23:51",
                "status": "placed",
                "price": "4560.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 1011,
                "user_id": 19,
                "name": "Right Choice,women's-Girls-Ladies-Laptop Sholder Handbags Online in India Black (RCH15 103)",
                "slug": "",
                "bdpin": "",
                "brand_id": 12,
                "model": "RCH15 103",
                "sku": "RCH15 103",
                "description": "Right Choice Girls-Ladies-Laptop Sholder Handbags Material : P.U - Colour :Black - Type : Casual Dimensions L X H X W (cm) : 47 x 29 x 12 (cm) Strap Type &amp; Closure Type : Belt-Zip Capacity &amp; Pockets : 2 kg-6+1 mobile pocket Warranty : 12 month On Manufacturing Defect With Replacement.",
                "specification": "\r\n\r\nWomen handbag laptop slot with velcro fastener\r\n\r\n",
                "weight": "450.00",
                "length": "47.00",
                "width": "29.00",
                "height": "12.00",
                "amount": "456.00",
                "quantity": 10,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2017-12-28 14:46:27",
                "updated_at": "2018-02-23 11:17:46",
                "min_price": "456.00",
                "max_price": "1299.00",
                "shipping_charge": "75.00",
                "brand_name": "Right Choice Bags",
                "brand": {
                    "id": 12,
                    "name": "Right Choice Bags"
                },
                "media": [
                    {
                        "id": 4883,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625166-1.jpg",
                        "small": "media/small/1514625166-1.jpg",
                        "medium": "media/medium/1514625166-1.jpg",
                        "large": "http://localhost:8000/media/large/1514625166-1.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4884,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625172-2.jpg",
                        "small": "media/small/1514625172-2.jpg",
                        "medium": "media/medium/1514625172-2.jpg",
                        "large": "http://localhost:8000/media/large/1514625172-2.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4885,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625173-3.jpg",
                        "small": "media/small/1514625173-3.jpg",
                        "medium": "media/medium/1514625173-3.jpg",
                        "large": "http://localhost:8000/media/large/1514625173-3.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4886,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625174-4.jpg",
                        "small": "media/small/1514625174-4.jpg",
                        "medium": "media/medium/1514625174-4.jpg",
                        "large": "http://localhost:8000/media/large/1514625174-4.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4887,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-5.jpg",
                        "small": "media/small/1514625175-5.jpg",
                        "medium": "media/medium/1514625175-5.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-5.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 4888,
                        "mime": "image/jpeg",
                        "thumb": "media/thumb/1514625175-6.jpg",
                        "small": "media/small/1514625175-6.jpg",
                        "medium": "media/medium/1514625175-6.jpg",
                        "large": "http://localhost:8000/media/large/1514625175-6.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 21,
                "user_id": 759,
                "order_id": 292,
                "name": "sakshi",
                "email": null,
                "mobile": "1234567890",
                "address": "tggggawyhrfgbeyshgfraegegea",
                "street": "10 , 1bgdddddddddddddb",
                "colony": "uygsfukrg",
                "city": "vbycgsvafyk",
                "state": "fsuyf",
                "landmark": "sgfyuesgtes",
                "pincode": "421848",
                "country": "India",
                "type": null,
                "status": 1,
                "created_at": "2018-05-17 18:34:23",
                "updated_at": "2018-05-17 18:34:23"
            }
        },
        {
            "id": 293,
            "order_id": 305,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "204051305",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 305,
                "user_id": 989,
                "client_id": 989,
                "name": "DS_Order_BtpGzTODkMmUNMxe",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 12:35:55",
                "updated_at": "2018-05-29 12:37:38",
                "status": "dispatched",
                "price": "20.00",
                "payment_method": "cod"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 22,
                "user_id": 796,
                "order_id": 293,
                "name": "sakshi",
                "email": null,
                "mobile": "1234567890",
                "address": "tggggawyhrfgbeyshgfraegegea",
                "street": "10 , 1bgdddddddddddddb",
                "colony": "uygsfukrg",
                "city": "vbycgsvafyk",
                "state": "fsuyf",
                "landmark": "sgfyuesgtes",
                "pincode": "421848",
                "country": "India",
                "type": null,
                "status": 1,
                "created_at": "2018-05-17 18:51:59",
                "updated_at": "2018-05-17 18:51:59"
            }
        },
        {
            "id": 294,
            "order_id": 306,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "203273306",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 306,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_JTTv69trQxTeHksv",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 13:06:47",
                "updated_at": "2018-05-29 15:34:39",
                "status": "dispatched",
                "price": "20.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 23,
                "user_id": 796,
                "order_id": 294,
                "name": "Gunjan Kumar",
                "email": null,
                "mobile": "7290918926",
                "address": "B block",
                "street": "Gali No:8",
                "colony": "Gali No:8",
                "city": "New Delhi",
                "state": "Delhi",
                "landmark": "New Ashok Nagar Metro",
                "pincode": "110096",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-17 18:54:18",
                "updated_at": "2018-05-17 18:54:18"
            }
        },
        {
            "id": 295,
            "order_id": 307,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "completed",
            "shipment_id": "180182307",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 307,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_n1ja2ojJISEAPdLr",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 14:29:20",
                "updated_at": "2018-05-29 14:29:20",
                "status": "placed",
                "price": "20.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 24,
                "user_id": 796,
                "order_id": 295,
                "name": "sakshi",
                "email": null,
                "mobile": "1234567890",
                "address": "tggggawyhrfgbeyshgfraegegea",
                "street": "10 , 1bgdddddddddddddb",
                "colony": "uygsfukrg",
                "city": "vbycgsvafyk",
                "state": "fsuyf",
                "landmark": "sgfyuesgtes",
                "pincode": "421848",
                "country": "India",
                "type": null,
                "status": 1,
                "created_at": "2018-05-17 19:00:06",
                "updated_at": "2018-05-17 19:00:06"
            }
        },
        {
            "id": 296,
            "order_id": 308,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "795224308",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 308,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_NWnX09kNzeupTaqm",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 15:45:44",
                "updated_at": "2018-05-29 16:13:29",
                "status": "dispatched",
                "price": "20.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": null
        },
        {
            "id": 297,
            "order_id": 309,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "772968309",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 309,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_xUKjuigd6jYUPkeo",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 16:39:32",
                "updated_at": "2018-05-29 16:39:32",
                "status": "placed",
                "price": "20.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 27,
                "user_id": 759,
                "order_id": 297,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-29 10:57:25",
                "updated_at": "2018-05-29 10:57:25"
            }
        },
        {
            "id": 298,
            "order_id": 310,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "324378310",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 310,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_gCUxqxO3hKmoJJP6",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 16:43:54",
                "updated_at": "2018-05-29 16:43:54",
                "status": "placed",
                "price": "20.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 28,
                "user_id": 989,
                "order_id": 298,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-29 11:00:05",
                "updated_at": "2018-05-29 11:00:05"
            }
        },
        {
            "id": 299,
            "order_id": 311,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "346530311",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 311,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_vUxmemRiONfqyMgd",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 16:45:30",
                "updated_at": "2018-05-29 16:45:30",
                "status": "placed",
                "price": "20.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 29,
                "user_id": 759,
                "order_id": 299,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-29 11:24:51",
                "updated_at": "2018-05-29 11:24:51"
            }
        },
        {
            "id": 300,
            "order_id": 312,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "175330312",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 312,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_EjKCEiSqVtxdnHj5",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 16:47:00",
                "updated_at": "2018-05-29 16:47:00",
                "status": "placed",
                "price": "20.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 30,
                "user_id": 989,
                "order_id": 300,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-29 11:26:36",
                "updated_at": "2018-05-29 11:26:36"
            }
        },
        {
            "id": 301,
            "order_id": 313,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "632691313",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 313,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_JQFXEHMO9DFrd3Tn",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 16:50:42",
                "updated_at": "2018-05-29 16:50:42",
                "status": "placed",
                "price": "20.00",
                "payment_method": "COD"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 31,
                "user_id": 989,
                "order_id": 301,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-29 11:43:40",
                "updated_at": "2018-05-29 11:43:40"
            }
        },
        {
            "id": 302,
            "order_id": 314,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "679135314",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 314,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_paGtUklp7fkdh99u",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 16:53:02",
                "updated_at": "2018-05-29 16:53:02",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 32,
                "user_id": 989,
                "order_id": 302,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-29 12:03:08",
                "updated_at": "2018-05-29 12:03:08"
            }
        },
        {
            "id": 303,
            "order_id": 315,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "461292315",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 315,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_XQ3D9LCI1kPxoFu7",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 16:54:18",
                "updated_at": "2018-05-29 16:54:18",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 33,
                "user_id": 989,
                "order_id": 303,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": null,
                "status": 1,
                "created_at": "2018-05-29 12:20:32",
                "updated_at": "2018-05-29 12:20:32"
            }
        },
        {
            "id": 304,
            "order_id": 316,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "436697316",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 316,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_yGJ3r5RqAZpKGmps",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 16:59:23",
                "updated_at": "2018-05-29 16:59:23",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 34,
                "user_id": 989,
                "order_id": 304,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 12:23:51",
                "updated_at": "2018-05-29 12:23:51"
            }
        },
        {
            "id": 305,
            "order_id": 317,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "263014317",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 317,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_VEVARWNl1WEAYDl5",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 17:10:37",
                "updated_at": "2018-05-29 17:10:37",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": null
        },
        {
            "id": 306,
            "order_id": 318,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "667066318",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 318,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_tWsnLSXjH0Kg3WfN",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 17:15:30",
                "updated_at": "2018-05-29 17:15:30",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 35,
                "user_id": 989,
                "order_id": 306,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 13:06:47",
                "updated_at": "2018-05-29 13:06:47"
            }
        },
        {
            "id": 307,
            "order_id": 319,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "261416319",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 319,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_vCSJjGj42najRg4I",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 17:22:32",
                "updated_at": "2018-05-29 17:22:32",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 36,
                "user_id": 989,
                "order_id": 307,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 14:29:20",
                "updated_at": "2018-05-29 14:29:20"
            }
        },
        {
            "id": 308,
            "order_id": 320,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "860557320",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 320,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_PYlNWyG412OfSNvq",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 18:05:11",
                "updated_at": "2018-05-29 18:05:11",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 37,
                "user_id": 989,
                "order_id": 308,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 15:45:44",
                "updated_at": "2018-05-29 15:45:44"
            }
        },
        {
            "id": 309,
            "order_id": 321,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "985466321",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 321,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_6nqfoBOoKcNoIqXt",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-29 18:08:23",
                "updated_at": "2018-05-29 18:08:23",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 38,
                "user_id": 989,
                "order_id": 309,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 16:39:32",
                "updated_at": "2018-05-29 16:39:32"
            }
        },
        {
            "id": 310,
            "order_id": 322,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "526910322",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 322,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_5B4EmWENowulLIBE",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 11:41:54",
                "updated_at": "2018-05-30 11:41:54",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 39,
                "user_id": 989,
                "order_id": 310,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 16:43:54",
                "updated_at": "2018-05-29 16:43:54"
            }
        },
        {
            "id": 311,
            "order_id": 323,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "772667323",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 323,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_AUpg52KGAZMHJSiF",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:05:30",
                "updated_at": "2018-05-30 12:05:30",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 40,
                "user_id": 989,
                "order_id": 311,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 16:45:30",
                "updated_at": "2018-05-29 16:45:30"
            }
        },
        {
            "id": 312,
            "order_id": 324,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "451279324",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 324,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_GTW1bPqN1uh21Tju",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:07:45",
                "updated_at": "2018-05-30 12:07:45",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 41,
                "user_id": 989,
                "order_id": 312,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 16:47:00",
                "updated_at": "2018-05-29 16:47:00"
            }
        },
        {
            "id": 313,
            "order_id": 325,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "736937325",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 325,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_be5akMFEq4vDfrI7",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:09:55",
                "updated_at": "2018-05-30 12:09:55",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 42,
                "user_id": 989,
                "order_id": 313,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 16:50:42",
                "updated_at": "2018-05-29 16:50:42"
            }
        },
        {
            "id": 314,
            "order_id": 326,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "441188326",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 326,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_j2rw1ksgIo0Nw6xV",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:11:47",
                "updated_at": "2018-05-30 12:11:47",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 43,
                "user_id": 989,
                "order_id": 314,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 16:53:02",
                "updated_at": "2018-05-29 16:53:02"
            }
        },
        {
            "id": 315,
            "order_id": 327,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "517171327",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 327,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_d7OjFFwfvcLQzECQ",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:14:52",
                "updated_at": "2018-05-30 12:15:35",
                "status": "dispatched",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 44,
                "user_id": 989,
                "order_id": 315,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 16:54:18",
                "updated_at": "2018-05-29 16:54:18"
            }
        },
        {
            "id": 316,
            "order_id": 328,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "completed",
            "shipment_id": "371615328",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 328,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_QTmlTxo6Exy31DVD",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:19:02",
                "updated_at": "2018-05-30 12:19:02",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 45,
                "user_id": 989,
                "order_id": 316,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 16:59:23",
                "updated_at": "2018-05-29 16:59:23"
            }
        },
        {
            "id": 317,
            "order_id": 329,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "697787329",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 329,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_9uxKcafF23ExSoLX",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:21:00",
                "updated_at": "2018-05-30 12:21:00",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 46,
                "user_id": 989,
                "order_id": 317,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 17:10:37",
                "updated_at": "2018-05-29 17:10:37"
            }
        },
        {
            "id": 318,
            "order_id": 330,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "992264330",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 330,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_4hJ34ldewSP5yTA1",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:24:20",
                "updated_at": "2018-05-30 12:24:58",
                "status": "dispatched",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 47,
                "user_id": 989,
                "order_id": 318,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 17:15:30",
                "updated_at": "2018-05-29 17:15:30"
            }
        },
        {
            "id": 319,
            "order_id": 331,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "621616331",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 331,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_uV0pI0I5mWdtCigT",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:26:25",
                "updated_at": "2018-05-30 12:27:00",
                "status": "dispatched",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 48,
                "user_id": 989,
                "order_id": 319,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 17:22:32",
                "updated_at": "2018-05-29 17:22:32"
            }
        },
        {
            "id": 320,
            "order_id": 332,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "delivered",
            "shipment_id": "624938332",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 332,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_L045tR2Wi1IR3pzf",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-30 12:32:55",
                "updated_at": "2018-05-30 12:33:34",
                "status": "dispatched",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 49,
                "user_id": 989,
                "order_id": 320,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 18:05:11",
                "updated_at": "2018-05-29 18:05:11"
            }
        },
        {
            "id": 321,
            "order_id": 333,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "shipped",
            "shipment_id": "160897333",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 333,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_2LGmCmeYOSp2ToRN",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-05-31 16:38:58",
                "updated_at": "2018-05-31 16:38:58",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 50,
                "user_id": 989,
                "order_id": 321,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-29 18:08:23",
                "updated_at": "2018-05-29 18:08:23"
            }
        },
        {
            "id": 322,
            "order_id": 334,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "placed",
            "shipment_id": "710209334",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 334,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_Sr93YlbGUxAJeUjD",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-06-01 16:39:19",
                "updated_at": "2018-06-01 16:39:19",
                "status": "placed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 51,
                "user_id": 989,
                "order_id": 322,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-30 11:41:54",
                "updated_at": "2018-05-30 11:41:54"
            }
        },
        {
            "id": 323,
            "order_id": 335,
            "product_id": 12583,
            "attribute_id": 0,
            "name": "General Knowledge 2019",
            "quantity": 1,
            "amount": 20,
            "organization_id": 219,
            "status": "dispatched",
            "shipment_id": "804562335",
            "shipping_charge": "30.00",
            "transfer_price": "20.00",
            "order": {
                "id": 335,
                "user_id": 989,
                "client_id": 0,
                "name": "DS_Order_5kpNG8X870EbbQwf",
                "invoice": "",
                "amount": "20.00",
                "created_at": "2018-06-01 16:40:43",
                "updated_at": "2018-06-01 16:40:43",
                "status": "completed",
                "price": "20.00",
                "payment_method": "PREPAID"
            },
            "product": {
                "id": 12583,
                "user_id": 254,
                "name": "General Knowledge 2019",
                "slug": "",
                "bdpin": "",
                "brand_id": 57,
                "model": "BDPIN10003",
                "sku": "BDPIN10003",
                "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
                "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
                "weight": "100.00",
                "length": "20.00",
                "width": "0.60",
                "height": "13.00",
                "amount": "20.00",
                "quantity": 123,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-02-20 15:49:34",
                "updated_at": "2018-06-01 16:42:12",
                "min_price": "20.00",
                "max_price": "50.00",
                "shipping_charge": "30.00",
                "brand_name": "By Manohar Pandey",
                "brand": {
                    "id": 57,
                    "name": "By Manohar Pandey"
                },
                "media": [
                    {
                        "id": 27558,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                        "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                        "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                        "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ]
            },
            "cart_address": {
                "id": 52,
                "user_id": 989,
                "order_id": 323,
                "name": "Gunjan",
                "email": null,
                "mobile": "7290918926",
                "address": "gaya",
                "street": "gzhzg",
                "colony": "gzhzg",
                "city": "New Dehi",
                "state": "Bihar",
                "landmark": "vzhsj",
                "pincode": "9865325",
                "country": "INDIA",
                "type": "BILLING",
                "status": 1,
                "created_at": "2018-05-30 12:05:30",
                "updated_at": "2018-05-30 12:05:30"
            }
        }
    ],
    "responseMessage": "User All Orders",
    "responseCode": 200
}
```



<!-- 23 -->

##  Orders Details


**API** `http://localhost:8000/api/orders/199`

**Method** : Get

### Response :


_Example_

```
{
    "order_detail": {
        "id": 314,
        "order_id": 326,
        "product_id": 12583,
        "attribute_id": 0,
        "name": "General Knowledge 2019",
        "quantity": 1,
        "amount": 20,
        "organization_id": 219,
        "status": "delivered",
        "shipment_id": "441188326",
        "shipping_charge": "30.00",
        "product": {
            "id": 12583,
            "user_id": 254,
            "name": "General Knowledge 2019",
            "slug": "",
            "bdpin": "",
            "brand_id": 57,
            "model": "BDPIN10003",
            "sku": "BDPIN10003",
            "description": "\r\n\r\nGeneral Knowledge is the steady awareness towards progress of one’s surroundings. Building knowledge of all significant events and happenings requires consistency in learning on day to day basis and has also become essential for success in all competitions. General knowledge 2019 by Manohar Pandey comes as a comprehensive assimilation of factual information which proves useful for the aspirants of SSC, Bank, Railway, Police, NDA/CDS and Other Exams. With extensive coverage on current affairs, the book presents facts and figures with appropriate use of pictograms, graphics and tables for Simplified Learning and Easy Grasping. The syllabus for General Knowledge is broad and undefined and requires accurate, complete, topical coverage of facts from all walks of life.Covered in 5 chapters, one for each discipline, the book is a reliable and recommended source of information for anyone appearing in the forthcoming competitive exams.Table of ContentsCurrent AffairsHistory, Geography, Indian Polity, Indian Economy, General Science.\r\n\r\n",
            "specification": "\r\n\r\nPaperback:&nbsp;160 pagesPublisher:&nbsp;Arihant Publications; Eleventh edition (2018)Language:&nbsp;English\r\n\r\n",
            "weight": "100.00",
            "length": "20.00",
            "width": "0.60",
            "height": "13.00",
            "amount": "20.00",
            "quantity": 124,
            "status": 1,
            "source": "bigly",
            "source_id": null,
            "created_at": "2018-02-20 15:49:34",
            "updated_at": "2018-05-30 17:27:28",
            "min_price": "20.00",
            "max_price": "50.00",
            "shipping_charge": "30.00",
            "brand_name": "By Manohar Pandey",
            "brand": {
                "id": 57,
                "name": "By Manohar Pandey"
            },
            "media": [
                {
                    "id": 27558,
                    "mime": "image/jpeg",
                    "thumb": "http://s.bigly.io/products/thumb/1519121995-41cme4z8c.jpg",
                    "small": "http://s.bigly.io/products/small/1519121995-41cme4z8c.jpg",
                    "medium": "http://s.bigly.io/products/medium/1519121995-41cme4z8c.jpg",
                    "large": "http://s.bigly.io/products/large/1519121995-41cme4z8c.jpg",
                    "caption": null,
                    "default": 1,
                    "check": "pending"
                }
            ]
        },
        "order": {
            "id": 326,
            "user_id": 989,
            "client_id": 0,
            "name": "DS_Order_j2rw1ksgIo0Nw6xV",
            "invoice": "",
            "amount": "20.00",
            "created_at": "2018-05-30 12:11:47",
            "updated_at": "2018-05-30 12:11:47",
            "status": "placed",
            "price": "20.00",
            "payment_method": "PREPAID"
        },
        "attribute_data": null,
        "organization": {
            "id": 219,
            "name": "Forbidden Retail"
        }
    },
    "shipping_address": {
        "id": 55,
        "user_id": 989,
        "order_id": 326,
        "name": "Gunjan",
        "email": null,
        "mobile": "7290918926",
        "address": "gaya",
        "street": "gzhzg",
        "colony": "gzhzg",
        "city": "New Dehi",
        "state": "Bihar",
        "landmark": "vzhsj",
        "pincode": "9865325",
        "country": "INDIA",
        "type": "BILLING",
        "status": 1,
        "created_at": "2018-05-30 12:11:47",
        "updated_at": "2018-05-30 12:11:47"
    },
    "responseMessage": "Order Detail",
    "responseCode": 200
}

```



<!-- 24 -->

##  Cancel Reason


**API** `http://localhost:8000/api/reason`

**Method** : Get

### Response :


_Example_

```
{
    "reasons": [
        {
            "id": 1,
            "reason": "rdetjdrf6jureu"
        },
        {
            "id": 2,
            "reason": "this is my reason"
        }
    ]
}
```




<!-- 25 -->

##  Cancel Order


**API** `http://dropship.bigly.io/api/orderCancel/271`

**Method** : Post

### Request :


_Example_

```
{
    "reason_id" : 2,
    "reason" : "Reason Text"
}

```

### Response

```
{
    "order": {
        "id": 271,
        "user_id": "796",
        "client_id": "0",
        "name": "DS_Order_qLvsDGnAyyBqXRM0",
        "invoice": "",
        "amount": "449.00",
        "created_at": "2018-05-10 15:52:41",
        "updated_at": "2018-05-18 12:19:37",
        "status": "cancelled",
        "price": "449.00",
        "payment_method": "PREPAID"
    },
    "reason": {
        "user_id": 796,
        "order_id": "271",
        "reason": "this is reason 2",
        "user_type": "client",
        "reason_type": 2,
        "type": "orders",
        "updated_at": "2018-05-18 12:20:07",
        "created_at": "2018-05-18 12:20:07",
        "id": 7
    },
    "responseMessage": "Order Cancelled",
}
```


<!-- 26 -->

## My Profile 

**API** `http://localhost:8000/api/user`

**Method** : Get

### Response

```

{
    "user": {
        "id": 759,
        "name": "sakshi",
        "username": null,
        "email": "sakshikbc@gmail.com",
        "status": 1,
        "phone": null,
        "created_at": "Apr 13, 2018",
        "updated_at": "2018-05-19 18:09:33",
        "type": "client"
    },
    "address": {
        "id": 25,
        "user_id": 759,
        "order_id": 0,
        "name": "sakshi",
        "email": "sakshikbc@gmail.com",
        "mobile": null,
        "address": "tggggawyhrfgbeyshgfraegegea",
        "street": "10 , 1bgdddddddddddddb",
        "colony": "uygsfukrg",
        "city": "vbycgsvafyk",
        "state": "fsuyf",
        "landmark": "sgfyuesgtes",
        "pincode": "421848",
        "country": "India",
        "type": "BILLING",
        "status": 1,
        "created_at": "2018-05-19 18:09:33",
        "updated_at": "2018-05-19 18:09:33"
    }
}

```


<!-- 27 -->

## Edit Profile 

**API** `http://localhost:8000/api/user/510/edit`

**Method** : Get


### Response

```

{
    "id": 510,
    "name": "client",
    "username": null,
    "email": "client@seller.com",
    "status": 1,
    "phone": "1234567890",
    "created_at": "Mar 03, 2018",
    "updated_at": "2018-03-03 07:23:29",
    "type": "client"
}

```


<!-- 28 -->

## Update Profile 

**API** `http://localhost:8000/api/user/510/update`

**Method** : Post


### Request

```
{
    "name" : "sakshi",
    "email" : "yo@gmail.com",
    "mobile" : "1234567890",
    "address" : "tggggawyhrfgbeyshgfraegegea",
    "street" : "10 , 1bgdddddddddddddb",
    "colony" : "uygsfukrg",
    "city" : "vbycgsvafyk",
    "state" : "fsuyf",
    "landmark" : "sgfyuesgtes",
    "pincode" : 421848,
    "country" : "India",
    "type" : "BILLING"

}

```


### Response

```
{
    "user": {
        "id": 759,
        "name": "sakshi",
        "username": null,
        "email": "sakshikbc@gmail.com",
        "status": 1,
        "phone": null,
        "created_at": "Apr 13, 2018",
        "updated_at": "2018-05-19 18:09:33",
        "type": "client"
    },
    "address": {
        "id": 25,
        "user_id": 759,
        "order_id": 0,
        "name": "sakshi",
        "email": "sakshikbc@gmail.com",
        "mobile": null,
        "address": "tggggawyhrfgbeyshgfraegegea",
        "street": "10 , 1bgdddddddddddddb",
        "colony": "uygsfukrg",
        "city": "vbycgsvafyk",
        "state": "fsuyf",
        "landmark": "sgfyuesgtes",
        "pincode": "421848",
        "country": "India",
        "type": "BILLING",
        "status": 1,
        "created_at": "2018-05-19 18:09:33",
        "updated_at": "2018-05-19 18:09:33"
    }
}
```

<!-- 29 -->

## User Wishlist

**API** `http://dropship.bigly.io/api/userWishlist`

**Method** : Get


### Response

```
{
    "products": {
        "current_page": 1,
        "data": [
            {
                "id": 1,
                "user_id": 1,
                "name": "cfdsgvd",
                "slug": "",
                "bdpin": "1b2327d1-313d-368b-bd91-0638931d5ff5",
                "brand_id": null,
                "model": null,
                "sku": "6b9390ec-1992-3bcb-b658-5743a401ca9c",
                "description": "There was a long tail, certainly,' said Alice, swallowing down her anger as well as if nothing had happened. 'How am I then? Tell me that first, and then, and holding it to be found: all she could.",
                "specification": "",
                "weight": "5904.00",
                "length": "5079.00",
                "width": "8730.00",
                "height": "3265.00",
                "amount": "37.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:54:50",
                "updated_at": "2018-04-06 10:09:16",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "brand_name": "",
                "organization": {
                    "id": 2,
                    "user_id": 2,
                    "type_id": 0,
                    "name": "Ederno",
                    "logo": "http://s.bigly.io/logo/1520848354-mEbtXPl2agzy9vz.jpg",
                    "gst": "",
                    "incorporation_number": "",
                    "address": "N 21 , Above United Bank of India",
                    "introduction": "",
                    "created_at": "2018-03-01 07:36:47",
                    "updated_at": "2018-03-14 10:14:17",
                    "city": "Satna",
                    "state": "Madhya Pradesh",
                    "pincode": "485001",
                    "country": "India"
                },
                "media": [
                    {
                        "id": 2,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/business/2",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/business/2",
                        "large": "http://lorempixel.com/1280/720/business/2",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    }
                ],
                "categories": [
                    {
                        "id": 38,
                        "name": "Keebler-Huels",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 17,
                        "name": "Denesik-Ondricka",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 28,
                        "name": "Lubowitz Group",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ]
            },
            {
                "id": 11,
                "user_id": 1,
                "name": "Bergnaum-Watsica",
                "slug": "",
                "bdpin": "28cdf437-98d1-3fa8-983b-4776a00a76b3",
                "brand_id": null,
                "model": null,
                "sku": "051c0184-e905-31ad-bfd9-35245869b9ca",
                "description": "She is such a subject! Our family always HATED cats: nasty, low, vulgar things! Don't let him know she liked them best, For this must ever be A secret, kept from all the creatures wouldn't be so.",
                "specification": "",
                "weight": "6396.00",
                "length": "251.00",
                "width": "8996.00",
                "height": "8259.00",
                "amount": "43.00",
                "quantity": 0,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-03-01 10:54:50",
                "updated_at": "2018-03-01 10:54:50",
                "min_price": "0.00",
                "max_price": "0.00",
                "shipping_charge": "0.00",
                "attributes": [],
                "brand_name": "",
                "organization": null,
                "media": [
                    {
                        "id": 42,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/food/2",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/food/2",
                        "large": "http://lorempixel.com/1280/720/food/2",
                        "caption": null,
                        "default": 1,
                        "check": "pending"
                    },
                    {
                        "id": 43,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/people/2",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/people/2",
                        "large": "http://lorempixel.com/1280/720/people/2",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    },
                    {
                        "id": 44,
                        "mime": "",
                        "thumb": "http://lorempixel.com/270/220/nature/2",
                        "small": null,
                        "medium": "http://lorempixel.com/480/360/nature/2",
                        "large": "http://lorempixel.com/1280/720/nature/2",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ],
                "categories": [
                    {
                        "id": 19,
                        "name": "Carroll-Swaniawski",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    },
                    {
                        "id": 42,
                        "name": "Spencer Group",
                        "description": "",
                        "meta_title": "",
                        "meta_des": "",
                        "meta_keywords": "",
                        "slug": "",
                        "parent_id": null,
                        "status": 1
                    }
                ]
            },
            {
                "id": 1011,
                "user_id": 2,
                "name": "sZEfgfr",
                "slug": "",
                "bdpin": "",
                "brand_id": 9,
                "model": "sdgdsgsd",
                "sku": "sdxg",
                "description": "jhgjhg",
                "specification": "srgsde",
                "weight": "15.00",
                "length": "55.00",
                "width": "55.00",
                "height": "5.00",
                "amount": "21.00",
                "quantity": 533,
                "status": 1,
                "source": "bigly",
                "source_id": null,
                "created_at": "2018-05-02 18:11:59",
                "updated_at": "2018-05-18 12:52:17",
                "min_price": "121.00",
                "max_price": "1200.00",
                "shipping_charge": "2.00",
                "attributes": [
                    {
                        "id": 16,
                        "value": "0000FF",
                        "quantity": null,
                        "price": null,
                        "name": "color",
                        "attr_id": 2,
                        "children": [
                            {
                                "id": 17,
                                "value": "50",
                                "quantity": 20,
                                "price": null,
                                "attr_id": 3,
                                "name": "size"
                            }
                        ]
                    }
                ],
                "brand_name": "dsgesdge",
                "organization": {
                    "id": 2,
                    "user_id": 2,
                    "type_id": 0,
                    "name": "Ederno",
                    "logo": "http://s.bigly.io/logo/1520848354-mEbtXPl2agzy9vz.jpg",
                    "gst": "",
                    "incorporation_number": "",
                    "address": "N 21 , Above United Bank of India",
                    "introduction": "",
                    "created_at": "2018-03-01 07:36:47",
                    "updated_at": "2018-03-14 10:14:17",
                    "city": "Satna",
                    "state": "Madhya Pradesh",
                    "pincode": "485001",
                    "country": "India"
                },
                "media": [
                    {
                        "id": 4683,
                        "mime": "image/jpeg",
                        "thumb": "http://s.bigly.io/products/thumb/zkqr1y4lujen9ks-9htf1uw.jpg",
                        "small": "http://s.bigly.io/products/small/zkqr1y4lujen9ks-9htf1uw.jpg",
                        "medium": "http://s.bigly.io/products/medium/zkqr1y4lujen9ks-9htf1uw.jpg",
                        "large": "http://s.bigly.io/products/large/zkqr1y4lujen9ks-9htf1uw.jpg",
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ],
                "categories": []
            }
        ],
        "from": 1,
        "last_page": 1,
        "next_page_url": null,
        "path": "http://localhost:8000/api/userWishlist",
        "per_page": 15,
        "prev_page_url": null,
        "to": 3,
        "total": 3
    },
    "reponse_message": "wishlist found"
}
```

<!-- 30 -->

## Get Faqs

**API** `http://dropship.bigly.io/api/faqs`

**Method** : Get


### Response

```
{
    "data": [
        {
            "que": "What is Bigly",
            "ans": "BigLy is Ecommerce platform tool"
        },
        {
            "que": "What is pricing",
            "ans": "Goto app.bigly.io/pricing to check pricing"
        }
    ]
}
```




<!-- 31-->

## Update Faqs

**API** `http://dropship.bigly.io/api/updateFaq`

**Method** : Post


### Response

```
{
    "data": [
        {
            "que": "What is Bigly",
            "ans": "BigLy is Ecommerce platform tool"
        },
        {
            "que": "What is pricing",
            "ans": "Goto app.bigly.io/pricing to check pricing"
        }
    ]
}
```

<!-- 31 -->



##  All Notifications

**API** `http://localhost:8000/api/notifications`

**Method** : Get

### Response :

_Example_

```
{
    "notifications": [
        {
            "id": 4880,
            "user_id": 989,
            "message_id": 3020,
            "status": "unseen",
            "created_at": "2018-05-30 16:12:27",
            "updated_at": "2018-05-30 16:12:27",
            "type": null,
            "message": {
                "id": 3020,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       70 to 72 .<br>Thankyou",
                "created_at": "2018-05-30 16:12:27",
                "updated_at": "2018-05-30 16:12:27",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 4930,
            "user_id": 989,
            "message_id": 3070,
            "status": "unseen",
            "created_at": "2018-05-30 16:16:38",
            "updated_at": "2018-05-30 16:16:38",
            "type": null,
            "message": {
                "id": 3070,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       75 to 78 .<br>Thankyou",
                "created_at": "2018-05-30 16:16:38",
                "updated_at": "2018-05-30 16:16:38",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 4961,
            "user_id": 989,
            "message_id": 3101,
            "status": "unseen",
            "created_at": "2018-05-30 16:18:47",
            "updated_at": "2018-05-30 16:18:47",
            "type": null,
            "message": {
                "id": 3101,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       78 to 80 .<br>Thankyou",
                "created_at": "2018-05-30 16:18:47",
                "updated_at": "2018-05-30 16:18:47",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 4992,
            "user_id": 989,
            "message_id": 3132,
            "status": "unseen",
            "created_at": "2018-05-30 17:07:44",
            "updated_at": "2018-05-30 17:07:44",
            "type": null,
            "message": {
                "id": 3132,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       80 to 82 .<br>Thankyou",
                "created_at": "2018-05-30 17:07:44",
                "updated_at": "2018-05-30 17:07:44",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5023,
            "user_id": 989,
            "message_id": 3163,
            "status": "unseen",
            "created_at": "2018-05-30 17:08:36",
            "updated_at": "2018-05-30 17:08:36",
            "type": null,
            "message": {
                "id": 3163,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       82 to 85 .<br>Thankyou",
                "created_at": "2018-05-30 17:08:36",
                "updated_at": "2018-05-30 17:08:36",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5054,
            "user_id": 989,
            "message_id": 3194,
            "status": "unseen",
            "created_at": "2018-05-30 17:10:32",
            "updated_at": "2018-05-30 17:10:32",
            "type": null,
            "message": {
                "id": 3194,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       85 to 88 .<br>Thankyou",
                "created_at": "2018-05-30 17:10:32",
                "updated_at": "2018-05-30 17:10:32",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5085,
            "user_id": 989,
            "message_id": 3225,
            "status": "unseen",
            "created_at": "2018-05-30 17:11:29",
            "updated_at": "2018-05-30 17:11:29",
            "type": null,
            "message": {
                "id": 3225,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       88 to 91 .<br>Thankyou",
                "created_at": "2018-05-30 17:11:29",
                "updated_at": "2018-05-30 17:11:29",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5116,
            "user_id": 989,
            "message_id": 3256,
            "status": "unseen",
            "created_at": "2018-05-30 17:12:23",
            "updated_at": "2018-05-30 17:12:23",
            "type": null,
            "message": {
                "id": 3256,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       91 to 94 .<br>Thankyou",
                "created_at": "2018-05-30 17:12:23",
                "updated_at": "2018-05-30 17:12:23",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5147,
            "user_id": 989,
            "message_id": 3287,
            "status": "unseen",
            "created_at": "2018-05-30 17:12:45",
            "updated_at": "2018-05-30 17:12:45",
            "type": null,
            "message": {
                "id": 3287,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       94 to 97 .<br>Thankyou",
                "created_at": "2018-05-30 17:12:45",
                "updated_at": "2018-05-30 17:12:45",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5178,
            "user_id": 989,
            "message_id": 3318,
            "status": "unseen",
            "created_at": "2018-05-30 17:13:06",
            "updated_at": "2018-05-30 17:13:06",
            "type": null,
            "message": {
                "id": 3318,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       97 to 100 .<br>Thankyou",
                "created_at": "2018-05-30 17:13:06",
                "updated_at": "2018-05-30 17:13:06",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5209,
            "user_id": 989,
            "message_id": 3349,
            "status": "unseen",
            "created_at": "2018-05-30 17:13:55",
            "updated_at": "2018-05-30 17:13:55",
            "type": null,
            "message": {
                "id": 3349,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       100 to 103 .<br>Thankyou",
                "created_at": "2018-05-30 17:13:55",
                "updated_at": "2018-05-30 17:13:55",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5240,
            "user_id": 989,
            "message_id": 3380,
            "status": "unseen",
            "created_at": "2018-05-30 17:14:13",
            "updated_at": "2018-05-30 17:14:13",
            "type": null,
            "message": {
                "id": 3380,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       103 to 106 .<br>Thankyou",
                "created_at": "2018-05-30 17:14:13",
                "updated_at": "2018-05-30 17:14:13",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5271,
            "user_id": 989,
            "message_id": 3411,
            "status": "unseen",
            "created_at": "2018-05-30 17:14:15",
            "updated_at": "2018-05-30 17:14:15",
            "type": null,
            "message": {
                "id": 3411,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       106 to 109 .<br>Thankyou",
                "created_at": "2018-05-30 17:14:15",
                "updated_at": "2018-05-30 17:14:15",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5302,
            "user_id": 989,
            "message_id": 3442,
            "status": "unseen",
            "created_at": "2018-05-30 17:14:17",
            "updated_at": "2018-05-30 17:14:17",
            "type": null,
            "message": {
                "id": 3442,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       109 to 112 .<br>Thankyou",
                "created_at": "2018-05-30 17:14:17",
                "updated_at": "2018-05-30 17:14:17",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5333,
            "user_id": 989,
            "message_id": 3473,
            "status": "unseen",
            "created_at": "2018-05-30 17:14:53",
            "updated_at": "2018-05-30 17:14:53",
            "type": null,
            "message": {
                "id": 3473,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       112 to 114 .<br>Thankyou",
                "created_at": "2018-05-30 17:14:53",
                "updated_at": "2018-05-30 17:14:53",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5364,
            "user_id": 989,
            "message_id": 3504,
            "status": "unseen",
            "created_at": "2018-05-30 17:15:11",
            "updated_at": "2018-05-30 17:15:11",
            "type": null,
            "message": {
                "id": 3504,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       114 to 116 .<br>Thankyou",
                "created_at": "2018-05-30 17:15:11",
                "updated_at": "2018-05-30 17:15:11",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5395,
            "user_id": 989,
            "message_id": 3535,
            "status": "unseen",
            "created_at": "2018-05-30 17:16:11",
            "updated_at": "2018-05-30 17:16:11",
            "type": null,
            "message": {
                "id": 3535,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       116 to 118 .<br>Thankyou",
                "created_at": "2018-05-30 17:16:11",
                "updated_at": "2018-05-30 17:16:11",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5426,
            "user_id": 989,
            "message_id": 3566,
            "status": "unseen",
            "created_at": "2018-05-30 17:16:25",
            "updated_at": "2018-05-30 17:16:25",
            "type": null,
            "message": {
                "id": 3566,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       118 to 120 .<br>Thankyou",
                "created_at": "2018-05-30 17:16:25",
                "updated_at": "2018-05-30 17:16:25",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5457,
            "user_id": 989,
            "message_id": 3597,
            "status": "unseen",
            "created_at": "2018-05-30 17:17:22",
            "updated_at": "2018-05-30 17:17:22",
            "type": null,
            "message": {
                "id": 3597,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       120 to 122 .<br>Thankyou",
                "created_at": "2018-05-30 17:17:22",
                "updated_at": "2018-05-30 17:17:22",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5488,
            "user_id": 989,
            "message_id": 3628,
            "status": "unseen",
            "created_at": "2018-05-30 17:27:29",
            "updated_at": "2018-05-30 17:27:29",
            "type": null,
            "message": {
                "id": 3628,
                "subject": "Change in Product Quantity",
                "message": "Dear BiglyShipper,<br>There is a major Information for you. Just Now, Supplier has changed Quantity of General Knowledge 2019 . Now the Quantity of <b>'General Knowledge 2019 '</b> is changed from       122 to 124 .<br>Thankyou",
                "created_at": "2018-05-30 17:27:29",
                "updated_at": "2018-05-30 17:27:29",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5489,
            "user_id": 989,
            "message_id": 3629,
            "status": "unseen",
            "created_at": "2018-05-31 10:54:24",
            "updated_at": "2018-05-31 10:54:24",
            "type": null,
            "message": {
                "id": 3629,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 10:54:24",
                "updated_at": "2018-05-31 10:54:24",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5490,
            "user_id": 989,
            "message_id": 3630,
            "status": "unseen",
            "created_at": "2018-05-31 10:55:24",
            "updated_at": "2018-05-31 10:55:24",
            "type": null,
            "message": {
                "id": 3630,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 10:55:24",
                "updated_at": "2018-05-31 10:55:24",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5491,
            "user_id": 989,
            "message_id": 3631,
            "status": "unseen",
            "created_at": "2018-05-31 11:15:25",
            "updated_at": "2018-05-31 11:15:25",
            "type": null,
            "message": {
                "id": 3631,
                "subject": "Your Order has been' . shipped ",
                "message": "",
                "created_at": "2018-05-31 11:15:25",
                "updated_at": "2018-05-31 11:15:25",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5492,
            "user_id": 989,
            "message_id": 3632,
            "status": "unseen",
            "created_at": "2018-05-31 11:15:33",
            "updated_at": "2018-05-31 11:15:33",
            "type": null,
            "message": {
                "id": 3632,
                "subject": "Your Order has been' . delivered ",
                "message": "",
                "created_at": "2018-05-31 11:15:33",
                "updated_at": "2018-05-31 11:15:33",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5493,
            "user_id": 989,
            "message_id": 3633,
            "status": "unseen",
            "created_at": "2018-05-31 11:16:46",
            "updated_at": "2018-05-31 11:16:46",
            "type": null,
            "message": {
                "id": 3633,
                "subject": "Your Order has beenshipped",
                "message": "",
                "created_at": "2018-05-31 11:16:46",
                "updated_at": "2018-05-31 11:16:46",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5494,
            "user_id": 989,
            "message_id": 3634,
            "status": "unseen",
            "created_at": "2018-05-31 11:17:14",
            "updated_at": "2018-05-31 11:17:14",
            "type": null,
            "message": {
                "id": 3634,
                "subject": "Your Order has been delivered",
                "message": "",
                "created_at": "2018-05-31 11:17:14",
                "updated_at": "2018-05-31 11:17:14",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5495,
            "user_id": 989,
            "message_id": 3635,
            "status": "unseen",
            "created_at": "2018-05-31 13:00:33",
            "updated_at": "2018-05-31 13:00:33",
            "type": null,
            "message": {
                "id": 3635,
                "subject": "Your Order has been shipped",
                "message": "",
                "created_at": "2018-05-31 13:00:33",
                "updated_at": "2018-05-31 13:00:33",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5496,
            "user_id": 989,
            "message_id": 3636,
            "status": "unseen",
            "created_at": "2018-05-31 13:00:51",
            "updated_at": "2018-05-31 13:00:51",
            "type": null,
            "message": {
                "id": 3636,
                "subject": "Your Order has been delivered",
                "message": "",
                "created_at": "2018-05-31 13:00:51",
                "updated_at": "2018-05-31 13:00:51",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5497,
            "user_id": 989,
            "message_id": 3637,
            "status": "unseen",
            "created_at": "2018-05-31 13:01:21",
            "updated_at": "2018-05-31 13:01:21",
            "type": null,
            "message": {
                "id": 3637,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:01:21",
                "updated_at": "2018-05-31 13:01:21",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5498,
            "user_id": 989,
            "message_id": 3638,
            "status": "unseen",
            "created_at": "2018-05-31 13:05:14",
            "updated_at": "2018-05-31 13:05:14",
            "type": null,
            "message": {
                "id": 3638,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:05:14",
                "updated_at": "2018-05-31 13:05:14",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5499,
            "user_id": 989,
            "message_id": 3639,
            "status": "unseen",
            "created_at": "2018-05-31 13:05:30",
            "updated_at": "2018-05-31 13:05:30",
            "type": null,
            "message": {
                "id": 3639,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:05:30",
                "updated_at": "2018-05-31 13:05:30",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5500,
            "user_id": 989,
            "message_id": 3640,
            "status": "unseen",
            "created_at": "2018-05-31 13:05:46",
            "updated_at": "2018-05-31 13:05:46",
            "type": null,
            "message": {
                "id": 3640,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:05:46",
                "updated_at": "2018-05-31 13:05:46",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5501,
            "user_id": 989,
            "message_id": 3641,
            "status": "unseen",
            "created_at": "2018-05-31 13:05:56",
            "updated_at": "2018-05-31 13:05:56",
            "type": null,
            "message": {
                "id": 3641,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:05:56",
                "updated_at": "2018-05-31 13:05:56",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5502,
            "user_id": 989,
            "message_id": 3642,
            "status": "unseen",
            "created_at": "2018-05-31 13:06:04",
            "updated_at": "2018-05-31 13:06:04",
            "type": null,
            "message": {
                "id": 3642,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:06:04",
                "updated_at": "2018-05-31 13:06:04",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5503,
            "user_id": 989,
            "message_id": 3643,
            "status": "unseen",
            "created_at": "2018-05-31 13:06:25",
            "updated_at": "2018-05-31 13:06:25",
            "type": null,
            "message": {
                "id": 3643,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:06:25",
                "updated_at": "2018-05-31 13:06:25",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5504,
            "user_id": 989,
            "message_id": 3644,
            "status": "unseen",
            "created_at": "2018-05-31 13:06:41",
            "updated_at": "2018-05-31 13:06:41",
            "type": null,
            "message": {
                "id": 3644,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:06:41",
                "updated_at": "2018-05-31 13:06:41",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5505,
            "user_id": 989,
            "message_id": 3645,
            "status": "unseen",
            "created_at": "2018-05-31 13:06:57",
            "updated_at": "2018-05-31 13:06:57",
            "type": null,
            "message": {
                "id": 3645,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:06:57",
                "updated_at": "2018-05-31 13:06:57",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5506,
            "user_id": 989,
            "message_id": 3646,
            "status": "unseen",
            "created_at": "2018-05-31 13:07:41",
            "updated_at": "2018-05-31 13:07:41",
            "type": null,
            "message": {
                "id": 3646,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:07:41",
                "updated_at": "2018-05-31 13:07:41",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5507,
            "user_id": 989,
            "message_id": 3647,
            "status": "unseen",
            "created_at": "2018-05-31 13:07:48",
            "updated_at": "2018-05-31 13:07:48",
            "type": null,
            "message": {
                "id": 3647,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:07:48",
                "updated_at": "2018-05-31 13:07:48",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5508,
            "user_id": 989,
            "message_id": 3648,
            "status": "unseen",
            "created_at": "2018-05-31 13:08:15",
            "updated_at": "2018-05-31 13:08:15",
            "type": null,
            "message": {
                "id": 3648,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:08:15",
                "updated_at": "2018-05-31 13:08:15",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5509,
            "user_id": 989,
            "message_id": 3649,
            "status": "unseen",
            "created_at": "2018-05-31 13:10:04",
            "updated_at": "2018-05-31 13:10:04",
            "type": null,
            "message": {
                "id": 3649,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:10:04",
                "updated_at": "2018-05-31 13:10:04",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5510,
            "user_id": 989,
            "message_id": 3650,
            "status": "unseen",
            "created_at": "2018-05-31 13:10:24",
            "updated_at": "2018-05-31 13:10:24",
            "type": null,
            "message": {
                "id": 3650,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:10:24",
                "updated_at": "2018-05-31 13:10:24",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5511,
            "user_id": 989,
            "message_id": 3651,
            "status": "unseen",
            "created_at": "2018-05-31 13:12:14",
            "updated_at": "2018-05-31 13:12:14",
            "type": null,
            "message": {
                "id": 3651,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 13:12:14",
                "updated_at": "2018-05-31 13:12:14",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5512,
            "user_id": 989,
            "message_id": 3652,
            "status": "unseen",
            "created_at": "2018-05-31 14:10:25",
            "updated_at": "2018-05-31 14:10:25",
            "type": null,
            "message": {
                "id": 3652,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 14:10:25",
                "updated_at": "2018-05-31 14:10:25",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5513,
            "user_id": 989,
            "message_id": 3653,
            "status": "unseen",
            "created_at": "2018-05-31 14:11:07",
            "updated_at": "2018-05-31 14:11:07",
            "type": null,
            "message": {
                "id": 3653,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 14:11:07",
                "updated_at": "2018-05-31 14:11:07",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5514,
            "user_id": 989,
            "message_id": 3654,
            "status": "unseen",
            "created_at": "2018-05-31 15:05:34",
            "updated_at": "2018-05-31 15:05:34",
            "type": null,
            "message": {
                "id": 3654,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 15:05:34",
                "updated_at": "2018-05-31 15:05:34",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5515,
            "user_id": 989,
            "message_id": 3655,
            "status": "unseen",
            "created_at": "2018-05-31 15:07:56",
            "updated_at": "2018-05-31 15:07:56",
            "type": null,
            "message": {
                "id": 3655,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 15:07:56",
                "updated_at": "2018-05-31 15:07:56",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        },
        {
            "id": 5516,
            "user_id": 989,
            "message_id": 3656,
            "status": "unseen",
            "created_at": "2018-05-31 15:08:21",
            "updated_at": "2018-05-31 15:08:21",
            "type": null,
            "message": {
                "id": 3656,
                "subject": "Congratulations !! Notification Done",
                "message": "",
                "created_at": "2018-05-31 15:08:21",
                "updated_at": "2018-05-31 15:08:21",
                "expires_at": "0000-00-00 00:00:00",
                "type": ""
            }
        }
    ]
}
```

<!-- 33 -->

##  Check Profile Api (Get)

**API** `http://localhost:8000/api/user/check`

**Method** : GET

### Response :

_Example_

```
{
    "user_detail": 1,
    "billing_address": 1,
    "shipping_address": 0,
    "bank_details": 1
}

```

<!-- 34 -->


##  View Bank Details of user

**API** `http://localhost:8000/api/bank/details`

**Method** : GET

### Response :

_Example_

```
{
    "bank": {
        "id": 121,
        "user_id": 989,
        "organization_id": 951,
        "bank_name": "nkanikefwa",
        "account_number": "27974374979479",
        "account_holder_name": "sakshi",
        "IFSC_code": "UZXNDJD"
    },
    "responseCode": 200,
    "responseMessage": "Bank Details Found"
}
```



<!-- 35 -->


##  Insert or Update Bank Details

**API** `http://localhost:8000/api/bank/details`

**Method** : Post

### Request :

_Example_

```
{
    "bank_name" : "nkanikefwa",
    "account_number" : 27974374979479,
    "account_holder_name" : "sakshi",
    "IFSC_code" : "UZXNDJD" 
}
```


### Response
```
{
    "bank": {
        "id": 121,
        "user_id": 989,
        "organization_id": 951,
        "bank_name": "nkanikefwa",
        "account_number": "27974374979479",
        "account_holder_name": "sakshi",
        "IFSC_code": "UZXNDJD"
    },
    "responseCode": 200,
    "responseMessage": "Bank Details Found"
}
```


<!-- 36 -->

##  View Particular Query

**API** `http://localhost:8000/api/contact/110`

**Method** : GET

### Response :

_Example_

```
{
    "query": {
        "id": 110,
        "subject": "gunjan test",
        "email": "7898888758@app.com",
        "message": "testing",
        "created_at": "2018-06-18 13:01:57",
        "updated_at": "2018-06-18 13:01:57",
        "status": "open",
        "replies": [
            {
                "id": 58,
                "user_id": 6,
                "contactus_id": 110,
                "subject": "",
                "message": "<p>sakshi repliing</p>",
                "created_at": "2018-06-18 13:02:32",
                "updated_at": "2018-06-18 13:02:32",
                "user": {
                    "id": 6,
                    "name": "Md Adil",
                    "username": "adil",
                    "email": "md-adil@live.com",
                    "status": 1,
                    "phone": null,
                    "created_at": "Jun 18, 2018",
                    "updated_at": null,
                    "type": "super_user"
                },
                "media": [
                    {
                        "id": 71004,
                        "mime": "",
                        "thumb": "http://s.bigly.io/reply/1529307152-C83MM2RjAZeVNZj.jpeg",
                        "small": null,
                        "medium": null,
                        "large": null,
                        "caption": null,
                        "default": 0,
                        "check": "pending"
                    }
                ]
            },
            {
                "id": 59,
                "user_id": 6,
                "contactus_id": 110,
                "subject": "",
                "message": "<p>sakshi again replying</p>",
                "created_at": "2018-06-18 13:03:03",
                "updated_at": "2018-06-18 13:03:03",
                "user": {
                    "id": 6,
                    "name": "Md Adil",
                    "username": "adil",
                    "email": "md-adil@live.com",
                    "status": 1,
                    "phone": null,
                    "created_at": "Jun 18, 2018",
                    "updated_at": null,
                    "type": "super_user"
                },
                "media": []
            }
        ]
    },
    "response_code": 200,
    "response_message": "Query"
}
```


<!-- 37 -->

##  All Queries of user

**API** `http://localhost:8000/api/queries`

**Method** : GET

### Response :

_Example_

```
{
    "queries": [
        {
            "id": 108,
            "subject": "sfgsgras",
            "email": "7898888758@app.com",
            "message": "ayhdgef",
            "created_at": "2018-06-18 12:20:30",
            "updated_at": "2018-06-18 12:20:30",
            "status": "open",
            "replies": [
                {
                    "id": 55,
                    "user_id": 6,
                    "contactus_id": 108,
                    "subject": "",
                    "message": "<p>yo</p>",
                    "created_at": "2018-06-18 12:53:01",
                    "updated_at": "2018-06-18 12:53:01",
                    "user": {
                        "id": 6,
                        "name": "Md Adil",
                        "username": "adil",
                        "email": "md-adil@live.com",
                        "status": 1,
                        "phone": null,
                        "created_at": "Jun 18, 2018",
                        "updated_at": null,
                        "type": "super_user"
                    },
                    "media": []
                }
            ]
        },
        {
            "id": 109,
            "subject": "testing",
            "email": "7898888758@app.com",
            "message": "tototot",
            "created_at": "2018-06-18 12:55:07",
            "updated_at": "2018-06-18 12:55:07",
            "status": "open",
            "replies": [
                {
                    "id": 56,
                    "user_id": 6,
                    "contactus_id": 109,
                    "subject": "",
                    "message": "<p>ssfvseng</p>",
                    "created_at": "2018-06-18 12:55:32",
                    "updated_at": "2018-06-18 12:55:32",
                    "user": {
                        "id": 6,
                        "name": "Md Adil",
                        "username": "adil",
                        "email": "md-adil@live.com",
                        "status": 1,
                        "phone": null,
                        "created_at": "Jun 18, 2018",
                        "updated_at": null,
                        "type": "super_user"
                    },
                    "media": [
                        {
                            "id": 71003,
                            "mime": "",
                            "thumb": "http://s.bigly.io/reply/1529306732-i6nai6pVYfmkfXk.jpeg",
                            "small": null,
                            "medium": null,
                            "large": null,
                            "caption": null,
                            "default": 0,
                            "check": "pending"
                        }
                    ]
                },
                {
                    "id": 57,
                    "user_id": 6,
                    "contactus_id": 109,
                    "subject": "",
                    "message": "<p>sdnkefpkem</p><p><br></p>",
                    "created_at": "2018-06-18 12:57:23",
                    "updated_at": "2018-06-18 12:57:23",
                    "user": {
                        "id": 6,
                        "name": "Md Adil",
                        "username": "adil",
                        "email": "md-adil@live.com",
                        "status": 1,
                        "phone": null,
                        "created_at": "Jun 18, 2018",
                        "updated_at": null,
                        "type": "super_user"
                    },
                    "media": []
                }
            ]
        },
        {
            "id": 110,
            "subject": "gunjan test",
            "email": "7898888758@app.com",
            "message": "testing",
            "created_at": "2018-06-18 13:01:57",
            "updated_at": "2018-06-18 13:01:57",
            "status": "open",
            "replies": [
                {
                    "id": 58,
                    "user_id": 6,
                    "contactus_id": 110,
                    "subject": "",
                    "message": "<p>sakshi repliing</p>",
                    "created_at": "2018-06-18 13:02:32",
                    "updated_at": "2018-06-18 13:02:32",
                    "user": {
                        "id": 6,
                        "name": "Md Adil",
                        "username": "adil",
                        "email": "md-adil@live.com",
                        "status": 1,
                        "phone": null,
                        "created_at": "Jun 18, 2018",
                        "updated_at": null,
                        "type": "super_user"
                    },
                    "media": [
                        {
                            "id": 71004,
                            "mime": "",
                            "thumb": "http://s.bigly.io/reply/1529307152-C83MM2RjAZeVNZj.jpeg",
                            "small": null,
                            "medium": null,
                            "large": null,
                            "caption": null,
                            "default": 0,
                            "check": "pending"
                        }
                    ]
                },
                {
                    "id": 59,
                    "user_id": 6,
                    "contactus_id": 110,
                    "subject": "",
                    "message": "<p>sakshi again replying</p>",
                    "created_at": "2018-06-18 13:03:03",
                    "updated_at": "2018-06-18 13:03:03",
                    "user": {
                        "id": 6,
                        "name": "Md Adil",
                        "username": "adil",
                        "email": "md-adil@live.com",
                        "status": 1,
                        "phone": null,
                        "created_at": "Jun 18, 2018",
                        "updated_at": null,
                        "type": "super_user"
                    },
                    "media": []
                }
            ]
        }
    ],
    "response_code": 200,
    "response_message": "All Queries"
}
```

<!-- 38 -->

##  Reply on a Query

**API** `http://localhost:8000/api/reply/{contactus_id}`
        `http://localhost:8000/api/reply/110`

**Method** : Post

### Request :

_Example_

```
{
    "message": "tototot"
}
```

### Response

```
{
    "id": 104,
    "user_id": "1033",
    "contactus_id": "133",
    "subject": "",
    "message": "testing",
    "created_at": "2018-06-19 16:56:25",
    "updated_at": "2018-06-19 16:56:25",
    "user": {
        "id": 1033,
        "name": "Gunjan Kumar",
        "username": null,
        "email": "gunjan@gmail.com",
        "status": "1",
        "phone": "449606792",
        "created_at": "May 24, 2018",
        "updated_at": "2018-06-18 18:48:18",
        "type": "admin"
    },
    "media": []
}
```


<!-- 38 -->

##  Get Setting Notification

**API** `http://localhost:8000/api/settings/notification`

**Method** : GET

### Response :

_Example_

```
{
    "status": "1"
}
```


<!-- 38 -->

##  Update Notification Setting

**API** `http://localhost:8000/api/settings/notification`

**Method** : POST

### Response :

_Example_

```
{
    "status": "1"
}
```



