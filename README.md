# `Backend-AgroMarket`


Strapi comes with a full featured [Command Line Interface](https://docs.strapi.io/dev-docs/cli) (CLI) which lets you scaffold and manage your project in seconds.

### `Endpoints`

```
https://clever-eggs-512f1b05ad.strapiapp.com
```

### `Get all Product`


```
GET  /api/products?pagination[page]=1&pagination[pageSize]=34&populate=*
``` 
Example : https://clever-eggs-512f1b05ad.strapiapp.com/api/products?pagination[page]=1&pagination[pageSize]=34&populate=*

### `Get a Single Product`


```
GET  /api/products?filters[id][$in][0]=1&filters[id][$in][1]=7&filters[id][$in][2]=12
```
Example: https://clever-eggs-512f1b05ad.strapiapp.com/api/products?filters[id][$in][0]=1&filters[id][$in][1]=7&filters[id][$in][2]=12

### `Filter Product by Catagary`

```
GET  /api/products?populate=*&filters[category_ids][Name][$eq]=Fruit
```
Example: https://clever-eggs-512f1b05ad.strapiapp.com/api/products?populate=*&filters[category_ids][Name][$eq]=Fruit

### `Response Format`


The API responses will be in JSON format and follow this structure:
Example : data

```
{
    "data": [
        {
            "id": 1,
            "attributes": {
                "productid": 1,
                "name": "Mango ",
                "price": 2.5,
                "quantity": 100,
                "organic": true,
                "originprovince": "Kampong Speu",
                "ownerid": 1,
                "createdAt": "2024-05-21T07:05:09.064Z",
                "updatedAt": "2024-05-21T07:05:58.050Z",
                "publishedAt": "2024-05-21T07:05:58.041Z",
                "images": {
                    "data": {
                        "id": 1,
                        "attributes": {
                            "name": "mango.jpg",
                            "alternativeText": null,
                            "caption": null,
                            "width": 558,
                            "height": 600,
                            "formats": {
                                "small": {
                                    "ext": ".jpg",
                                    "url": "https://clever-eggs-512f1b05ad.media.strapiapp.com/small_mango_b33a21d866.jpg",
                                    "hash": "small_mango_b33a21d866",
                                    "mime": "image/webp",
                                    "name": "small_mango.jpg",
                                    "path": null,
                                    "size": 8.19,
                                    "width": 465,
                                    "height": 500,
                                    "sizeInBytes": 8188
                                },
                                "thumbnail": {
                                    "ext": ".jpg",
                                    "url": "https://clever-eggs-512f1b05ad.media.strapiapp.com/thumbnail_mango_b33a21d866.jpg",
                                    "hash": "thumbnail_mango_b33a21d866",
                                    "mime": "image/webp",
                                    "name": "thumbnail_mango.jpg",
                                    "path": null,
                                    "size": 1.83,
                                    "width": 145,
                                    "height": 156,
                                    "sizeInBytes": 1832
                                }
                            },
                            "hash": "mango_b33a21d866",
                            "ext": ".jpg",
                            "mime": "image/webp",
                            "size": 12.67,
                            "url": "https://clever-eggs-512f1b05ad.media.strapiapp.com/mango_b33a21d866.jpg",
                            "previewUrl": null,
                            "provider": "strapi-provider-upload-strapi-cloud",
                            "provider_metadata": null,
                            "createdAt": "2024-05-21T07:04:58.447Z",
                            "updatedAt": "2024-05-21T07:04:58.447Z"
                        }
                    }
                },
                "category_ids": {
                    "data": [
                        {
                            "id": 1,
                            "attributes": {
                                "CategoryID": 1,
                                "Name": "Fruit",
                                "createdAt": "2024-05-21T07:05:45.226Z",
                                "updatedAt": "2024-05-21T07:05:51.480Z",
                                "publishedAt": "2024-05-21T07:05:51.475Z"
                            }
                        }
                    ]
                },
                "strapi_stage": {
                    "data": null
                },
                "strapi_assignee": {
                    "data": null
                }
            }
        },
```





