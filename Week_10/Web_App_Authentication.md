# Web App Authentication
## Cookie-based Authentication
disadvantage, they only work on one domain
## Token-based Authentication (Different to token authentication)
its used to store the users state on the clients machine
token is better for performance as it doesnt have to read from a database
disadvantage: cant terminate a token before the expiry date
    have to create a table that holds the revoked tokens
### Cookie vs Token

|  |  |  |
|:---------: |:----------------------------: |:--------: |
|  |  |  |
|  |  |  |

when u want user profile, to be known putting something in a shopping cart without an account(cookie)
tokens can be used without a web server