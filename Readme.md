
# <h1 align=center> **PROYECTO INDIVIDUAL Nº2** </h1>
# <h1 align=center> **SINIESTROS VIALES CON VÍCTIMAS FATALES EN CABA (2016-2021)** <h1>
# <h1 align=center> DATA FT17 </h1>

<p align="center">
<p align="center">
    <img src= "Imagenes\accidente.jpg"height=300 >
</p>

<hr>

<hr>


<details>
  <summary>Tabla de contenido</summary>
  <ol>  
    <li><a href="#INTRODUCCION">INTRODUCCION</a></li>
    <li><a href="#DATOS">DATOS</a></li>
    <li><a href="#TAREAS-DESARROLLADAS">TAREAS DESARROLLADAS</a></li>
    <li><a href="#ETL">ETL</a></li>
    <li><a href="#EDA">EDA</a></li>
    <li><a href="#  Indicador Clave de Rendimiento  - KPI ">INDICADOR CLAVE DE RENDIMIENTO KPI</a></li>
    <li><a href="#Primer KPI">PRIMER KPI</a></li>
    <li><a href="#Segundo KPI">SEGUNDO KPI</a></li>
    <li><a href="#Tercer KPI">TERCER KPI</a></li>
    <li><a href="#DASHBOARD">DASHBOARD</a></li>
    <li><a href="#Conjunto de Tecnologías">TECNOLOGIAS</a></li>
    <li><a href="#CONCLUSIONES">CONCLUSIONES</a></li>
  </ol>
</details>


</body>
</html></p>

<hr></p>



# INTRODUCCION </p>

<p style="text-align: justify;"> En el marco de este proyecto, desempeñé el papel de Data Analyst para la elaboración de un informe de análisis de datos solicitado por el Observatorio de Movilidad y Seguridad Vial (OMSV), una entidad adscrita a la Secretaría de Transporte del Gobierno de la Ciudad Autónoma de Buenos Aires (CABA).

<p style="text-align: justify;"> El objetivo primordial del proyecto consiste en generar información crucial para que las autoridades locales puedan tomar medidas concretas orientadas a reducir la cantidad de víctimas fatales en los siniestros viales acontecidos en la ciudad. Para llevar a cabo este análisis, se dispuso de un extenso dataset que abarca los años 2016-2021, proporcionado por el gobierno argentino, con información detallada sobre homicidios en siniestros viales.

 <p style="text-align: justify;"> El análisis, llevado a cabo mediante herramientas como Python y librerías como pandas, matplotlib y seaborn, consistió en un proceso integral. Se realizó un ETL para evaluar la limpieza de los datos, seguido de un análisis exploratorio que condujo a conclusiones valiosas. Estas conclusiones fueron luego contrastadas con KPIs relevantes y plasmadas en un dashboard interactivo.

 <p style="text-align: justify;"> Las tasas de mortalidad derivadas de siniestros viales son consideradas indicadores cruciales para evaluar la seguridad vial, y reducirlas es esencial para preservar la vida de los habitantes de Buenos Aires. La ciudad, con una densidad demográfica significativa, presenta desafíos específicos que este análisis pretende abordar.

 <hr></html></p> </p>


  # DATOS </p> 

 <p style="text-align: justify;"> En el desarrollo de este proyecto, se utilizó la Base de Víctimas Fatales en Siniestros Viales, la cual está en formato Excel y consta de dos pestañas de datos:

<b>- HECHOS:</b> Esta pestaña incluye una fila por cada incidente con un identificador único y variables relacionadas con el tiempo, el espacio y los participantes asociados a ese incidente.

<b>-VICTIMAS: </b> En esta pestaña, cada fila representa a una víctima de los incidentes y contiene información sobre la edad, sexo y modo de desplazamiento asociados a cada víctima. Estos datos se conectan a los incidentes a través del identificador único de cada incidente en la pestaña HECHOS.

<hr></p></p> </p> 



# TAREAS DESARROLLADAS <hr></p> 

## ETL 

<p style="text-align: justify;">  Durante la fase de Extracción, Transformación y Carga (ETL), se llevaron a cabo procesos sobre conjuntos cruciales, como HECHOS y VICTIMAS. La selección de datasets base y complementarios abarcó información detallada sobre incidentes y sus víctimas. En el proceso de Transformación y Limpieza, se depuró la información, eliminando elementos superfluos y extrayendo columnas esenciales para el análisis propuesto.

