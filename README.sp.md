[ 🌐 عربي ](README.ar.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Deja de explicar la pérdida de inventario. Empieza a localizarla.
# Conciliación de inventario multi-nodo y análisis de merma

[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Browser + Excel](https://img.shields.io/badge/Platform-Browser%20%2B%20Excel-217346.svg)](#quick-start-workflow)
[![Tool Type: Decision Support](https://img.shields.io/badge/Tool%20Type-Decision%20Support-2251FF.svg)](#what-it-helps-you-track)

**Una herramienta ligera de conciliación de inventario y análisis de merma para comparar el inventario de Shopify, WMS y 3PL, localizar discrepancias y traducir la pérdida de existencias en impacto financiero, sin reconstruir el análisis en cada ciclo de reporte.**

**Sin registro. Sin instalación. Gratis en tu navegador.**

Prueba la versión de navegador gratis. Si necesitas la versión de Excel, puedes comprarla con una garantía de devolución del dinero de 30 días, sin hacer preguntas.

>
> 🌐 **[Abrir en el navegador](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)** — versión HTML en vivo
> 📥 **[Descargar Excel](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)** — versión de Excel

## Qué te ayuda a controlar

* **Diferencias de inventario entre Shopify, WMS y 3PL** — ve dónde dejan de coincidir las cantidades reportadas por los sistemas.
* **Varianza total de inventario y valor de merma estimado** — comprende la consecuencia financiera en lugar de revisar solo diferencias de cantidad.
* **Tasas de discrepancia entre 3PL y almacén interno** — distingue dónde se concentra el mayor problema de conciliación.
* **SKU de mayor valor de pérdida** — identifica qué productos merecen investigarse primero.
* **Excepciones de alto riesgo** — resalta los SKU cuyas cantidad o tasa de discrepancia superan el umbral de advertencia configurado.
* **Exposición potencial a reclamaciones 3PL** — proporciona una base fáctica para la corrección de procesos internos o reclamaciones de pérdida contractuales.

## Flujo de trabajo de inicio rápido

1. **Define los parámetros clave.**
   En `Config_Master`, mantén la lista estándar de SKU, la información del producto, el costo unitario y los umbrales de discrepancia o advertencia usados por el negocio.

2. **Importa los datos existentes.**
   Pega la exportación más reciente de Shopify en `Import_Shopify`, la exportación de inventario del WMS en `Import_WMS` y la exportación de inventario físico del 3PL en `Import_3PL`. El flujo de trabajo previsto es usar las exportaciones originales directamente en lugar de reconstruir manualmente una tabla de conciliación normalizada.

3. **Obtén los resultados.**
   Pasa a la salida de conciliación y al `Dashboard`. El libro de Excel limpia y alinea los registros importados, compara las cantidades de inventario entre nodos, calcula las discrepancias y convierte las diferencias relevantes en valores financieros.

4. **Mantén con una actualización periódica.**
   Repite el proceso semanal o mensualmente usando un momento de corte de inventario consistente. El libro es intencionalmente ligero: actualiza los datos de origen en lugar de reconstruir el análisis.

**Define los parámetros de control. Suelta las exportaciones de inventario existentes. Obtén la conciliación. Investiga las excepciones. Actualiza cuando lo necesites.**

## Por qué lo construí

Los problemas de inventario multi-nodo rara vez son causados por la ausencia de un número. Son causados por **diferentes sistemas que presentan diferentes versiones del mismo número**.

Una exportación de inventario de Shopify puede describir lo que el sistema de ventas cree que está disponible. Una exportación del WMS puede describir lo que el almacén interno registra como existente. Un reporte 3PL puede describir el inventario físico en una ubicación de cumplimiento externa. Cuando estos archivos se unen manualmente cada semana, el proceso de conciliación en sí se convierte en otra fuente de error.

El fracaso es especialmente costoso porque una varianza se trata normalmente como un problema de cantidad:

> "El SKU A tiene un faltante de 18 unidades."

Esa afirmación no responde la pregunta de gestión.

La pregunta útil es:

> **¿Dónde desaparecieron esas 18 unidades y qué significa financieramente esa diferencia?**

Esta herramienta convierte la conciliación en un flujo de trabajo analítico repetible. En lugar de comparar manualmente tres hojas de cálculo, el usuario establece una referencia estándar de SKU, importa las tres instantáneas de inventario y deja que el libro alinee los registros y calcule las diferencias.

Por ejemplo, una discrepancia de 20 unidades en un artículo de $3 y una discrepancia de 20 unidades en un artículo de $45 no deberían recibir la misma prioridad de gestión. Introducir la matriz de costos del SKU convierte la varianza de cantidad en una exposición financiera estimada. El dashboard entonces puede ordenar las discrepancias de mayor valor en lugar de forzar al operador a inspeccionar cada fila manualmente.

El resultado es **razonamiento productizado**: un marco reutilizable para responder la misma pregunta operativa cada semana o mes, en lugar de una hoja de cálculo puntual armada en torno a un solo evento de conciliación.

## Problemas comunes de conciliación de inventario que esto resuelve

| Problema                                     | Sin esta herramienta                                                                                              | Con esta herramienta                                                                                              |
| -------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| **Los tres sistemas no coinciden**          | Las exportaciones de Shopify, WMS y 3PL se comparan manualmente, aumentando el riesgo de filas omitidas y coincidencias inconsistentes. | Una capa de conciliación estandarizada alinea los registros en torno a la referencia de SKU configurada.        |
| **Datos exportados desordenados**           | Filas en blanco, formato inconsistente, espacios y mayúsculas crean falsas coincidencias.                        | La capa de cálculo normaliza los campos clave antes de la comparación.                                           |
| **La varianza se mide solo en unidades**    | La gestión ve una diferencia de stock pero no puede estimar de inmediato su significado financiero.              | El costo unitario del SKU convierte las diferencias de cantidad relevantes en valor de pérdida estimado.        |
| **Las excepciones grandes se entierran en el detalle** | Los operadores revisan largas tablas de conciliación y pueden pasar por alto discrepancias comercialmente importantes. | Las salidas del dashboard resaltan tasas de discrepancia, valor de pérdida y los 10 SKU de mayor valor.        |
| **Las pérdidas 3PL son difíciles de sustentar** | Una pérdida sospechada puede quedar como una queja operativa informal.                                          | Un reporte de conciliación estandarizado proporciona una base fáctica para la investigación y posible preparación de reclamo. |
| **La conciliación ocurre demasiado tarde**  | El inventario se revisa de forma reactiva tras acumular discrepancias.                                          | Una cadencia de control semanal o mensual respalda la conciliación proactiva y el seguimiento de excepciones.   |

## Para quién es esto

Esta herramienta está diseñada para **operadores de comercio electrónico y retail, gerentes de cadena de suministro, equipos financieros, controladores de inventario y dueños de negocios** que reciben datos de inventario de múltiples nodos operativos y necesitan una forma repetible de conciliarlos sin introducir un ERP completo o un proyecto de integración personalizada.

Es especialmente adecuada para negocios donde Shopify, un WMS interno y uno o más reportes de inventario 3PL deben compararse de forma recurrente.

**No** está diseñada para reemplazar un ERP, WMS, TMS o integración API en tiempo real. No proporciona seguimiento GPS, previene la sobreventa física en el momento de la transacción, ni resuelve demoras de sincronización de sistemas instantáneas. Esos son problemas de integración de sistemas o control operativo, más que problemas de conciliación en hoja de cálculo.

**No se requiere experiencia en hojas de cálculo para entender la versión de navegador. Ábrela, revisa el flujo de trabajo y determina si el modelo de conciliación se ajusta al proceso operativo.**

## Acerca de

Construyo rastreadores operativos ligeros y herramientas de soporte para la toma de decisiones en situaciones donde hay demasiadas piezas móviles para retener en la cabeza, pero no suficiente complejidad para justificar otro sistema empresarial.

La pregunta central es simple: **¿Qué información necesita estar en un solo lugar para que la próxima decisión operativa se tome con confianza?**

La Conciliación de Inventario Multi-Nodo y el Análisis de Merma es un ejemplo de ese enfoque: convertir la comparación recurrente de inventario entre sistemas en un flujo de trabajo analítico estandarizado que conecta las discrepancias operativas con las consecuencias financieras.

## Detalles técnicos

<details>
<summary>Para revisores técnicos, practicantes de Excel y colaboradores</summary>

### Arquitectura del libro

El libro está estructurado deliberadamente como un **motor de limpieza y conciliación de datos + dashboard de decisiones de pérdida financiera**, en lugar de como una base de datos de inventario permanente. Cada ciclo de conciliación puede sobrescribir el conjunto de importación anterior o guardarse como un libro separado, manteniendo el archivo ligero y evitando dependencias innecesarias de base de datos o macros.

La arquitectura sigue un simple:

**Entrada → Normalizar → Conciliar → Cuantificar → Marcar → Presentar**

```text
                    ┌──────────────────────┐
                    │    Config_Master      │
                    │ SKU / Cost / Rules    │
                    └──────────┬───────────┘
                               │
             ┌─────────────────┼─────────────────┐
             │                 │                 │
             ▼                 ▼                 ▼
     Import_Shopify       Import_WMS       Import_3PL
     System snapshot      WMS snapshot     Physical stock
             │                 │                 │
             └─────────────────┼─────────────────┘
                               ▼
                    ┌──────────────────────┐
                    │     Calc_Engine      │
                    │ Normalize + Match    │
                    │ Variance Calculation  │
                    │ Loss Valuation        │
                    │ Exception Flagging    │
                    └──────────┬───────────┘
                               │
                               ▼
                    ┌──────────────────────┐
                    │      Dashboard       │
                    │ KPI + Loss Analysis  │
                    │ Risk Ranking         │
                    └──────────────────────┘
```

El libro se divide en seis hojas funcionales:

| Hoja            | Capa          | Responsabilidad                                                              | Usuario principal       |
| --------------- | ------------- | ----------------------------------------------------------------------------- | ---------------------- |
| `Dashboard`     | Decision      | Resumen KPI, exposición de pérdida, comparación de nodos, 10 excepciones principales | CEO / Gestión       |
| `Config_Master` | Configuration | Lista estándar de SKU, información del producto, costo unitario, umbrales de discrepancia | Operaciones / Finanzas |
| `Import_Shopify`| Input         | Exportación cruda de inventario de Shopify                                   | Operaciones            |
| `Import_WMS`    | Input         | Exportación cruda de inventario del WMS interno                              | Almacén / Operaciones  |
| `Import_3PL`    | Input         | Exportación cruda de inventario físico 3PL                                  | 3PL / Operaciones      |
| `Calc_Engine`   | Calculation   | Normalización de datos, coincidencia de SKU, cálculos de varianza, impacto financiero | Capa técnica oculta |

Las tres hojas de importación se mantienen intencionalmente como **zonas de pegado**. La especificación de origen permite a los usuarios pegar las exportaciones originales directamente, incluida la compatibilidad con filas en blanco iniciales, en lugar de forzarlos a reformar manualmente los archivos antes de la conciliación.

### Flujo de datos y lógica de conciliación

La capa de cálculo central usa `Config_Master` como punto de referencia para los SKU estandarizados.

```text
Raw Export
   ↓
Trim / Normalize
   ↓
Standard SKU Key
   ↓
Cross-System Lookup
   ↓
Shopify Quantity
WMS Quantity
3PL Quantity
   ↓
Absolute Variance
   ↓
Relative Variance
   ↓
Unit Cost
   ↓
Estimated Financial Loss
   ↓
Warning / Exception Status
   ↓
Dashboard
```

El diseño aborda específicamente el problema de los **datos desordenados**. La arquitectura de origen requiere `TRIM()` para eliminar espacios ocultos o accidentales y `UPPER()` para normalizar las mayúsculas, seguido de `XLOOKUP` o `INDEX + MATCH` para la recuperación no invasiva entre tablas.

Esto importa porque un SKU como:

```text
ABC-001
```

no debería convertirse en una falsa excepción simplemente porque otra exportación contiene:

```text
 abc-001
```

El motor de conciliación por tanto trata la normalización como un requisito previo a la comparación, en lugar de intentar resolver problemas de calidad de datos después de que el reporte de varianza ya se ha generado.

### Principio de corte de conciliación

Las instantáneas de inventario deben representar el **mismo momento de corte del negocio**.

Por ejemplo:

```text
Shopify Snapshot     → Sunday 23:59:59
WMS Snapshot         → Sunday 23:59:59
3PL Physical Count   → Sunday 23:59:59
```

Si las instantáneas se toman en momentos materialmente distintos, los movimientos de inventario, devoluciones o pedidos en tránsito pueden crear diferencias aparentes que no son merma real.

La arquitectura de origen identifica explícitamente el momento de corte consistente como una restricción operativa central y advierte que las instantáneas que no coinciden pueden crear "falsas diferencias".

Esto es por tanto un **requisito de control de negocio**, no meramente un requisito de fórmula de hoja de cálculo.

### El SKU como única clave de conciliación

El SKU se trata como la identidad estándar que conecta los tres sistemas de origen.

La capa de configuración mantiene:

* SKU estándar
* Nombre del producto
* Costo unitario
* Umbral de discrepancia
* Umbral de advertencia

El motor de cálculo entonces usa esa clave estándar para recuperar las cantidades de cada origen.

Esto evita que la conciliación dependa del orden de filas de los archivos importados. Shopify puede listar los SKU en una secuencia, el WMS en otra y el 3PL en una tercera; el motor de cálculo sigue comparando el mismo producto contra el mismo producto.

La especificación de origen enfatiza la unicidad y consistencia del SKU como una restricción fundamental: un producto físico no debería representarse mediante múltiples identificadores inconsistentes.

### Arquitectura del dashboard

El Dashboard está diseñado intencionalmente para la **gestión primero por excepciones**, no para reproducir las tablas de origen crudas.

La capa primaria de KPI contiene:

* Varianza total de cantidad
* Pérdida financiera estimada total
* Tasa de discrepancia 3PL
* Tasa de discrepancia del almacén interno

La capa visual proporciona:

* Distribución del valor de pérdida entre 3PL y almacén interno
* 10 SKU principales ordenados por valor de pérdida
* Identificación de excepciones de alto riesgo

Estas salidas se especifican directamente en la arquitectura de origen.

La secuencia de gestión prevista es:

```text
How much is different?
        ↓
How much money is exposed?
        ↓
Where is the exposure concentrated?
        ↓
Which SKUs matter most?
        ↓
Which exceptions should be investigated?
        ↓
Is a process correction or 3PL claim required?
```

Por eso el libro se entiende mejor como una **capa de soporte para la toma de decisiones** que como una simple hoja de comparación de inventario.

### Tres trampas que atrapan incluso a operadores de inventario experimentados

#### Trampa 1 — Tratar cada diferencia de cantidad como merma

**Decisión:**
Un operador ve que Shopify reporta 1.000 unidades mientras el 3PL reporta 970 e inmediatamente registra 30 unidades como perdidas.

**Número erróneo:**
La comparación usa instantáneas tomadas en momentos distintos.

**Por qué cambia la recomendación:**
La diferencia de 30 unidades puede representar envíos, devoluciones, ajustes u otros movimientos ocurridos entre las dos instantáneas.

**Enfoque correcto:**
Primero establece un momento de corte común y compara instantáneas de inventario equivalentes.

| Enfoque                     | Resultado                                           |
| --------------------------- | --------------------------------------------------- |
| Tiempos de instantánea distintos | Diferencia de 30 unidades tratada como pérdida |
| Corte común                 | Solo se investiga la varianza residual inexplicada  |

La fuente identifica específicamente la inconsistencia de corte como causa de discrepancias falsas.

La decisión corregida es por tanto **"investigar la varianza residual"**, no **"reclamar la varianza completa como merma"**.

<details>
<summary>Lógica de cálculo</summary>

```text
Comparable Variance
= Quantity at Node A
- Quantity at Node B

Only when:
Snapshot_A_Time = Snapshot_B_Time
```

Una discrepancia no debe interpretarse como pérdida financiera hasta que la base de comparación sea válida.

</details>

#### Trampa 2 — Ordenar problemas por unidades en lugar de por dinero

**Decisión:**
El operador ordena el reporte de conciliación por la mayor discrepancia de cantidad.

**Métrica errónea:**
Una varianza de 50 unidades se ordena por encima de una varianza de 10 unidades simplemente porque `50 > 10`.

**Por qué la recomendación es incompleta:**
La cantidad no representa la significancia económica.

Supongamos:

| SKU   | Variance | Unit Cost | Estimated Exposure |
| ----- | -------: | --------: | -----------------: |
| SKU-A |       50 |        $2 |               $100 |
| SKU-B |       10 |       $40 |               $400 |

Un ordenamiento solo por cantidad investigaría primero el SKU-A. Un ordenamiento por pérdida financiera investigaría primero el SKU-B.

La arquitectura de origen exige explícitamente introducir una matriz de costos del SKU para que las diferencias de cantidad se traduzcan en pérdida financiera.

**Decisión correcta:** prioriza las excepciones usando tanto la **varianza de cantidad como la exposición financiera**, en lugar de solo la cantidad.

<details>
<summary>Lógica de cálculo</summary>

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

Para el ejemplo:

```text
SKU-A = 50 × $2  = $100
SKU-B = 10 × $40 = $400
```

La segunda excepción tiene la menor cantidad pero la mayor consecuencia financiera.

</details>

#### Trampa 3 — Asumir que una coincidencia de SKU limpia significa datos limpios

**Decisión:**
El operador usa una búsqueda directa entre las tres exportaciones y asume que los registros sin coincidencia representan inventario faltante.

**Suposición errónea:**
Se presupone que las cadenas de SKU son idénticas entre sistemas.

**Por qué cambia la recomendación:**
Los datos exportados pueden contener espacios iniciales/finales, mayúsculas inconsistentes, caracteres especiales, filas en blanco o convenciones históricas de nombrado de SKU. La fuente identifica específicamente estos como problemas prácticos de calidad de datos.

Por ejemplo:

```text
Shopify → "sku-001"
WMS     → "SKU-001"
3PL     → " SKU-001 "
```

Una coincidencia exacta ingenua puede interpretar estos como productos diferentes.

**Enfoque correcto:** normaliza el identificador antes de la búsqueda entre sistemas.

<details>
<summary>Lógica de normalización</summary>

```excel
=UPPER(TRIM([@SKU]))
```

Luego usa la clave normalizada para la recuperación entre tablas.

Conceptualmente:

```text
Raw SKU
   ↓
TRIM()
   ↓
UPPER()
   ↓
Standardized SKU Key
   ↓
XLOOKUP / INDEX + MATCH
```

Esto reduce las falsas excepciones causadas por el formato en lugar del movimiento de inventario.

</details>

### Escenario de ejemplo

Supongamos que se realiza una conciliación semanal para un solo SKU después de que los tres sistemas se han capturado en el mismo momento de corte.

Las instantáneas importadas reportan:

| Source  | Quantity |
| ------- | -------: |
| Shopify |    1,000 |
| WMS     |      992 |
| 3PL     |      970 |

El costo unitario configurado del SKU es **$18**.

El primer paso analítico no es declarar 30 unidades perdidas. El sistema establece las diferencias entre cada posición de inventario reportada:

```text
Shopify vs. WMS
= 1,000 - 992
= 8 units

WMS vs. 3PL
= 992 - 970
= 22 units
```

Esto proporciona de inmediato una pregunta operativa más útil.

La discrepancia total no es simplemente "30 unidades faltantes". Los datos sugieren que la brecha inexplicada más grande se concentra entre el nodo WMS y 3PL.

Si la varianza 3PL de 22 unidades permanece inexplicada tras verificar el momento de envío, devoluciones, ajustes y otros movimientos legítimos, la exposición financiera estimada al costo configurado es:

```text
22 × $18 = $396
```

La implicación de gestión es por tanto diferente de una advertencia de inventario genérica.

La próxima acción no es inspeccionar cada SKU por igual. El operador debe investigar la **excepción del lado 3PL primero**, verificar si la varianza representa pérdida física, daño, momento o un problema de reporte, y luego determinar si la discrepancia supera la tolerancia contractual o interna de la empresa.

El dashboard está diseñado para hacer visible esta priorización: la gestión puede ver la exposición financiera total, la distribución de la pérdida entre nodos y las excepciones de SKU de mayor valor sin revisar manualmente las exportaciones crudas.

La herramienta por tanto respalda una secuencia de:

**conciliación → aislamiento de excepciones → cuantificación financiera → investigación operativa → posible reclamo o corrección de proceso.**

No determina por sí misma si una discrepancia es legalmente recuperable. Eso sigue siendo una decisión de gestión y contractual.

### Referencia de fórmulas

Las fórmulas a continuación describen los patrones de cálculo centrales especificados para la arquitectura de conciliación. Su objetivo es hacer auditable el razonamiento del libro en lugar de convertir el README en un catálogo genérico de fórmulas de Excel.

<details>
<summary>Normalización de SKU</summary>

**Propósito:** estandarizar las cadenas de SKU importadas antes de la comparación.

```excel
=UPPER(TRIM([@SKU]))
```

**Lógica:**

* `TRIM()` elimina los espacios iniciales, finales y redundantes.
* `UPPER()` estandariza las mayúsculas de las letras.
* La clave normalizada resultante se vuelve adecuada para la coincidencia entre sistemas.

La fuente recomienda específicamente `TRIM()` y `UPPER()` para este propósito.

</details>

<details>
<summary>Búsqueda entre sistemas</summary>

**Propósito:** recuperar la cantidad correspondiente de una tabla de origen tras estandarizar el SKU.

```excel
=XLOOKUP(
    Normalized_SKU,
    Source_SKU_Column,
    Source_Quantity_Column,
    0
)
```

La arquitectura permite `XLOOKUP` o `INDEX + MATCH` como mecanismo de recuperación entre tablas.

El principio de diseño importante no es la función de búsqueda específica. Es que **la identidad del SKU, en lugar de la posición de la fila, controla la conciliación**.

</details>

<details>
<summary>Cálculo de varianza</summary>

**Propósito:** cuantificar la diferencia entre posiciones de inventario comparables.

```text
Absolute Variance
= Source Quantity - Reference Quantity
```

La implementación debe preservar el signo donde la interpretación direccional es útil y usar valores absolutos al ordenar la magnitud de la discrepancia.

```text
Variance Magnitude
= ABS(Source Quantity - Reference Quantity)
```

Esto respalda tanto:

* reconciliación direccional;
* ordenamiento de excepciones.

</details>

<details>
<summary>Conversión de pérdida financiera</summary>

**Propósito:** convertir la varianza de inventario en una exposición financiera estimada.

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

El costo unitario se mantiene en `Config_Master`, permitiendo reutilizar el mismo motor de conciliación cuando cambian los costos de los productos.

La fuente define explícitamente la matriz de costos como el mecanismo para traducir las discrepancias de stock en pérdida financiera.

</details>

<details>
<summary>Varianza relativa y umbral de riesgo</summary>

**Propósito:** distinguir una pequeña diferencia numérica de una excepción operativa material.

Conceptualmente:

```text
Discrepancy Rate
= Absolute Variance ÷ Reference Inventory
```

La tasa resultante puede compararse contra el umbral de advertencia o tolerancia configurado.

El diseño de origen exige que `Config_Master` mantenga los umbrales de discrepancia y que el formato condicional marque las filas cuya cantidad o tasa de discrepancia cruza el límite configurado.

</details>

### Reglas de validación

El motor de conciliación depende de un pequeño número de controles que deben respetarse antes de que la salida pueda tratarse como de grado de decisión.

| Campo / Control                | Regla                                                                                                          | Comportamiento ante error                                                                                              |
| ------------------------------ | ------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| **SKU**                        | Debe estar estandarizado y ser identificable de forma consistente en los archivos de origen.                  | Los registros sin coincidencia o mal formados deben tratarse como excepciones de calidad de datos en lugar de clasificarse silenciosamente como merma. |
| **Unicidad de SKU**            | Un producto físico debe mapear a una identidad de SKU estándar.                                               | Los identificadores duplicados o conflictivos requieren corrección de datos maestros antes de una conciliación confiable. |
| **Costo unitario**             | Debe existir en `Config_Master` para la valoración financiera.                                              | La varianza de cantidad aún puede ser visible, pero la exposición financiera no puede valorarse de forma confiable sin costo. |
| **Corte de instantánea**       | Los datos de Shopify, WMS y 3PL deben representar el mismo punto en el tiempo.                               | Las marcas de tiempo distintas pueden crear varianza falsa y requieren re-exportación o ajuste.                       |
| **Datos de origen importados** | Las exportaciones crudas deben pegarse de forma consistente en sus zonas de importación designadas.          | Las anomalías estructurales o de formato de origen deben corregirse antes de interpretar las excepciones resultantes.  |
| **Umbral de discrepancia**     | Los umbrales de cantidad/tasa deben mantenerse en configuración en lugar de codificarse en las salidas individuales. | Las excepciones que cruzan el umbral se resaltan para investigación.                                              |
| **Tolerancia 3PL / SLA**       | La tolerancia de pérdida contractual debe considerarse al decidir si una excepción es digna de reclamo.       | El libro proporciona evidencia; la gestión determina si debe iniciarse un reclamo contractual.                       |
| **Momento de devoluciones**    | Las devoluciones registradas por un 3PL y los reembolsos registrados en Shopify pueden ocurrir en momentos distintos. | Las discrepancias a corto plazo no deben interpretarse automáticamente como merma permanente.                       |
| **Nombrado histórico de SKU**  | Las inconsistencias de nombrado heredadas deben normalizarse o mapearse.                                     | Los SKU históricos sin mapear deben permanecer visibles como excepciones de calidad de datos.                        |
| **Demora de sincronización de sistemas** | Los problemas temporales de sincronización Shopify/3PL están fuera de la lógica de conciliación de la hoja de cálculo. | Tratar como un problema de integración de sistemas en lugar de forzar una solución VBA en la hoja de cálculo.       |

La fuente distingue explícitamente entre problemas que Excel puede resolver y problemas que requieren intervención operativa o a nivel de sistema. La conciliación estandarizada, la valoración de pérdida y los dashboards de excepciones pertenecen al libro; la disciplina de conteo cíclico, la gestión de reclamos 3PL, la sincronización API y el seguimiento GPS no.

### Qué este libro no intenta resolver

La arquitectura mantiene deliberadamente un límite claro alrededor de la capa de Excel.

**Problemas de gestión operativa:**

* procedimientos de conteo cíclico 3PL inconsistentes;
* frecuencia insuficiente de conteo físico de inventario;
* fallo al iniciar reclamos cuando se exceden los límites de pérdida contractuales.

Estos requieren acción de gestión en lugar de otra fórmula.

**Problemas de integración de sistemas:**

* demoras de sincronización Shopify ↔ 3PL en tiempo real;
* comunicación API;
* integración ERP automatizada.

La fuente recomienda específicamente no forzar estos problemas en un libro de Excel ligero mediante VBA.

**Problemas de visibilidad de transporte:**

* seguimiento GPS en tiempo real del inventario en tránsito;
* flujos de trabajo de gestión de transporte.

Estos requieren un TMS dedicado en lugar de una hoja de conciliación de inventario.

Este límite es intencional. El propósito del libro es proporcionar una **capa repetible de conciliación y análisis de pérdida financiera**, no pretender que todo problema de control de inventario es un problema de Excel.

### Obtener el libro

La herramienta está diseñada para la conciliación recurrente en lugar del análisis de hoja de cálculo de una sola vez.

El ciclo operativo previsto es:

```text
Export Shopify inventory
        ↓
Export WMS inventory
        ↓
Export 3PL physical inventory
        ↓
Paste the three snapshots
        ↓
Refresh the reconciliation
        ↓
Review financial loss + exception ranking
        ↓
Investigate / correct / claim
```

El plano de origen especifica una cadencia semanal o mensual, con los usuarios pegando las tres exportaciones de origen en sus respectivas hojas de entrada y manteniendo los costos de SKU actuales y los umbrales de advertencia en `Config_Master`.

**Versión de navegador:** usa la versión HTML para una revisión operativa rápida.

**Versión de Excel:** usa el libro cuando la conciliación deba actualizarse con exportaciones reales de Shopify, WMS y 3PL.

La herramienta está diseñada intencionalmente para que un usuario de operaciones o finanzas no técnico pueda completar la conciliación recurrente sin reconstruir el modelo analítico cada vez. El objetivo de origen es aproximadamente **10 minutos** para limpiar, conciliar y revisar excepciones.

### Limitaciones

Este libro es una **capa de conciliación y análisis de pérdida**, no una plataforma de control de inventario.

No puede:

* garantizar la sincronización Shopify ↔ WMS ↔ 3PL en tiempo real;
* evitar que un operador de almacén envíe físicamente un artículo cuando el stock es insuficiente;
* reemplazar un WMS, ERP o sistema de gestión de inventario;
* imponer procedimientos de conteo cíclico 3PL;
* determinar automáticamente si una discrepancia es contractualmente recuperable;
* proporcionar seguimiento GPS en tiempo real del inventario en tránsito;
* resolver problemas históricos de datos maestros de SKU sin una decisión de mapeo apropiada.

Estos límites son explícitos en el diseño de origen. La conciliación estandarizada, la valoración de discrepancia, el ordenamiento de excepciones y el reporte en dashboard se consideran problemas de Excel apropiados. La disciplina de conteo cíclico y la gestión de reclamos 3PL requieren controles de gestión; la sincronización API en tiempo real pertenece a la integración de sistemas; el seguimiento de envíos físicos pertenece a un TMS.

También existen importantes restricciones de interpretación.

**Una diferencia de cantidad no es automáticamente merma.** Las devoluciones pueden registrarse por un 3PL en un momento distinto al reembolso correspondiente de Shopify, y el momento de instantánea inconsistente puede crear diferencias temporales. El operador debe validar el contexto del negocio antes de clasificar una discrepancia como pérdida permanente.

**La cifra de pérdida financiera es una estimación, no un asiento contable.** Depende del costo unitario de SKU configurado y de la interpretación de la diferencia de cantidad subyacente.

**Un resultado de hoja de cálculo limpio no garantiza datos de origen limpios.** Las inconsistencias históricas de nombrado de SKU, exportaciones incompletas, registros duplicados o conteos físicos incorrectos aún pueden producir conclusiones engañosas.

El libro debe por tanto usarse como un **mecanismo de investigación de hechos y priorización**, no como un motor de juicio automático.

</details>

## Otras herramientas de esta serie

Una colección de herramientas ligeras de soporte para la toma de decisiones en Excel que cubren control operativo, conciliación, rentabilidad, inventario y análisis financiero.

* **Planificación de inventario y control de reabastecimiento** — demanda, reposición, exposición de inventario y decisiones de compra.
* **Motor de rentabilidad a nivel de pedido** — ingresos, costos variables, asignación de envío y rentabilidad a nivel de pedido.
* **Control de construcción de proyecto único** — presupuesto del proyecto, compromisos, costos de trabajo y rentabilidad del proyecto.
* **Sistema de operaciones y gestión de rentabilidad para contratistas** — flujo Trabajo → Estimación → Trabajo → Mano de obra y materiales → Costo de trabajo → Ganancia → Historial del cliente.

## Licencia

Este proyecto se publica bajo la **Licencia Apache 2.0**.

Puedes usar, modificar, distribuir y adaptar el proyecto sujeto a los términos y condiciones de la Licencia Apache 2.0.

Consulta el archivo de licencia del repositorio para el texto completo de la licencia.