<h1 align='center'>
 <b>PROYECTO INDIVIDUAL Nº2</b>
</h1>

# <h1 align="center">**`Telecomunicaciones`**</h1>
<p align='center'>
<img src = 'Imagen/imagentelco.jpg' height = 200>
<p>

## **Contexto**

En Argentina, el acceso a Internet ha experimentado un gran crecimiento desde la década de 1990. La introducción de la banda ancha y el despliegue de redes móviles han mejorado la velocidad y calidad de conexión. Además, el gobierno ha implementado políticas para fomentar la conectividad en áreas rurales y remotas. Estos avances tecnológicos han tenido un impacto significativo en la economía y en la vida diaria de los argentinos.

Dados los datos de Ente Nacional de Comunicaciones [Enacom](https://datosabiertos.enacom.gob.ar/dashboards/20000/acceso-a-internet/)sobre el acceso a internet que estan publicados en su página web, se hara un analisis acerca de la distribucion, las tecnologias y los ingresos que genera el servicio de internet en el pais, ademas, poder ver el desarrollo actual de los demas servicios de telecomunicaciones que tambien estan en el mercado (TV y telefonia movil).

Se presentara en este proyecto un Eda realizado en Python con la libreria Pandas, el análisis posterior y los Kpis que surgieron. 

Usando las herramientas de un ***Data Analyst*** se confeccionara un análisis completo, simulando la demanda de una empresa, que permita reconocer el comportamiento del sector de telecomunicaciones a nivel nacional, con el fin de orientar a la misma para brindar una buena calidad de sus servicios, identificar oportunidades crecer y poder plantear soluciones personalizadas a sus posibles clientes.

## **Analisis**

`EDA` (Exploratory Data Analysis)

Como se menciono al inicio se usaron los dataset de la pagina de Enacom (ver carpeta Data de este repositorio) en un inicio para generar una primera exploracion y buscar insights que permitieran conlusiones y nuevas busquedas.
Todos los conjuntos de datos tenian como fecha base el año 2014 y finalizaban en el tercer trimestre del 2022.
Verificando en Python el tipo de informacion que brindaban los datasets y poniendo en contexto lo que se estaba revisando, decidi:

- Excluir del analisis los datos de dial up: Los datos de dial up respresentan menos del 1% de la muestra total de tecnologia siendo la banda ancha mas representativa de los accesos actuales a internet.

- Haciendo un analisis previo sobre el desarrollo de la banda ancha en el país y dados los avances tecnológicos traté de hacer foco en los datos de los ultimos tres años.

Luego empece a explorar los datasets y visualizarlos mediante graficas realizadas con las librerias matplotlib y seaborn, tambien en Python. De lo revisado mediante visualizacion y algunas medidas pude empezar a trazar Kpis para poder medir lo que se estaba investigando.
El primero que surgio fue : `Demanda del acceso a internet residencial en Argentina`analizando el dataset de Acceso a Internet por hogar y agregando datos de muestreo del [INDEC](https://www.indec.gob.ar/indec/web/Nivel4-Tema-4-26-153)para cruzar informacion sobre internet móvil. Se analizó el tercer trimmestre de los ultimos dos años (2021-2022) para poder comparar mismos periodos. Lo mas notable es el aumento de la demanda interanual no solo en el acceso a internet fijo sino tambien en internet movil. 

De la mano con esto surge un segundo Kpi: `Cobertura desplegada`, a traves de los datasets accesos por tecnologia y accesos por velocidad y analizando ahora un periodo de tres años, se puede detectar la presencia importante de FTTH en todo el país, cubriendo todo el territorio. Las velocidades desplegadas en la mayoria de las provincias son a partir de los 20 mb , solo el 12,5% muestra accesos a velocidades bajas como  512 , el minimo de la banda ancha.

El tercer y no mas importante indicador es `Comportamiento de compra`. Se analizaron comparativamente los datasets de ingresos tanto de Internet como tv para ver si tienen un comportamiento similar. Los ingresos de ambos se incrementan con los años siendo de la tv, la opcion de suscripcion por sobre la satelital la elegida. Tambien al igual que los accesos al servicio hay un aumento de ingresos en los ultimos trimestres de cada año.


## **Conclusiones**

Todas las tecnologias que tienen que ver con la transmisión de información a través de medios electrónicos aumentan considerablemente año tras año , los argentinos demandan a las empresas proveedoras cada vez mas conexiones y ademas de alta velocidad privilegiando conexiones estables como la Fibra optica. 
El desarrollo y el impulso de nuevas aplicaciones y plataformas de streaming le exigen al usuario tambien que pueda tener conexiones rapida y estables.
Esto se propulsa en un marco donde la cobertura es mayor porque el Estado tiene injerencia:" la Red Federal de Fibra Óptica (REFEFO), que fue diseñada para reducir la brecha digital entre los grandes centros urbanos y las pequeñas y medianas localidades, allí donde, por razones de rentabilidad del mercado, no existen proveedores de servicio de Internet o la cobertura resulta insuficiente" 
[Referencias](#https://www.enacom.gob.ar/institucional/mas-de-200--de-incremento-en-el-acceso-a-internet-de-fibra-optica-en-toda-la-argentina_n4455)
El comportamiento de compra de los consumidores no desprecia una tecnologia sobre la otra ya que aun aumentando los ingresos por internet tambien aumentan los accesos e ingresos por Tv e internet movil, por lo que las telecomunicaciones en general presentan una evolucion positiva generando un mercado fructifero para las grandes y pequeñas empresas.
