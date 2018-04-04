# <Project Name> API Documentation

Welcome to the Broadway Lab API Documentation! It's important to create a stable API with clear instructions on how clients can communicate. 

In this section, you should put a brief description of the project. 

## Making a Request

This is information about how you should make a request.

All URLs start with ```https://example.com/api/v1```.

Requests must be authenticated. In cURL, it looks like this:

```
curl -H "Authorization: Bearer $ACCESS_TOKEN" \
  -H 'Content-Type: application/json' \
  -H 'User-Agent: yourname@example.com' \
  https://example.com/api/v1/posts
```

## Authentication

Info about how to authenticate with the API... 

## Pagination

Broadway Lab APIs should follow the [RFC5988](https://tools.ietf.org/html/rfc5988) convention of using the Link header to provide URLs for the next page. Please follow this convention when building an API. 

## Handling Errors 

API clients should expect to gracefully handle errors. 

### 429 - Too Many Requests

If the application is rate limited, 429 should be the response when the rate limit is not achieved. 

### 5xx - Server Errors

When something unexpected happens, the application should return a 5xx status code. 

This may include: 
- [ ] 500 - Internal server error
- [ ] 502 - Bad Gateway
- [ ] 503 - Service Unavailable
- [ ] 504 - Gateway Timeout

### 404 - Not Found
 
 API requests may be 404 due to deleted content, an inaccessible endpoint, or other reasons. 

## API Endpoints

List the resources in alphabetical order. 

- [ ] Author
- [ ] [Comment](/sections/comment.md)
- [ ] Post

## Issues

If you see an issue with this API, please create a bug in the Product Backlog column on this Trello board: https:/trello.com/board-url
