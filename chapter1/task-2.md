## Task 2

Encoding.

Used encodint to create authentication token. using this hash function to create token which are passed through the network

Using jwt\_payload\_handler

`utilities/users.py`

![](/assets/tokencreate_token.png)

&gt;users/view.py

```py
 user_details = request.data
    user = User(
        email=user_details['email'],
        first_name=user_details['first_name'],
        last_name=user_details['last_name'],
        status=001,
        password=make_password(user_details['password'])
    )
```

Using django auth.hashers make\_password

