# Problema 3

Una plataforma académica define que un identificador válido
debe cumplir estas condiciones:

- Debe iniciar con la palabra 'est'.
  
- Debe tener exactamente 8 caracteres.
  
- Los últimos 3 caracteres deben ser dígitos.

- Código

```python

id = input('Ingrese su identificador académico: ')

espacios = id.strip()

largo = len(espacios)

if largo != 8:
    print('Error: longitud incorrecta')

elif espacios[0] != 'e' or espacios[1] != 's' or espacios[2] != 't':
    print('Error: no inicia con est')

elif not (espacios[5].isdigit() and espacios[6].isdigit() and espacios[7].isdigit()):
    print('Error: terminación numérica inválida')

else:
    print('Identificador válido')
```
