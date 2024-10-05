[![wakatime](https://wakatime.com/badge/user/d9585be0-a800-4e7a-9c42-e2fb31c12a87/project/018e34de-50de-4eb7-b01e-2a7bd930646c.svg)](https://wakatime.com/badge/user/d9585be0-a800-4e7a-9c42-e2fb31c12a87/project/018e34de-50de-4eb7-b01e-2a7bd930646c)

# Flask_Rest_APIs

Udemy Course Learning About Flask and Rest APIs. 

[Course Link](https://www.udemy.com/course/rest-api-flask-and-python/)

### Python Refresher

#### Unpacking Arguments

Use \*args to collect the arguments and \*\*kwargs for collection the keyword/dictionary arguments

```
def multiply(*args):
    print(args)
multiply(1,3,5)
```

#### Magic Methods

- **init**: initializes the value
- **str**: string representation of the object so it can be printed on the console
- **repr**: uniambiguous, used in debugger, can be used to recreate object.

#### Class and Static Method

Can be called without a object Creation but like normal function. @classmethod will be used with parameter while @staticmethod without parameters.

#### Decorators
```
import functools
@functools.wraps() - put in inside the function to access documentation and names
```

### Flask

To run flask, from the same folder containing app.py file
``` 
flask run
```

#### Use abort function to have nicer Not Found
```
abort(404,message = "Store not found.")
```
#### Docker Mount the folder
```
docker run -dp 5005:5000 -w /app -v "$(pwd):/app" flaskapp
```
#### Flask Migrate
```
flask db init
```
#### After Db Changes
```
flask db migrate
```
####  JWT Authorization
```
@jwt_required
```