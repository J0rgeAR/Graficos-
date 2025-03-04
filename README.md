# Graficos-
Graficos en python 
import matplotlib.pyplot as plt

# Datos de ejemplo
categorias = ['Smart', 'Celulares', 'Tablet', 'Consolas', 'Notebook']
valores = [10, 20, 15, 30, 25]

# Colores personalizados para cada barra
colores = ['red', 'blue', 'green', 'orange', 'purple']

# Crear el gráfico de barras con colores personalizados
plt.bar(categorias, valores, color=colores)

# Añadir título y etiquetas
plt.title("Gráfico de Barras con Colores Personalizados")
plt.xlabel("Categorías")
plt.ylabel("Valores")

# Añadir valores sobre las barras
for i, valor in enumerate(valores):
    plt.text(i, valor + 0.5, str(valor), ha='center', va='bottom', fontweight='bold')

# Mostrar el gráfico
plt.show()
