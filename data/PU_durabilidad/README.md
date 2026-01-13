# PU_durabilidad

Dataset de durabilidad y riesgo de fallo en poliuretanos (PU).
# PU_durabilidad

Dataset de durabilidad y riesgo de fallo en poliuretanos (PU).

## Nota sobre el target binario (ROBERT)

El dataset original `PU_durabilidad.csv` contiene la variable objetivo de durabilidad
en formato categórico (`"SI"` / `"NO"`).

Para poder utilizar este dataset con **ROBERT**, es necesario que la variable objetivo
sea **numérica**. Por este motivo, se ha generado el archivo:

- `PU_durabilidad_binaria.csv`

En este archivo, la variable de durabilidad se ha transformado de la siguiente forma:

- `"NO"` → `0`
- `"SI"` → `1`

Este es el archivo que debe utilizarse para el entrenamiento y predicción de modelos
de clasificación binaria con ROBERT.
