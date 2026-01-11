# Datasets-quimica-2026
Datasets para prácticas de IA en química
## Dataset TR_formulaciones

**Archivo**
- `data/TR_formulaciones/TR_formulaciones.csv`

**Descripción**
Dataset de formulaciones de TR utilizado con fines docentes.
El dataset corresponde a uno de los capítulos del libro (número de capítulo por confirmar).

**Variables**
- `tipo_TR`: tipo de formulación TR
- `fase_elastomerica_pct`: porcentaje de fase elastomérica
- `carga_pct`: porcentaje de carga
- `plastificante_pct`: porcentaje de plastificante
- `T_inyeccion`: temperatura de inyección
- `tiempo_ciclo`: tiempo de ciclo
- `Shore_A`: dureza Shore A
- `Abrasion_DIN`: abrasión DIN

**Uso en Python**
```python
import pandas as pd

df = pd.read_csv("data/TR_formulaciones/TR_formulaciones.csv")
df.head()

---

## Dataset PU_durabilidad

### Archivo

- `data/PU_durabilidad/PU_durabilidad.csv`

### Descripción

Dataset de durabilidad y riesgo de fallo en poliuretanos (PU), utilizado con fines docentes y metodológicos.  
El conjunto de datos se ha generado como dataset sintético guiado, basado en rangos industriales reales y tendencias fisicoquímicas ampliamente documentadas, ante la ausencia de bases de datos públicas sobre fallo y envejecimiento de PU en aplicaciones de calzado.

Este dataset corresponde a uno de los capítulos del libro y se emplea para ilustrar problemas de regresión (pérdida de propiedades) y clasificación (riesgo de fallo).

### Variables

- `tipo_poliol`: tipo de poliol (poliester, polieter, mixto)
- `indice_NCO`: índice NCO del sistema
- `plastificante_pct`: porcentaje de plastificante
- `densidad_g_cm3`: densidad del material
- `humedad_ensayo_pct`: humedad relativa durante el envejecimiento
- `tiempo_envejecimiento_h`: tiempo de envejecimiento

### Variables objetivo

- `perdida_propiedades_pct`: pérdida de propiedades mecánicas (%)
- `fallo`: indicador de fallo del material (SI / NO)

## Dataset de predicción

Además del dataset principal de entrenamiento, se incluye un conjunto de nuevas formulaciones de poliuretano destinado a la evaluación predictiva mediante modelos de IA.

### Archivo
- `PU_nuevas_formulaciones.csv`

### Descripción
Este archivo contiene formulaciones de PU no ensayadas experimentalmente, utilizadas para ilustrar la predicción del riesgo de fallo mediante modelos entrenados (KNIME, ROBERT y Python).

La variable objetivo `fallo` no está incluida, ya que constituye el resultado a predecir.

### Uso
El dataset puede emplearse directamente como entrada de predicción en los flujos de trabajo descritos en el libro.
