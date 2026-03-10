# Problema 5

En una red digital sencilla, una trama de 8 bits debe ser
analizada antes de procesarse.
Reglas:

- Si no tiene exactamente 8 caracteres, la trama es inválida.
- Si contiene caracteres distintos de 0 y 1, la trama es inválida.
- Si tiene más de 5 bits en 1 → Trama de alta activación.
- Si tiene entre 3 y 5 bits en 1 → Trama de activación media.
- Si tiene entre 0 y 2 bits en 1 → Trama de baja activación.
  
Diseñe un programa que:

a. Solicite al usuario la trama.
b. Limpie la entrada.
c. Valide longitud y contenido.
d. Cuente cuántos 1 tiene usando un método de cadena.

- Código

```python

entrada = input('Ingrese la trama de 8 bits: ')

trama = entrada.strip()

largo = len(trama)
binario = set(trama).issubset({'0', '1'})

if largo != 8:
    print('Trama invalida: no tiene 8 caracteres')

elif not binario:
    print('Trama invalida: tiene caracteres no binarios')

else:
    unos = trama.count('1')
    
    if unos > 5:
        print('Trama de alta activación')
    
    elif unos >= 3: 
        print('Trama de activación media')
    
    else: 
        print('Trama de baja activación')

    print(f'La trama tiene: {unos} unos')

```
