# ciencia01
#Importando a biblioteca pelo google drive
import pandas as pd

df = pd.read_csv("/content/drive/MyDrive/Cusro_Python_Pandas_Digital_Innovation-master/datasets/Gapminder.csv", error_bad_lines=False, sep=";")
#retorna as 5 primeiras linhas
df.head()

#Alterando o nome da tabela para portugues

df = df.rename(columns={"country":"Pais", "continent":"Continente", "year":"Ano", "lifeExp":"Expectativa_vida", "pop":"populacao_total", "gdpPercap":"PIB"})
df.head()

#Total de linhas e colunas

df.shape
#somente colunas
df.columns
#somente o tipo
df.dtypes
#ultimas 5 linhas
df.tail()

#Retorna informações estatisticas sobre o conjunto de dados
#count = total de linhas
#mean = media
#std = desvio padrao
#min = valor minimo
#  quartil
#25% =
#50% =
#75% = 

max = valor maximo
df.describe()


