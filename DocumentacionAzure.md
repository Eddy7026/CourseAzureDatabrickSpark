# EJEMPLO DE COUMENTACION PRINCIPAL 

## Nuevo Ejemplo

![Grafico de entorno Azure](EntornoAzure1.png)

# MI INTERPRETACION 


```python 
df["energy"] = df["energy"]*2
```


# DOCUMENTACION EN AZURE

## MENU

- # SECCION 3 AZURE DATABRICKS


# SECCION 2 
## Consideraciones sobre la cuenta de Azure

**Subcripciones**: 
al escribir en la parte superior las subcripciones veremos todo lo que hemos gastado y nuestro plan especifico.

# SECCION 3 AZURE DATABRICKS

## 10.Funciones de un Data Engineer 
Data Owner:
Propietarios de datos empresariales, capturan los datos empresariales.

Data Consumers:
optimizan el negocio, generan reportes kpis.
Fraude, Riesgo informes de ventas 

Data Engineer:
Recopilar y transformar los datos, facilitar su consumo los data engineer recibe los requisitos de los Data Owner.

## 11.Introduccion a Azure Databricks 

**Apache Spark:**
es un motor de analisis de datos unificado de alto rendimiento diseñado para el procesamiento masivo de big data y machine learning. Spark proporciona Apis para hacer mas facil su uso.(cuenta con procesamiento de flujo de datos en tiempo real (streaming))

**Arquitectura de Spark:**
contiene spark core
scala  python  java  R RDD

librerias -->

MLlib: desarrollo de algoritmos automaticos.
Graph x: API para trabajar graficos y computacion grafica paralela realizar tareas ETL.

## 12. Crear servicio de Azure Databrick

![Grafico2](DataBrick1.png)
creamos el entorno de trabajo.

![Grafico3](DTB2.png)
seleccionamos la supcripcion por default que es la de 30 dias gratis 200 dolares.

luego tenemos **Resource Group**
es para separar el gasto de recursos de una aplicacion y poder segmentar roles para distintos usarios que puede hacer en cada grupo de recursos puedes contener varios recursos como ( red virtual, maquina virtual, base de datos, storage account), tambien separar ambientes Dev Qa Prod.

![Grafico4](DBT3.png)
**workspace**:
como buena practica colocamos al final ws. ese sera el nombre del espacio de trabajo podriamos tener espacios de trabajo separados como Dev Prod Qa.

**Region:** 
la region es para escojer desde que datacenter estara y dependiendo de el pais que te encuentres entre mas cerca menos latencia tendras.

**Hybric:**
escojemos la opcion hibrida para decirle que trabajaremos en el almacenamiento de nuestra cuenta.

luego en Managed resource Group name databrick lo podria colocar automatico pero le colocamos un nombre. 

![Grafico5](DTB4.png) 

**NETWORKING**:
podriamos seleccion si la red puede ser publica le indicamos que no o si ya contamos con una red virtual que indiquemos cual usaremos el cual es la opcion roja de abajo el cual se nos deplegaria mas opciones.

**ENCRYPTION**:
aqui es para cifrar etc.
nostros podemos colocar nuestras propias claves habilitando use your own key maneged disk.

managed services son acciones irreversibles, son para habilitar contraseñas.

**SECURITY & COMPLIANCE**:
son requisitos normativos de seguridad, existe un monitoreo de seguridad mejorado.

enable automatic cluster update: si se habilita vamos a tener los recursos de seguridad actualizados automaticamente.

**TAGS**: nos ayuda con la facturacion e informacion que queramos brindar.


![Grafico6](DTB5.png) 

le damos a review + create y esperamos.


![Grafico6](DTB7.png)

estas configuraciones se pueden descargar para mantener la ultima version. no se ve en la imagen pero abajo dice download


![Grafico6](DBT8.png)

click on launch workspace.


## 13.Gruia por la interfas de Usuario de Azure DataBricks

![Grafico6](DTB9.png)

Este es el workspace para guardar tus archivos como librerias, .sql etc. tenemos nuestro espacio personal y espacio compartido.


**CATALOG:**
es donde podemos visualizar las bases de datos vistas ETC.


**WORKFLOWS / JOBS & PIPLINES:**
programar jobs tener dependencias de jobs, y flujos de trabajo.


**COMPUTE:**
desde aqui puedes crear los cluster, eliminarlos etc. 

**MARKETPLACE:**
aqui podemos ver proveedores que venden datos.

un click en databricks nos lleva al home de databricks.

## 14.Arquitectura de Azure Databricks 

**CONTROL PLANE**
web aplicacion, compute orsquestacion, unity catalog, querys.

**COMPUTE PLANE**
classic: se administra en mi suscripcion el tema de recourses.

**SERVERLESS**
aca lo hace en el mismo databricks lo que es mas agil.


el WORKSPACE CLOUD STORAGE esta relacionado con el espacio de trabajo si el espacio de trabajo se elimina tambien se eliminara el almacenamiento.


control plan y serverless residen en databricks.