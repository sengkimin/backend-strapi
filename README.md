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


