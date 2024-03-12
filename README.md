# Flask_Rest_APIs
 Udemy Course Learning About Flask and Rest APIs

### Python Refresher

#### Unpacking Arguments 
Use *args  to collect the arguments and **kwargs for collection the keyword/dictionary arguments
``` 
def multiply(*args):
    print(args)
multiply(1,3,5)
```
#### Magic Methods
- __init__: initializes the value
- __str__: string representation of the object so it can be printed on the console 
- __repr__: uniambiguous, used in debugger, can be used to recreate object.

#### Classic and Static Method