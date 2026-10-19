# Proyecto: Análisis de Calidad del Aire en Bogotá

## Pregunta de análisis
¿Cómo varía la concentración de material particulado (PM2.5) por estación y hora en Bogotá, y qué relación tiene con las condiciones climáticas?

## Fuente de datos
Red de Monitoreo de Calidad del Aire de Bogotá (RMCAB). Datos abiertos de la Secretaría de Ambiente. Licencia: Creative Commons.

## Variables previstas
- Estación de monitoreo
- Fecha y hora
- Concentración de PM2.5 (µg/m³)
- Variables meteorológicas (temperatura, humedad, viento)

## Herramientas del curso
Pandas para limpieza y análisis exploratorio. PySpark para el procesamiento de grandes volúmenes de datos si es necesario.

## Cómo reproducir
docker build --tag proyecto:0.1 proyecto/
docker run --rm proyecto:0.1
