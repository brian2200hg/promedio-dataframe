# promedio-dataframe
este programa calcula la edad de las personas.

# Paso 1: Importar las librerías necesarias: 

import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Paso 2: Crear un DataFrame (o cargar uno existente):

Aquí tienes un ejemplo con una columna de "Edad":
data = {
    'Nombre': ['joa', 'fabri', 'nacho', 'david', 'luca'],
    'Edad': [17, 18, 17, 17, 18]
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
    'Nombre': ['joa', 'fabri', 'nacho', 'David', 'luca'],
    'Edad': [17, 18, 17, 17, 18]
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

Resumen
Este código realiza las siguientes tareas:

Crea un conjunto de datos con nombres y edades.
Calcula el promedio de la edad.
Visualiza el promedio en un gráfico de barras.
Este proceso es útil para entender cómo se distribuyen los datos y cómo interactuar con ellos utilizando herramientas de análisis y visualización en Python.

