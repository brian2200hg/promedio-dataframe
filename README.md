# promedio-dataframe

# Abre tu terminal y clona el repositorio:
git clone https://github.com/tu_usuario/promedio-dataframe.git
cd promedio-dataframe

# Crea un archivo Python dentro del directorio del repositorio:
touch calcular_promedio.py

# Abre calcular_promedio.py en tu editor de texto favorito y copia el siguiente código:
import pandas as pd
import seaborn as sns
import matplotlib.pyplot as plt

# Crear un DataFrame
data = {
    'Nombre': ['A', 'B', 'C', 'D', 'E'],
    'Valor': [10, 20, 30, 40, 50]
}

df = pd.DataFrame(data)

# Calcular el promedio de la columna "Valor"
promedio = df['Valor'].mean()
print(f'El promedio es: {promedio}')

# Visualizar el promedio usando Seaborn
sns.barplot(x=['Promedio'], y=[promedio])
plt.title('Promedio de la Columna Valor')
plt.ylabel('Promedio')
plt.show()

