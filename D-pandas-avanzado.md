Dataframe
pd_ejemplo=pd.DataFrame(columns=["nota1","nota2","nota3","nota4","nota5"],
                        index=["yeison","steven","tatiana","camilo","samuel"],
                        data=[[5,None,4,5,2], [4,None,3,2,1], [None,None,5,4,3], [4,3,5,2,1], [4,3,5,2,1]])
pd_ejemplo

 


Filtros
.loc[ ] 
filtra por el índice y la columna que se le pasa 
pd_ejemplo.loc["camilo",”nota1”]

 
Filtra por el índice y me muestra todos los datos de la fila 
 
Iloc[ ] 
filtra por el índice numérico
pd_ejemplo.iloc[0]
 
pd_ejemplo.iloc[0:3]

 
pd_ejemplo.loc[["yeison","samuel"],["nota1","nota2"]]

 
.head()
Muestra el numero de datos de manera descendente que le hallamos indicado 
pd_ejemplo.head(2)
 
.tail()
Muestra el numero de datos que le hallamos indicado de abajo hacia arriba  
pd_ejemplo.tail(2)

 

.max()
.min()
pd_ejemplo["nota1"].max()
pd_ejemplo["nota1"].min()

Filtran por los valores máximos o mínimos 
 
Valores nulos

 
Podemos indicar la celda y asignarle un valor 
pd_ejemplo.iloc[2,1]=4
pd_ejemplo

 
.dropna()
Elimina las columnas con valores nulos 
pd_ejemplo.dropna()

 
.fillna()
Rellena los valores nulos con el valor que se le paso 
pd_ejemplo.fillna(4.2)

 
.to_excel(“”)
Nos permite crear un archivo de Excel con el data frame 
pd_ejemplo.to_excel("archivoexport.xlsx")

 
.read_excel(“ ”)
Permite importar archivos de una hoja de calculo 
 
.groupby()
Permite agrupar los datos y le aplica el método asignado


 
.join()
nos permite unir informacion de dos data frame dependiendo los parámetros que se le pasen 
pd_finaljoin=pd_fechas1.join(pd_fechas2.set_index("date"),on="date",how="right")

 
 
.merge()
También nos permite juntar informacion de dos dataframe teniendo encuenta una columna en común
pdfinalmerge=pd.merge(pd_fechas1,pd_fechas2,on="date")
pdfinalmerge

 
