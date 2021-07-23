# Web App Authentication
## Cookie-based Authentication
disadvantage, they only work on one domain
## Token-based Authentication (Different to token authentication)
its used to store the users state on the clients machine
token is better for performance as it doesnt have to read from a database
disadvantage: cant terminate a token before the expiry date
    have to create a table that holds the revoked tokens
### Cookie vs Token

| Cookie | Session | 
|:---------: |:----------------------------: 
| cookies are client side files that contain user information | sessions are server side which contain user information | 
| cookies ends depending on the lifetime you set for it | a session ends when a user closes his browser | 
| the official max cookie size is kb | the only limit is the maximum memory a script can consume at one time, which 128mb by default | 

| Use Cookie | Use Session | 
|:---------: |:----------------------------: 
| user profile needs personalisation | different domains on the system | 
| track the user | when the API is being used by different platforms such as the web, IoT and mobile devices | 
| logins, shopping carts and game scores, etc | NULL | 
when u want user profile, to be known putting something in a shopping cart without an account(cookie)
tokens can be used without a web server