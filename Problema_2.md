- Código

```python

respuesta = input('¿Desea continuar tu proceso? [si/no]: ')

respuesta = respuesta.strip()
respuesta = respuesta.lower()

if respuesta == 'si':
    print('El usuario desea continuar')

elif respuesta == 'sí':
    print('El usuario desea continuar')

elif respuesta == 'no':
    print('El usuario no desea continuar')

else:
    print('Respuesta inválida')

```