<p style="text-align: justify;"> En el contexto del ETL, se realizó una exhaustiva verificación de datos nulos y duplicados, con la creación de tablas que facilitaron análisis específicos, como la segmentación por semestres. Se llevó a cabo la eliminación de la columna "Altura", considerada no relevante. La fase de transformación y limpieza incorporó pasos cruciales para asegurar la calidad y coherencia de los datos, incluyendo la eliminación de duplicados, el filtrado de fechas inválidas y la gestión de valores nulos.

<p style="text-align: justify;">  Todas estas etapas se ejecutaron de manera local en Visual Studio Code (VSCODE), utilizando Jupyter Notebook como entorno principal y Python respaldado por bibliotecas como numpy y pandas para una manipulación eficiente de los datos. Este enfoque garantizó un flujo de trabajo coherente y organizado, permitiendo que el proyecto se desarrollara de manera eficiente.


<hr></p></p> </p> 

##   EDA

 <p style="text-align: justify;"> Tras la ejecución del proceso ETL y la obtención de los datos resultantes, se llevó a cabo un análisis exploratorio de datos (EDA) que reveló perspectivas fascinantes y patrones subyacentes. Este análisis se extendió a un examen detallado, tanto temporal como geográfico, después del ETL. Se exploraron las variaciones en el número de víctimas a lo largo de los años y se examinaron los siniestros viales en las diferentes comunas de CABA. Este análisis proporcionó reveladores patrones sobre las calles más peligrosas y los factores que influyen en la cantidad de homicidios en accidentes de tráfico. Además, se abordaron aspectos como el tipo de víctima y la relación entre el tipo de vehículo involucrado y los acusados. 


A traves de este analisis se pudieron identificar las victimas por año donde se evidencia que a lo largo de cada año, los hombres representan consistentemente un mayor número de víctimas en comparación con las mujeres. Además, se observa una disminución significativa en el número de víctimas tanto en hombres como en mujeres en 2019. Esta disminución podría estar relacionada con la pandemia por COVID, ya que coincide temporalmente con esas fechas. Por otro lado, se destaca un aumento en el número de víctimas femeninas entre 2016 y 2018. Estos patrones proporcionan insights valiosos sobre las variaciones en la incidencia de accidentes a lo largo del tiempo y sugieren posibles influencias externas, como eventos pandémicos.


<p align="center">
    <img src= "Imagenes\imagen1.jpg" height=400>
</p>

<p style="text-align: justify;"> Es destacable subrayar que, al analizar los datos, se observó que las motocicletas emergen como el tipo de vehículo con la mayor proporción de accidentes, siendo especialmente significativa la predominancia de hombres entre los involucrados en este tipo de incidentes. Esta tendencia sugiere una mayor exposición de los hombres a los riesgos asociados con el uso de motocicletas en comparación con otros grupos demográficos. Asimismo, resulta notable que los peatones constituyen el grupo con la mayor cantidad de víctimas fatales en accidentes, destacando una proporción significativa de hombres en esta categoría, aunque la diferencia en comparación con otros géneros no es tan marcada. Este hallazgo invita a una reflexión sobre los posibles factores que contribuyen a la vulnerabilidad de los peatones, especialmente de aquellos de género masculino, y sugiere la necesidad de medidas específicas para mejorar la seguridad vial de este grupo.


 <p align="center">
    <img src= "Imagenes\imagen2.jpg" height=500>
</p>


<p style="text-align: justify;">El minucioso análisis de los datos resalta que las "Avenidas" sobresalen con un total de 442 víctimas, liderando la estadística, seguidas por las "Calles" con 138 incidentes. Estos resultados evidencian una correlación directa entre el tipo de vía y la seguridad vial, planteando la importancia de considerar este factor al diseñar estrategias de prevención y control de accidentes.

<p style="text-align: justify;">En cuanto a los "Cruces", los incidentes que involucran cruces destacan con un significativo número de víctimas, alcanzando la cifra de 540, en comparación con los casos sin cruces que registran 177 víctimas. Este contraste subraya la urgencia de implementar medidas específicas destinadas a reducir los riesgos asociados a los cruces y, por ende, a minimizar el impacto en términos de víctimas. Estos hallazgos proporcionan una base sólida para la formulación de políticas y acciones focalizadas en áreas específicas que presentan mayores desafíos en términos de seguridad vial.

<p align="center">
    <img src= "Imagenes\imagen3.jpg" height=400>
</p>

<p style="text-align: justify;"> Este exhaustivo análisis proporcionó una visión completa, finalizando con la evaluación comparativa de varios indicadores clave de rendimiento (KPIs). Los descubrimientos obtenidos tienen la intención de servir como orientación para la formulación de estrategias y políticas futuras en materia de seguridad vial en la Ciudad de Buenos Aires. Estos valiosos insights ofrecen una base sólida para la toma de decisiones informadas, permitiendo el diseño de enfoques más efectivos y específicos que aborden de manera precisa los desafíos identificados en el análisis.


