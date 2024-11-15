# `collection` resource

Base endpoint:

```shell

{base_url}/collections
```

The `collection` resource contains details pertinent to the book collection. A `collection` may be blank, or include one or more books.

## Resource properties

Sample `user` resource

```js

{
      "collection_id": 101,
      "user_id": 1,
      "name": "Favorite Classics",
      "privacy": "private",
      "created_at": "2023-08-15",
      "books": [
        {
          "book_id": 26,
          "title": "Wuthering Heights",
          "author": "Emily Brontë",
          "isbn": "NA",
          "edition": "US First Edition",
          "year": "1848",
          "publisher": "Harper & Brothers",
          "cover type": "Cloth",
          "condition": "Good",
          "price": "$17,500",
          "seller": "Heritage Books Haven",
          "language": "English",
          "status": "Acquired",
        }
}
```

##Properties
| Property name | Type | Description | Required? |
| ------------- | ----------- | ----------- | ----------- |
| `collection_id` | number | ID of the collection | Yes |
| `user_id` | number | User's ID  | Yes |
| `name` | string | Title for the collection  | Yes |
| `privacy` | string | [Privacy level of the collection](https://github.com/cnjoyce1225/the-archivist/blob/9dbb03c52f3094ad080aaba5c88647ca44a9ed16/Docs/References/privacy.md)  | Yes |
| `created_at` | string | Date the collection was created  | Yes |
| `books` | array | List of books in the collection  | No |

## READ

* 
