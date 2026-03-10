# Problema 1


En un sistema básico de control, un usuario ingresa un código
que supuestamente representa un número binario. Sin embargo, la
entrada puede contener espacios al inicio o al final, letras en
mayúscula o caracteres inválidos. Diseñe un programa que:

a) Solicite al usuario una cadena con un supuesto número
binario.

b) Elimine espacios innecesarios con un método de cadena.
c) Verifique si la cadena está compuesta únicamente por 0 y 1.

d) Si la entrada es válida, convierta el valor binario a
decimal y muestre el resultado.

e) Si no es válida, muestre un mensaje indicando que el código
no corresponde a un binario correcto.


- Código

```python

numero = input('Ingrese el número binario: ')

binario = numero.strip()

numeros_validos = set('0, 1')

valido = set(binario).issubset(numeros_validos) 

if valido:
    decimal = int(binario, 2)
    print('El numero es binario')
    print(f'Resultado en decimal:{decimal}')

else:
    print('Error: El código no corresponde a un binario')

```
```
<img width="335" height="467" alt="image" src="https://github.com/user-attachments/assets/ca81a585-b566-48d6-a217-24f9eaacbbf1" />
```