<hr></p></p> </p> 


#  Indicador Clave de Rendimiento  - KPI 

<p style="text-align: justify;">  Para este proyecto, se requirieron tres KPIs (Indicadores Clave de Desempeño), de los cuales se recibieron dos, mientras que el tercero se desarrolló con base en la información recopilada durante la ejecución de esta tarea. A continuación, se presentan los KPIs utilizados en el análisis.

# <b> Primer KPI:</b>  

Reducir 10% la tasa de homicidios en siniestros viales de los últimos seis meses, en CABA, en comparación con la tasa de homicidios en siniestros viales del semestre anterior

<p align="center">
    <img src= "Imagenes\imagen4.jpg" height=300>
</p>

<p style="text-align: justify;">  A lo largo de los años, se han observado fluctuaciones en la tasa de homicidios en siniestros viales, destacando disminuciones en ciertos periodos. En el año 2017 y 2018, tanto en el primer como en el segundo semestre, se experimentaron reducciones, aunque ninguna alcanzó el objetivo del KPI de reducir la tasa en un 10%. En contraste, el año 2019 destacó por presentar disminuciones significativas de más del 20% en ambos periodos, superando ampliamente el objetivo establecido. El primer semestre de 2020 cumplió con el KPI, pero el segundo semestre presenció un aumento del 80.65%, incumpliendo el objetivo. En el año 2021, mientras el primer semestre mostró una reducción del 3.23%, el segundo semestre logró una disminución del 23.64%, cumpliendo finalmente con el KPI. En resumen, aunque algunos periodos exhibieron mejoras en la seguridad vial, solo en los años 2019 y 2021 se lograron reducciones consistentes de más del 10%, cumpliendo así con el objetivo establecido por el KPI.


# <b> Segundo KPI:</b>  

Reducir en un 7% la cantidad de accidentes mortales de motociclistas en el último año, en CABA, respecto al año anterior.

<p align="center">
    <img src= "Imagenes\imagen5.jpg" height=300>
    
</p>

<p style="text-align: justify;">  En el análisis, en 2016 y 2017, la evolución porcentual superó el objetivo del 7%, logrando un cumplimiento positivo del KPI. En 2018 y 2019, las reducciones fueron del 1.61% y 18.03%, mostrando resultados mixtos. En 2020, hubo una drástica disminución del 40.00%, cumpliendo con el KPI. Sin embargo, en 2021, se evidenció una evolución negativa del -53.33%, indicando un incumplimiento del KPI debido a un aumento significativo en accidentes mortales. Analizar las tendencias a lo largo de los años es esencial para comprender las variaciones en la evolución porcentual. La excepcional reducción en 2020 podría estar relacionada con la pandemia de COVID-19 y las restricciones, llevando a una disminución general en la movilidad. El aumento abrupto en 2021 subraya la importancia de monitorear continuamente las condiciones del tráfico y ajustar estrategias de seguridad vial según sea necesario. En resumen, aunque se logró una significativa reducción en 2020, la evolución negativa en 2021 destaca la necesidad de un enfoque proactivo en las medidas de seguridad vial ante los desafíos cambiantes en la movilidad.

# <b> Tercer KPI:</b>  

Reducir en un 5% la cantidad de accidentes mortales ocurridos en las avenidas en el último año, en CABA, respecto al año anterior.

<p align="center">
    <img src= "Imagenes\imagen6.jpg" height=300>  
</p>

<p style="text-align: justify;">  Los resultados indican que en 2016 y 2017 no hubo cambios significativos en la cantidad de víctimas en las avenidas. En 2018, se logró una reducción del -8.60%, superando la meta del KPI. Sin embargo, en 2019 se observó un aumento del 34.65%, incumpliendo la meta establecida. En 2020, se alcanzó una disminución del 15.15%, cumpliendo con la meta del KPI. En 2021, se registró una reducción del -8.93%, nuevamente superando la meta del KPI. En resumen, aunque se lograron reducciones significativas en 2020 y 2021, es esencial analizar las razones detrás del aumento en 2019 para ajustar estrategias y mantener mejoras continuas en la seguridad vial en las avenidas de CABA.



<hr></p></p> </p> 


# Dashboard 

