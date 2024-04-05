<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Proyecto de Análisis de Incendios Forestales</title>
</head>
<body>
    <h1>Proyecto de Análisis de Incendios Forestales</h1>
    <p>Este proyecto abarca un proceso completo de limpieza, imputación y visualización de datos utilizando Python junto con herramientas como Pandas, NumPy y Matplotlib.</p>
    
    <h2>Contexto de los Datos</h2>
    <p>Se utilizará el conjunto de datos "Forest Fires", derivado de un estudio entre investigadores asociados a la IEEE. Este dataset incluye información meteorológica y temporal recolectada en incendios forestales en Brasil y Portugal, con el objetivo de encontrar correlaciones entre las variables meteorológicas y el área afectada por los incendios.</p>
    
    <h2>Introducción</h2>
    <p>Los incendios forestales representan una creciente amenaza debido al cambio climático, afectando gravemente a la biodiversidad. Con recursos limitados para combatir estos desastres simultáneamente, surge la necesidad de un modelo predictivo basado en datos meteorológicos para estimar el área potencial afectada y optimizar la asignación de recursos de respuesta.</p>
    
    <h2>Problemática</h2>
    <p>La frecuencia y simultaneidad de los incendios forestales superan la capacidad de respuesta, lo que subraya la importancia de desarrollar herramientas predictivas para una gestión más eficaz de los recursos disponibles para la lucha contra incendios.</p>
    
    <h2>Valor Generado</h2>
    <p>La estimación del área potencialmente afectada puede ser una herramienta valiosa para los organismos de socorro, permitiendo una mejor planificación y priorización de los esfuerzos de combate a los incendios forestales.</p>
    
    <h3>Referencias</h3>
    <ul>
        <li>Cortez, Paulo y Morais, Aníbal. (2008). Forest Fires. UCI Machine Learning Repository. https://doi.org/10.24432/C5D88D.</li>
        <li>Cortez, P. y Aníbal de Jesus Raimundo Morais. “A data mining approach to predict forest fires using meteorological data.” (2007).</li>
        <li>Tables for the Canadian Forest Fire Weather Index System, Canadian Forestry Service, Forest Technical Report, 1984.</li>
    </ul>
    
    <h2>Composición de la Base de Datos</h2>
    <p>El conjunto de datos incluye 12 variables predictoras y un objetivo (target) continuo, describiendo las condiciones y características de los incendios forestales analizados.</p>
    
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
</body>
</html>
