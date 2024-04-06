<html lang="es">
<body>
    <h1>Proyecto de Análisis de Incendios Forestales</h1>
    <p>Este proyecto abarca un proceso completo de limpieza, imputación y visualización de datos utilizando Python junto con herramientas como Pandas, NumPy y Matplotlib.</p>
        <div style="text-align: center;">
    <img src="foto.webp" alt="Incendio Forestal" width="800" height="600">
    </div>
    <h2>Contexto de los Datos</h2>
    <p>Se utilizará el conjunto de datos "Forest Fires", derivado de un estudio entre investigadores asociados a la IEEE. Este dataset incluye información meteorológica y temporal recolectada en incendios forestales en Brasil y Portugal, con el objetivo de encontrar correlaciones entre las variables meteorológicas y el área afectada por los incendios.</p>
    <h2>Introducción</h2>
    <p>Los incendios forestales representan una creciente amenaza debido al cambio climático, afectando gravemente a la biodiversidad. Con recursos limitados para combatir estos desastres simultáneamente, surge la necesidad de un modelo predictivo basado en datos meteorológicos para estimar el área potencial afectada y optimizar la asignación de recursos de respuesta.</p>
    <h2>Problemática abordada</h2>
    <p>Debido al cambio climático y demás factores (medioambientales, auto-provocados, etc), hemos presenciado en nuestra región una creciente ola de incendios forestales; acabando con la vida de gran parte de nuestra fauna, flora y biodiversidad en general. No obstante, en la mayoría de las ocasiones se presenta más de un incendio al tiempo y al tener un personal de apoyo limitado, no se pueden cubrir de manera eficiente estos desastres.

En este sentido, se ha decidio seleccionar un dataset de incendios de forestales, con la intención de generar un modelo que sea capaz de estimar (de acuerdo con ciertas variables meteorológicas), el área potencial a quemarse o perderse debido a dichos fenómenos.</p>
    <h2>Contenido del repositorio</h2>
    <p> Este repositorio está compuesto principamente por 2 Notebooks, que contienen los códigos de limpieza y visualización de los datos (Limpieza_de_datos.ipynb) y el proceso de cargue del dataset a el entorno de MySQL, la elaboración y conversión del archivo en .db, algunas consultas y modificaciones, y la posterior visualización de los datos modificados (Manipulación_de_datos.ipynb).
    Así mismo, se cargan los archivos: 
        <li><strong>forestfires.csv :</strong> Archivo inicial, sin modificaciones.</li>
        <li><strong>data_clean_forest_fires.csv :</strong> Dataset generado después del proceso de procesamiento, limpieza y estandarización.</li>
        <li><strong>forest_fires.db :</strong> Base de datos modificada (final).</li></p>
    <h2>Composición de la Base de Datos</h2>
    <p>El conjunto de datos incluye 517 registros, 12 variables predictoras y una variable objetivo (target) continua, describiendo las condiciones y características de los incendios forestales analizados.</p>
    <h3>Variables</h3>
    <ul>
        <li><strong>X:</strong> Coordenada espacial del eje x (1 a 9).</li>
        <li><strong>Y:</strong> Coordenada espacial del eje y (2 a 9).</li>
        <li><strong>Mes:</strong> Mes del año ('ene' a 'dic').</li>
        <li><strong>Día:</strong> Día de la semana ('mon' a 'sun').</li>
        <li><strong>FFMC:</strong> Índice FFMC del sistema FWI (18,7 a 96,20).</li>
        <li><strong>DMC:</strong> Índice DMC del sistema FWI (1,1 a 291,3).</li>
        <li><strong>DC:</strong> Índice DC del sistema FWI (7,9 a 860,6).</li>
        <li><strong>ISI:</strong> Índice ISI del sistema FWI (0,0 a 56,10).</li>
        <li><strong>Temp:</strong> Temperatura en grados Celsius (2° a 33,3°).</li>
        <li><strong>RH:</strong> Humedad relativa en % (15 a 100%).</li>
        <li><strong>Viento:</strong> Velocidad del viento en km/h (0,4 a 9,4).</li>
        <li><strong>Lluvia:</strong> Precipitación exterior en mm/m^2 (0,0 a 6,4).</li>
        <li><strong>Superficie [Target]:</strong> Superficie quemada del bosque en hectáreas (0.00 a 1090.84).</li>
    </ul>
    <h2>Valor generado</h2>
    <p>Una vez estimando el área potencial a ser quemada, se podría disponibilizar la información a los organismos de socorro, bomberos y/o atención de incendios, como una herramienta que les permita priorizar la atención de estos fenómenos en la región, optimizando el número de personas que componen cada equipo de apoyo acorde al área potencial a ser quemada y así poder atender de mejor manera los indencios forestales.</p>
<h2>Conclusiones</h2>
<p> 
<li> Las condiciones meteorológicas y los índices del sistema FWI varían ampliamente, reflejando la complejidad y la diversidad de las condiciones bajo las cuales ocurren los incendios forestales.
<li> La temperatura es la variable con la correlación más fuerte con la superficie quemada, pero incluso esta correlación es baja. Esto sugiere que ningún factor individual es un predictor fuerte de la superficie quemada.
<li> La humedad relativa es la única variable con una correlación negativa notable con la superficie quemada, aunque sigue siendo baja.
<li> Aunque algunas variables muestran correlaciones con la superficie quemada, estas son bajas, lo que indica que ningún factor por sí solo es un predictor fuerte de la extensión del área quemada. Esto sugiere la importancia de considerar modelos multivariados o técnicas de aprendizaje automático para predecir la superficie quemada de manera más efectiva.</p>
   
<h3>Referencias</h3>
    <ul>
        <li>Cortez, Paulo y Morais, Aníbal. (2008). Forest Fires. UCI Machine Learning Repository. https://doi.org/10.24432/C5D88D.</li>
        <li>Cortez, P. y Aníbal de Jesus Raimundo Morais. “A data mining approach to predict forest fires using meteorological data.” (2007).</li>
        <li>Tables for the Canadian Forest Fire Weather Index System, Canadian Forestry Service, Forest Technical Report, 1984.</li>
    </ul>
</div>
</body>
</html>