<p style="text-align: justify;"> Se ha desarrollado un panel de control en Power BI con el propósito de resumir visualmente la información recopilada y facilitar la comprensión de los conocimientos adquiridos durante este proyecto. Este panel cuenta con elementos visuales interactivos que permiten observar cambios al hacer clic en cada uno de ellos.

<p style="text-align: justify;"> El diseño meticuloso y profesional de este panel en Power BI tiene como objetivo presentar de manera accesible y visual los resultados obtenidos en el análisis de datos realizado en este proyecto. Destinado específicamente a la persona que nos encargó este trabajo, este recurso se presenta como una herramienta esencial para comunicar eficazmente los descubrimientos derivados de la exhaustiva exploración de datos.

<p style="text-align: justify;"> Los elementos visuales interactivos incorporados en el panel brindan la posibilidad de explorar detalladamente la información con un solo clic, ofreciendo una experiencia dinámica que facilita la comprensión de los resultados. Esta herramienta no solo resume de manera efectiva los hallazgos, sino que también proporciona un medio poderoso para la toma de decisiones informadas en el ámbito de la seguridad vial en la Ciudad de Buenos Aires.


<p align="center">
    <img src= "Imagenes\imagen7.jpg" height=600>  
</p>

<hr></p></p> </p> 

# Conjunto de Tecnologías

![Visual Studio Code](https://img.shields.io/badge/Visual%20Studio%20Code-0078d7.svg?style=for-the-badge&logo=visual-studio-code&logoColor=white)
![Jupyter Notebook](https://img.shields.io/badge/jupyter-%23FA0F00.svg?style=for-the-badge&logo=jupyter&logoColor=white)
![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![NumPy](https://img.shields.io/badge/numpy-%23013243.svg?style=for-the-badge&logo=numpy&logoColor=white)
![Pandas](https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Seaborn](https://img.shields.io/badge/Seaborn-3795D6?style=for-the-badge&logo=seaborn&logoColor=white)
![PowerBI]( https://img.shields.io/badge/PowerBI-F2C811?style=for-the-badge&logo=Power%20BI&logoColor=white)
![GitHub](https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white)
![Markdown](https://img.shields.io/badge/markdown-%23000000.svg?style=for-the-badge&logo=markdown&logoColor=white)




<hr></p></p> </p> 


# Conclusiones

<p style="text-align: justify;"> En síntesis, los datos revelan inquietudes significativas acerca de la seguridad vial, resaltando varios aspectos clave. En términos de participantes y roles, los conductores ocupan una posición predominante, subrayando la necesidad de abordar la seguridad de este grupo en particular. La vulnerabilidad de los accidentes en motocicletas resalta la importancia de adoptar medidas específicas para salvaguardar a este colectivo. Asimismo, los pasajeros y los peatones experimentan un número considerable de incidentes, subrayando la necesidad de considerar la seguridad de todos los participantes en el tráfico.

<p style="text-align: justify;"> Los conductores de motocicletas son la categoría más frecuentemente afectada, indicando su vulnerabilidad inherente. Ciclistas y peatones también muestran cifras significativas, evidenciando la necesidad de enfoques específicos para mejorar su seguridad. Los accidentes que involucran a pasajeros de automóviles y motocicletas también son notables, resaltando la importancia de medidas específicas en estas circunstancias.

<p style="text-align: justify;"> Se observa una marcada disparidad de género, con un 77% de víctimas masculinas en comparación con un 23% de víctimas femeninas. Esta discrepancia es especialmente evidente entre los conductores, donde la mayoría son hombres. En cuanto a las edades, la mayoría de los involucrados en accidentes tienen menos de 55 años, con una concentración particular entre los 20 y 40 años. La disminución en el número de víctimas en 2019 podría estar relacionada con la pandemia de COVID-19.

<p style="text-align: justify;"> La variabilidad temporal muestra fluctuaciones por semestre, con notables disminuciones en 2019 y 2020, posiblemente asociadas con la pandemia. Diciembre destaca como el mes con la mayor cantidad de accidentes fatales, proporcionando perspicacia sobre la variabilidad estacional. En cuanto a la distribución espacial, las avenidas lideran en número de víctimas. Los incidentes en cruces registran un mayor número de víctimas que aquellos sin cruces, destacando la importancia de medidas específicas en estas intersecciones. Comunas específicas, como la Comuna 1, presentan cifras más elevadas, sugiriendo la necesidad de evaluaciones y políticas de seguridad vial más focalizadas en esas áreas. En conjunto, estos datos constituyen un punto de partida valioso para análisis detallados y la implementación de medidas específicas destinadas a mejorar la seguridad vial, identificando áreas críticas y grupos vulnerables que requieren atención prioritaria.
