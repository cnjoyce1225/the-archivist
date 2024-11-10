# `user` resource

Base endpoint:

```shell

{base_url}/users
```

The `user` resource contains details about the individual using the service.

## Resource properties

| Property name | Type | Description | Required? |
| ------------- | ----------- | ----------- | ----------- |
| `last_name` | string | The user's last name | Yes |
| `first_name` | string | The user's first name | Yes |
| `privacy` | string | The user's privacy choice | Yes |
| `email` | string | The user's email address | Yes |
| `id` | number | The user's unique record ID | Yes |

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
