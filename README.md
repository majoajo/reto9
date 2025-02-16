# reto9

Punto 1 

```python
def calcular_promedio(n):
     if len(n) > 0:
        return sum(n) / len(n)
     return 0
def main():
    evaluados = input("Ingrese los números separados por espacio: ")
    n = [float(num) for num in evaluados.split()]
    promedio = calcular_promedio(n)
    
    print(f"Promedio de la lista: {promedio}")

main()
```

Punto 2

```python
def producto_punto(vector1, vector2):
    if len(vector1) != len(vector2):
        raise ValueError("Los vectores deben tener la misma longitud")
    return sum(a * b for a, b in zip(vector1, vector2))

# Ejemplo de uso
v1 = [1, 3, 3]
v2 = [4, 5, 6]

resultado = producto_punto(v1, v2)
print("Producto punto: ", resultado)  # Salida: 1*4 + 3*5 + 3*6 = 37

```

punto 3

```python
def mover_ceros_al_final(n):
    n_sin_ceros = [x for x in n if x != 0]
    ceros = [0] * (len(n) - len(n_sin_ceros))
    return n_sin_ceros + ceros

def main():
    entrada_n = input("Ingrese los números separados por espacio: ")
    n = [int(num) for num in entrada_n.split()]
    n_modificados = mover_ceros_al_final(n)
    
    print(f"Lista con ceros al final: {n_modificados}")

    main()

```
