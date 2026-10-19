# Informe del taller · Unidad 6 · Grupo 12

## 1. Repositorio e integrantes
Enlace al repositorio: https://github.com/fahmitoledo-star/taller-u6-grupo-12
- Integrantes: [Samuel y Miguel] (@fahmitoledo-star)(@Miguegon2003) - Roles R1, R2 y R3 (Grupo unipersonal).

## 2. Reproducción de la versión 1.0 (M2)
Resultado de la ejecución: "Reproducción exacta: 3 de 3 salidas coinciden."
Huellas obtenidas:
- 154b62824a5a7f02e37a5e7a0a93e46ddd0237f2d88a57a8048800650b15a59a  resumen_ciudad.parquet
- 0c598115bb5676dd920eb4ada9a1be22dc6509f79aad616d795a65e337fbb4b  resumen_ciudad.csv
- 568842db5a3964bdf2714a947311d127a9e35722593c2f12cba9b2ced58e74b2  tarifa_media_ciudad.png

## 3. Trabajo en paralelo (M3)
Salida de `git log --oneline --graph`:
* bf2e386 Documenta integrantes; prepara imagen 1.1 (R1)
* aa74104 Agrega desviación estándar de la tarifa (R3)
* 3fb3dd5 Agrega Pereira al generador de datos (R2)

No hubo push rechazado, ya que los cambios se hicieron de forma secuencial.

## 4. Versión 1.1 (M4)
Se construyó la imagen 1.1 y se verificó que las huellas coinciden con las de referencia. La tabla de 6 ciudades muestra a Pereira. La huella de resumen_ciudad.csv es 8160729e...
Se publicó la etiqueta v1.1.

## 5. Diagnósticos (M5)
- **Prueba de semilla:** Cambiar la semilla altera todos los números aleatorios, por lo que los datos generados cambian, y por tanto las huellas son diferentes (0 de 3).
- **Prueba de versión sin fijar:** Al quitar `==2.1.3` y dejar `>=2.1`, el resultado puede ser 3 de 3 (si la versión descargada es compatible) o fallar. Esto demuestra que sin versiones fijas no hay garantía de reproducibilidad en el tiempo.
- **Prueba de .gitignore:** El archivo .gitignore evita que los datos generados y las salidas se suban a GitHub, manteniendo el repositorio ligero y permitiendo que cualquiera regenere los resultados con el código.

## 6. Semilla del proyecto (M6)
Se creó la carpeta `proyecto/` con README.md, requirements.txt (versiones fijas) y Dockerfile. El comando `docker run --rm proyecto:0.1` imprime "Entorno listo, pandas 2.2.3".
