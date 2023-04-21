# vardump
Colored Python var_dump for CLI

A small wrapper function to output the colored variable prints to the terminal. The peculiarity of the library is that, like in PHP, the var_dump function is in the global scope. You just need to write import vardump in one startup file and then the var_dump function will be available in all modules that you connect to this script.

## Installation
```
pip install vardump
```

## Enable
```python
# app.py
import vardump
import some_controller

...
var_dump(...)
...
```

## Usage
```python
# some_controller.py

some_obj = {
  'int': 123,
  'str': 'abc',
  'dict': {
    'list': [1,2,3]
  }
}

var_dump(some_obj)
```