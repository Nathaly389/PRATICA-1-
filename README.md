# PRATICA-1-
def buscar_valor(matriz, valor):
    for i in range(len(matriz)):
        for j in range(len(matriz[i])):
            if matriz[i][j] == valor:
                return f"Valor {valor} encontrado en la posición ({i}, {j})"
    return f"Valor {valor} no encontrado en la matriz"

# Definir la matriz 3x3
matriz = [
    [5, 8, 3],
    [9, 1, 6],
    [2, 4, 7] 
]

# Mostrar la matriz
print("Matriz:")
for fila in matriz:
    print(fila)

# Valor a buscar (entrada del usuario)
try:
    valor_a_buscar = int(input("Ingresa el valor a buscar: "))
    print(buscar_valor(matriz, valor_a_buscar))
except ValueError:
    print("Error: Ingresa un número válido.")
