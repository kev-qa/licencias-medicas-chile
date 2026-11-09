# Licencias Médicas en Chile 2020-2024
Análisis de licencias médicas en Chile 2020-2024 (SUSESO)
https://www.kaggle.com/datasets/kevqa6/licencias-mdicas-en-chile-2020-2024-suseso.

Pregunta: ¿cuáles son los principales diagnósticos de las licencias médicas en Chile y cómo cambian por región?

## Archivos
- **Datos_Pais.csv** (260 filas): año, seguro, diagnóstico, medida y valor a nivel nacional.
- **Datos_Region.csv** (4.420 filas): igual, pero por región (16 regiones, con código).

## Columnas
- Año: 2020 a 2024
- Seguro: Fonasa o Isapre (se pueden sumar para obtener el Sistema)
- Region / Codigo: región y número romano (solo Datos_Region)
- Diagnostico: capítulo CIE-10 agrupado por SUSESO (13 categorías)
- Medida: "Licencias emitidas" o "Días otorgados" (no sumar entre sí)
- Valor: cantidad
- Grupo_Diag: 5 diagnósticos principales + "Resto de diagnósticos"

## Fuente
SUSESO, Estadísticas Nacionales de LM y SIL, nueva metodología 2020-2024, hoja C5_LME_DIAG.

## Notas y limitaciones
- Se excluyeron las columnas y filas TOTAL para no duplicar sumas.
- En la fuente, la columna TOTAL de Fonasa 5.1.4.1 (por región) de 2021 y 2024 viene incorrecta; todo se recalculó desde los diagnósticos, que sí coinciden con el total nacional.
- La metodología cambió: verificar comparabilidad con años anteriores.
- Las licencias no reflejan todas las atenciones de salud.
- Las fórmulas y la limpieza se elaboraron con asistencia de Claude (IA de Anthropic); los resultados fueron revisados y validados contra los totales oficiales de SUSESO.

