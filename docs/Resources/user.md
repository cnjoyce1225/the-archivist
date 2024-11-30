# `user` resource

Base endpoint:

```shell

{base_url}/users
```

The `user` resource contains details about the individual using the service.

## Resource properties

| Property name | Type | Description | Required? |
| ------------- | ----------- | ----------- | ----------- |
| `last_name` | string | User's last name | Yes |
| `first_name` | string | User's first name | Yes |
| `privacy` | string | [Privacy level of user](https://github.com/cnjoyce1225/the-archivist/blob/9dbb03c52f3094ad080aaba5c88647ca44a9ed16/Docs/References/privacy.md) | Yes |
| `email` | string | User's email address | Yes |
| `id` | number | User's unique record ID | Yes |

Sample `user` resource

```js

{
    "last_name": "Carter",
    "first_name": "Liam",
    "privacy": "public",
    "email": "liam.carter@example.com",
    "id": 1
}
```


## CRUD actions for `users`

<details><summary>Click here for a list of topics!</summary>

* [Add users](https://github.com/cnjoyce1225/the-archivist/blob/b8a83f17422a7e9a015a7ef29e576512491659e8/Docs/Resources/CRUD-topics/add-users.md)
* [Pull users](https://github.com/cnjoyce1225/the-archivist/blob/b8a83f17422a7e9a015a7ef29e576512491659e8/Docs/Resources/CRUD-topics/get-users.md)
* [Update users](https://github.com/cnjoyce1225/the-archivist/blob/0a5b13bb1411f3ff7b56cb9156a9f87ca316f68f/Docs/Resources/CRUD-topics/update-users.md)
* [Delete users](https://github.com/cnjoyce1225/the-archivist/blob/0a5b13bb1411f3ff7b56cb9156a9f87ca316f68f/Docs/Resources/CRUD-topics/delete-users.md)

</details>
