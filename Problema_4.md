- Código

```python

dato = input('Ingrese un valor para clasificar: ')

if dato == 'true' or dato == 'false':
    print('El dato es un valor booleano')

elif dato.isdigit():
    print('El dato es un numero entero')

elif dato.replace(".", "", 1).isdigit() and "." in dato:
    print('El dato es un numero decimal')

else:
    print('El dato es una cadena de texto general')
```
