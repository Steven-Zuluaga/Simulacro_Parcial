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
