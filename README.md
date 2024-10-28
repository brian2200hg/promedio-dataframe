# promedio-dataframe

# Paso 1: Importar las librerías necesarias: 

import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Paso 2: Crear un DataFrame (o cargar uno existente):

Aquí tienes un ejemplo con una columna de "Edad":
data = {
    'Nombre': ['Alice', 'Bob', 'Charlie', 'David', 'Eva'],
    'Edad': [24, 30, 22, 29, 25]
}

df = pd.DataFrame(data)

# Paso 3: Calcular el promedio de la columna "Edad":

Calculamos el promedio de la columna "Edad":
promedio_edad = df['Edad'].mean()
print(f'El promedio de edad es: {promedio_edad}')
# Paso 4: Visualizarlo usando Seaborn:

Vamos a crear un gráfico de barras que muestre el promedio de edad:
sns.barplot(x=['Promedio de Edad'], y=[promedio_edad])
plt.title('Promedio de Edad')
plt.ylabel('Edad')
plt.ylim(0, 40)  # Ajustar el límite del eje Y si es necesario
plt.show()

# Código Completo

import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Crear un DataFrame
data = {
    'Nombre': ['Alice', 'Bob', 'Charlie', 'David', 'Eva'],
    'Edad': [24, 30, 22, 29, 25]
}

df = pd.DataFrame(data)

# Calcular el promedio de la columna "Edad"
promedio_edad = df['Edad'].mean()
print(f'El promedio de edad es: {promedio_edad}')

# Visualizar el promedio usando Seaborn
sns.barplot(x=['Promedio de Edad'], y=[promedio_edad])
plt.title('Promedio de Edad')
plt.ylabel('Edad')
plt.ylim(0, 40)  # Ajustar el límite del eje Y si es necesario
plt.show()

