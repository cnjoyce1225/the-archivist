

# `collection` resource
The `collection` resource contains details pertinent to the book collection. A `collection` may be blank, or include one or more books.


## Sample `collection` resource

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
          "status": "Acquired"
        }
}
```

## `Collection` Properties

The properies of a `collection` are as follows:

| Property name | Type | Description | Required? |
| ------------- | ----------- | ----------- | ----------- |
| `collection_id` | number | ID of the collection | Yes |
| `user_id` | number | User's ID  | Yes |
| `name` | string | Title for the collection  | Yes |
| `privacy` | string | [Privacy level of the collection](privacy.md)  | Yes |
| `created_at` | string | Date the collection was created  | Yes |
| *`books` | array | List of books in the collection  | No |  
        
  
*The `books` property has its own properties:

| Property name | Type | Description | Required? |
| ------------- | ----------- | ----------- | ----------- |
| `book_id` | number | ID of the book in the user's database | Yes |
| `title` | number | Book's title  | Yes |
| `author` | string | Book's author  | No |
| `isbn` | string | Book's ISBN code  | Yes |
| `edition` | number | Book's edition  | No |
| `year` | number | Year the book was published  | No |
| `publisher` | string | Book's publishing company | No |
| `cover_type` | string | Type of the book's cover  | No |
| `condition` | string | Condition of the book  | No |
| `price` | number | Price paid for the book | No |
| `seller` | string | Store the book was purchased from  | No |
| `language` | string | Language the book's text is in  | No |
| **`status` | string | `wishilist`, `acquired`, `partially_read`, or `fully_read`  | No |

**The meanings behind each `status` are:
* `wishlist`: the user doesn't possess the book yet, but would like to purchase it
* `acquired`: the user possesses the book, but has not yet read it
* `partially_read`: the user has read part of the book
* `fully_read`: the user has read the entire book
  


## Actions for `collection`

* [Create collections](./CRUD-topics/add-collections.md)
* [Get collections](./CRUD-topics/get-collections.md)
* [Update collections](./CRUD-topics/update-collections.md)
* [Delete collections](./CRUD-topics/delete-collections.md)

---
### Navigation

* Go to the [user resource](./user.md)

* Go to the [homepage](https://cnjoyce1225.github.io/the-archivist/)
