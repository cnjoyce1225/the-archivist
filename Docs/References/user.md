# `user` resource

Base endpoint:

```shell

{base_url}/users
```

The `user` resource contains details about the individual using the service.

## Resource properties

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `last_name` | string | The user's last name | Required |
| `first_name` | string | The user's first name | Required |
| `privacy` | string | The user's privacy choice | Required |
| `email` | string | The user's email address | Required |
| `id` | number | The user's unique record ID | Required |

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


## READ

* 
