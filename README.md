# latinex_sdk
Python SDK for basic interactions with the Latinex API

# Developed by Rodolfo Blasser 
https://www.linkedin.com/in/rodblasser/

## Usage
This is prototype SDK and it's not currently maintain.

## Example
```python
from latinex_sdk import generic_utils as utils

fecha_inicio = "2023-05-28"
fecha_fin = "2023-06-28"
tipo_emision = "BONOS"
key = '2y2z6i0r-3b2K-6e7m-4a0t-3p3Q0h7u5600'

# Test Connectivity
test = utils.whois()
print(test)

# Welcome
greetings = utils.welcome()
print(greetings)

# Registrar
email = "example@mail.com"
get_key = utils.register(email)
print(get_key)

# Consultar
data = utils.get_historic(key, fecha_inicio, fecha_fin, tipo_emision)
```
