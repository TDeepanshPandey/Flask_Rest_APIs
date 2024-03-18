# Flask_Rest_APIs

Udemy Course Learning About Flask and Rest APIs

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
JWT
```
