# Comments

This is where you should write a description of the resource and include a link to the operations for this resource. Typically, those are going to be CRUD operations. We try and keep APIs RESTful. For example: Comments are ways for users to interact with posts. 

Endpoints: 
- [ ] (Get Comments)[#get-comments]
- [ ] (Get a Comment)[get-a-comment]

### Get Comments

- [ ] ```GET /posts/1/comments``` will return a paginated list of comments. 

###### Example JSON Response
<!-- START GET /posts/1/comments -->
```json
[
  {
    "id": 1000473885,
    "created_at": "2018-04-04T22:22:22.123Z",
    "updated_at": "2018-04-04T22:22:22.123Z",
    "text": "Hello world!",
    "creator": {
      "id": 4000473885,
      "name": "Michael Fellows",
      "email": "michael@broadwaylab.com",
    }
  }
]
```
<!-- END GET GET /posts/1/comments -->

###### Copy as cURL

``` shell
curl -s -H "Authorization: Bearer $ACCESS_TOKEN" https://example.com/api/v1/posts/1/comments
```

### Get a Comment
- [ ] ```GET /posts/1/comments/1``` will return a single of comment.

###### Example JSON Response
<!-- START GET /posts/1/comments -->
```json
{
    "id": 1000473885,
    "created_at": "2018-04-04T22:22:22.123Z",
    "updated_at": "2018-04-04T22:22:22.123Z",
    "text": "Hello world!",
    "creator": {
      "id": 4000473885,
      "name": "Michael Fellows",
      "email": "michael@broadwaylab.com",
    }
}
```
<!-- END GET GET /posts/1/comments -->

###### Copy as cURL

``` shell
curl -s -H "Authorization: Bearer $ACCESS_TOKEN" https://example.com/api/v1/posts/1/comments/1
```
