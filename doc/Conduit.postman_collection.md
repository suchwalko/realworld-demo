
# Conduit

Collection for testing the Conduit API

https://github.com/gothinkster/realworld

## Indices

* [Articles](#articles)

  * [All Articles](#1-all-articles)
  * [Articles by Author](#2-articles-by-author)
  * [Articles Favorited by Username](#3-articles-favorited-by-username)
  * [Articles by Tag](#4-articles-by-tag)

* [Articles, Favorite, Comments](#articles,-favorite,-comments)

  * [Create Article](#1-create-article)
  * [Feed](#2-feed)
  * [All Articles](#3-all-articles)
  * [All Articles with auth](#4-all-articles-with-auth)
  * [Articles by Author](#5-articles-by-author)
  * [Articles by Author with auth](#6-articles-by-author-with-auth)
  * [Articles Favorited by Username](#7-articles-favorited-by-username)
  * [Articles Favorited by Username with auth](#8-articles-favorited-by-username-with-auth)
  * [Single Article by slug](#9-single-article-by-slug)
  * [Articles by Tag](#10-articles-by-tag)
  * [Update Article](#11-update-article)
  * [Favorite Article](#12-favorite-article)
  * [Unfavorite Article](#13-unfavorite-article)
  * [Create Comment for Article](#14-create-comment-for-article)
  * [All Comments for Article](#15-all-comments-for-article)
  * [Delete Comment for Article](#16-delete-comment-for-article)
  * [Delete Article](#17-delete-article)

* [Auth](#auth)

  * [Register](#1-register)
  * [Login](#2-login)
  * [Login and Remember Token](#3-login-and-remember-token)
  * [Current User](#4-current-user)
  * [Update User](#5-update-user)

* [Profiles](#profiles)

  * [Register Celeb](#1-register-celeb)
  * [Profile](#2-profile)
  * [Follow Profile](#3-follow-profile)
  * [Unfollow Profile](#4-unfollow-profile)

* [Tags](#tags)

  * [All Tags](#1-all-tags)


--------


## Articles



### 1. All Articles



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



### 2. Articles by Author



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| author | johnjacob |  |



### 3. Articles Favorited by Username



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| favorited | jane |  |



### 4. Articles by Tag



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| tag | dragons |  |



## Articles, Favorite, Comments



### 1. Create Article



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Body:***

```js        
{"article":{"title":"How to train your dragon", "description":"Ever wonder how?", "body":"Very carefully.", "tagList":["dragons","training"]}}
```



### 2. Feed



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles/feed
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 3. All Articles



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 4. All Articles with auth



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 5. Articles by Author



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| author | {{USERNAME}} |  |



### 6. Articles by Author with auth



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| author | {{USERNAME}} |  |



### 7. Articles Favorited by Username



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| favorited | jane |  |



### 8. Articles Favorited by Username with auth



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| favorited | jane |  |



### 9. Single Article by slug



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles/{{slug}}
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 10. Articles by Tag



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Query params:***

| Key | Value | Description |
| --- | ------|-------------|
| tag | dragons |  |



### 11. Update Article



***Endpoint:***

```bash
Method: PUT
Type: RAW
URL: {{APIURL}}/articles/{{slug}}
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Body:***

```js        
{"article":{"body":"With two hands"}}
```



### 12. Favorite Article



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{APIURL}}/articles/{{slug}}/favorite
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 13. Unfavorite Article



***Endpoint:***

```bash
Method: DELETE
Type: RAW
URL: {{APIURL}}/articles/{{slug}}/favorite
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 14. Create Comment for Article



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{APIURL}}/articles/{{slug}}/comments
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Body:***

```js        
{"comment":{"body":"Thank you so much!"}}
```



### 15. All Comments for Article



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/articles/{{slug}}/comments
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 16. Delete Comment for Article



***Endpoint:***

```bash
Method: DELETE
Type: RAW
URL: {{APIURL}}/articles/{{slug}}/comments/{{commentId}}
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 17. Delete Article



***Endpoint:***

```bash
Method: DELETE
Type: RAW
URL: {{APIURL}}/articles/{{slug}}
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



## Auth



### 1. Register



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{APIURL}}/users
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



***Body:***

```js        
{"user":{"email":"{{EMAIL}}", "password":"{{PASSWORD}}", "username":"{{USERNAME}}"}}
```



### 2. Login



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{APIURL}}/users/login
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



***Body:***

```js        
{"user":{"email":"{{EMAIL}}", "password":"{{PASSWORD}}"}}
```



### 3. Login and Remember Token



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{APIURL}}/users/login
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



***Body:***

```js        
{"user":{"email":"{{EMAIL}}", "password":"{{PASSWORD}}"}}
```



### 4. Current User



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/user
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 5. Update User



***Endpoint:***

```bash
Method: PUT
Type: RAW
URL: {{APIURL}}/user
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Body:***

```js        
{"user":{"email":"{{EMAIL}}"}}
```



## Profiles



### 1. Register Celeb



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{APIURL}}/users
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



***Body:***

```js        
{"user":{"email":"celeb_{{EMAIL}}", "password":"{{PASSWORD}}", "username":"celeb_{{USERNAME}}"}}
```



### 2. Profile



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/profiles/celeb_{{USERNAME}}
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



### 3. Follow Profile



***Endpoint:***

```bash
Method: POST
Type: RAW
URL: {{APIURL}}/profiles/celeb_{{USERNAME}}/follow
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



***Body:***

```js        
{"user":{"email":"{{EMAIL}}"}}
```



### 4. Unfollow Profile



***Endpoint:***

```bash
Method: DELETE
Type: RAW
URL: {{APIURL}}/profiles/celeb_{{USERNAME}}/follow
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |
| Authorization | Token {{token}} |  |



## Tags



### 1. All Tags



***Endpoint:***

```bash
Method: GET
Type: RAW
URL: {{APIURL}}/tags
```


***Headers:***

| Key | Value | Description |
| --- | ------|-------------|
| Content-Type | application/json |  |
| X-Requested-With | XMLHttpRequest |  |



---
[Back to top](#conduit)
> Made with &#9829; by [thedevsaddam](https://github.com/thedevsaddam) | Generated at: 2019-07-28 21:49:26 by [docgen](https://github.com/thedevsaddam/docgen)
