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

