
PCNubbies POSTMAN API TESTING NOTES (GROUP I-Tech)     ||
=========================================================

Table for Authorization
For gender answers: (0-1)
[0 = male,
1 = female]

For age range answers: (answer only from 1-5)
[1 = 18-24,
2 = 25-34,
3 = 35-45,
4 = 46-59,
5 = 60+]


For Authorization End Point
----------------------------------------------------------------------------------------------------
Register (POST):
http://127.0.0.1:8000/api/register

Params: (below are the needed fields to register)

(name,
email, 
gender,
age_range,
password)


Login (POST):
http://127.0.0.1:8000/api/login

Params:

email,
password

(Get the access token, go to authorization, choose bearer token, put the token on the right side)

User Profile (GET):
http://127.0.0.1:8000/api/user
(You need to still have the bearer token in the authorization)

Logout (POST):
http://127.0.0.1:8000/api/logout
(You need to still have the bearer token in the authorization)


For Shop End Point
----------------------------------------------------------------------------------------------------
Check all products (GET)
http://127.0.0.1:8000/api/products

Product Filter (GET)
Not yet finalized)


For Add to Cart End Point
----------------------------------------------------------------------------------------------------
Add to Cart a certain product (POST)
http://127.0.0.1:8000/api/cart/{product_id}

Params:
(quantity)

