# Problema 2


En una encuesta, el usuario debe responder si desea
continuar con el proceso. La respuesta puede venir escrita de muchas
formas: "SI", "si", "Sí", "no", etc. Construya un programa que:

a) Solicite una respuesta al usuario.

b) Normalice el texto usando métodos de cadena para eliminar
espacios y unificar mayúsculas/minúsculas.

c) Determine si la respuesta corresponde a una afirmación, una
negación o si es inválida.

d) Muestre el resultado usando una estructura if elif else.

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
