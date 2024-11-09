# `user` resource

Base endpoint:

```shell

{base_url}/users
```

Contains information about the users of the service.

## Resource properties

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

| Property name | Type | Description |
| ------------- | ----------- | ----------- |
| `last_name` | string | The user's last name |
| `first_name` | string | The user's first name |
| `privacy` | string | The user's privacy choice |
| `email` | string | The user's email address |
| `id` | number | The user's unique record ID |

## READ

* 
