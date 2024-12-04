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

* [Add users](./CRUD-topics/add-users.md)
* [Pull users](./CRUD-topics/get-users.md)
* [Update users](./CRUD-topics/update-users.md)
* [Delete users](./CRUD-topics/delete-users.md)

