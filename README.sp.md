[ 🌐 عربي ](README.ar.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Multi-Node Inventory Reconciliation & Shrinkage Analysis | Plantilla Excel de Shopify y 3PL
<img width="1920" height="790" alt="image" src="https://github.com/user-attachments/assets/6689bffe-1aac-43d7-9f63-6e85a14470f0" />


[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#licencia)
[![Platform: Browser + Excel](https://img.shields.io/badge/Platform-Browser%20%2B%20Excel-217346.svg)](#tutorial-de-inicio-r%C3%A1pido-c%C3%B3mo-automatizar-tu-conciliaci%C3%B3n-de-inventario)
[![Tool Type: Decision Support](https://img.shields.io/badge/Tool%20Type-Decision%20Support-2251FF.svg)](#qu%C3%A9-te-ayuda-a-seguir-puntos-de-dolor-de-inventario-vs-soluciones)

**Una hoja de cálculo de conciliación de inventario automatizada y plantilla de análisis de mermas (shrinkage) diseñada para marcas de ecommerce multicanal. Compara al instante los niveles de stock de Shopify, los registros del sistema de gestión de almacén (WMS) interno y los recuentos físicos del operador logístico (3PL) para localizar discrepancias y traducir la pérdida de unidades en impacto financiero directo, sin escribir fórmulas VLOOKUP ni reconstruir informes cada mes.**

**Sin registro. Sin instalación. Gratis en tu navegador.**

Prueba tus datos operativos al instante en la versión gratuita del navegador. Para cierres de mes recurrentes y seguridad de datos sin conexión, actualiza a la plantilla de Excel totalmente desbloqueada con una garantía de devolución de 30 días sin preguntas.

> 🌐 **Abrir el dashboard interactivo**  
> [Prueba el simulador gratuito de conciliación de inventario 3PL en el navegador](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
> 
> 📥 **Obtener la hoja de cálculo reutilizable**  
> [Descargar la plantilla Excel de merma de inventario y auditoría](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)

---

## Qué te ayuda a seguir: Puntos de dolor de inventario vs. Soluciones

En lugar de limitarse a identificar que «los números no cuadran», esta herramienta traduce las diferencias brutas de stock en un plan de acción financiero.

| Punto de dolor de inventario ecommerce (El "porqué") | Solución de conciliación (El "cómo") |
| :--- | :--- |
| **Puntos ciegos entre sistemas:** No saber qué sistema (Shopify vs. 3PL vs. WMS) contiene la verdad sobre el stock disponible. | **Triangulación multinodo:** Alinea las cantidades reportadas por los sistemas lado a lado para ubicar con precisión dónde fallan las sincronizaciones de datos. |
| **Merma financiera sin cuantificar:** Tratar una variación de 20 unidades de un artículo de $5 igual que la de uno de $50. | **Análisis de variación ponderado por COGS:** Multiplica las discrepancias de unidades por el coste del SKU para revelar la exposición real al castigo contable. |
| **Fugas del operador logístico (3PL):** Sospechar que los socios de fulfillment pierden stock, pero carecer de pruebas sólidas para reclamaciones SLA. | **Seguimiento de la tasa de discrepancia:** Aísla las tasas de variación del 3PL frente al almacén interno para construir una base fáctica de reclamaciones contractuales por pérdidas. |
| **Parálisis por análisis con datos brutos:** Recorrer miles de filas de hojas de recuento cíclico para encontrar errores. | **Dashboards basados en excepciones:** Clasifica automáticamente los "10 SKU con mayor valor de pérdida" para priorizar las investigaciones de gestión. |

---

## Tutorial de inicio rápido: Cómo automatizar tu conciliación de inventario

Transforma exportaciones desordenadas y multisource en una auditoría de inventario ejecutiva en cuatro pasos estructurados.

### Paso 1: Configura tus datos maestros de SKU (configuración única)
Ve a la hoja `Config_Master`. Define tu nomenclatura estándar de SKU, el coste unitario (COGS) y los umbrales de advertencia específicos del negocio (p. ej., marcar cualquier discrepancia > 5 unidades o > $100 de valor). Esta línea base garantiza que todos los datos entrantes se midan contra una única fuente de verdad.

### Paso 2: Importa las exportaciones de WMS, 3PL y Shopify
Evita la normalización manual de datos. Pega tus exportaciones CSV brutas directamente en sus pestañas designadas:
*   `Import_Shopify` (La disponibilidad de tu tienda)
*   `Import_WMS` (Los registros de tu almacén interno)
*   `Import_3PL` (Los recuentos físicos de tu fulfillment externo)
*Nota: El sistema está diseñado para ingerir exportaciones brutas directamente, sin eliminación manual de columnas ni reconstrucción.*

### Paso 3: Genera el dashboard de merma y revisa las excepciones
Ve al resultado de `Dashboard`. El motor de conciliación automatizado limpia el formato, alinea los SKU y calcula las discrepancias al instante. Revisa tus variaciones de inventario de mayor valor, la merma total y las tasas de exactitud entre nodos sin calcular manualmente una sola celda.

### Paso 4: Establece una rutina y descarga para uso repetido
Para tu primera auditoría, usa la versión del navegador para identificar problemas de stock inmediatos. Para establecer una cadencia robusta de control de inventario mensual, exporta el sistema para uso a largo plazo.

👉 **Acción requerida:** Una vez validado tu flujo de trabajo, **[descarga aquí la plantilla Excel reutilizable de conciliación de inventario](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**. El mes siguiente, simplemente pega la nueva instantánea de inventario sobre los datos antiguos; todo el análisis de variación se actualizará automáticamente.

---

## La lógica de negocio y la metodología

Esta herramienta está diseñada en torno a principios de auditoría profesional, desplazando el foco de la agregación de datos a la protección proactiva de activos. Esta es la metodología operativa que impulsa el libro de trabajo:

### 1. Metodología: Conciliación a tres bandas del inventario
*   **El método:** Al igual que en las auditorías financieras de cuentas por pagar (AP), este marco emplea un **principio de conciliación a tres bandas** entre las ventas digitales (Shopify), el seguimiento interno (WMS) y el almacenamiento físico (3PL).
*   **El impacto de negocio:** Elimina el «juego de culpas». Al triangular los datos, los gerentes de operaciones pueden identificar si un problema es un error de sincronización de la tienda (retraso de API) o una pérdida física de fulfillment (merma), reduciendo drásticamente el tiempo de resolución.

### 2. Metodología: Priorización por valor financiero en riesgo (VaR)
*   **El método:** Las discrepancias se ponderan inherentemente por el costo de los bienes vendidos (COGS). La capa de cálculo transforma la `Variación de unidades` en `Exposición al castigo contable financiero`.
*   **El impacto de negocio:** Optimiza la asignación de mano de obra. En lugar de que el personal del almacén dedique 4 horas a investigar una variación de 50 unidades en sobres de plástico, el dashboard los redirige a investigar una variación de 3 unidades en electrónica de alto margen.

### 3. Metodología: Informes basados en excepciones
*   **El método:** La herramienta filtra miles de SKU coincidentes en una lista condensada de excepciones operativas según umbrales de tolerancia definidos por el usuario (p. ej., merma aceptable < 0.5%).
*   **El impacto de negocio:** Crea **razonamiento productizado**. El director de la cadena de suministro no mira un vertedero de datos; mira una lista de tareas accionable para la corrección de procesos internos o la presentación de reclamaciones al 3PL.

---

## Escenarios del mundo real: Cuándo usar esta plantilla de auditoría de inventario

Este sistema está construido específicamente para puntos críticos de inflexión de la cadena de suministro donde la exactitud del stock físico dicta la salud financiera.

*   **Escenario A: Cierre financiero de fin de mes.** Los equipos de finanzas necesitan una cifra exacta de castigo contable por COGS para contabilidad. Usa esta plantilla para calcular el valor en dólares exacto del inventario perdido en todos los almacenes el último día del mes.
*   **Escenario B: Disputas contractuales de SLA con el 3PL.** Sospechas que tu socio de fulfillment pierde mercancía por encima de la tolerancia de merma del 1.5%. Usa la comparación multinodo para generar un informe de reclamación documentado de los SKU faltantes de alto valor.
*   **Escenario C: Prevención de quiebres de stock en temporada alta (Q4/Black Friday).** Shopify muestra 100 unidades, pero el 3PL solo tiene 20. Ejecuta esta conciliación semanalmente durante el Q4 para detectar el «inventario fantasma» antes de que los clientes compren stock que físicamente no posees, evitando tasas masivas de reembolsos y tickets de soporte.

---

## Problemas comunes de operaciones de inventario que esto resuelve

| Problema de operaciones de inventario | Proceso manual en hoja de cálculo | Solución de plantilla automatizada |
| :--- | :--- | :--- |
| **Tres sistemas dispares en desacuerdo** | Los operadores ejecutan manualmente `INDEX/MATCH` entre los archivos de Shopify, WMS y 3PL, aumentando el riesgo de referencias rotas. | Una capa de conciliación estandarizada alinea automáticamente todas las unidades de mantenimiento de stock (SKU). |
| **Formato de datos exportados desordenado** | Las filas en blanco, los espacios finales y los SKU sensibles a mayúsculas crean errores falsos de discrepancia. | La capa de cálculo normaliza cadenas y tipos de datos antes de la verificación de variaciones. |
| **La merma se mide solo en unidades** | La dirección ve un déficit de unidades pero no puede estimar con precisión el impacto en el COGS. | La matriz de costes de SKU incorporada convierte los déficits de cantidad en castigos contables financieros estimados. |
| **Las excepciones grandes quedan enterradas en el detalle** | Los controladores escanean miles de filas y pasan por alto discrepancias de stock comercialmente fatales. | El dashboard ejecutivo destaca las tasas de error del 3PL, el stock muerto y los 10 artículos de mayor valor de pérdida. |
| **Las pérdidas del 3PL son difíciles de sustanciar** | El inventario faltante sigue siendo una queja informal de almacén sin documentación. | Genera un libro de variaciones fáctico para respaldar reclamaciones formales de SLA al 3PL y reembolsos. |

---

## Para quién es: Roles y casos de uso

Esta herramienta cierra la brecha entre el almacenamiento físico y el informe financiero. Está diseñada específicamente para:

*   **Gerentes de operaciones ecommerce** que necesitan una *plantilla de conciliación de inventario Shopify* para sincronizar las tiendas digitales con los centros de fulfillment físicos.
*   **Directores de cadena de suministro** que buscan una *alternativa de software de auditoría 3PL* para exigir responsabilidades a los socios externos por las tasas de merma contractuales.
*   **Controladores de inventario y gerentes de almacén** que realizan *conciliaciones de recuento cíclico* mensuales entre múltiples nodos internos.
*   **CFOs fraccionados y gerentes financieros** que requieren un método preciso para calcular la *merma de inventario y el impacto en el COGS* para los cierres contables de fin de mes.
*   **Fundadores DTC** que necesitan una visión ejecutiva de la salud del inventario sin invertir en integraciones ERP complejas de seis cifras.

*Nota: Esta herramienta **no** está diseñada para reemplazar APIs en tiempo real, sistemas ERP ni escaneo de códigos de barras WMS en vivo. Es un marco periódico de apoyo a decisiones usado para auditar esos sistemas.*

---

## Acerca del creador

Construyo rastreadores operativos ligeros y herramientas de apoyo a decisiones para situaciones donde hay demasiadas variables en movimiento para sostenerlas en la cabeza, pero insuficiente complejidad como para justificar otro sistema empresarial.

La pregunta central es simple: **¿Qué información debe estar en un lugar centralizado antes de poder tomar con confianza la próxima decisión estratégica de la cadena de suministro?**

Este libro de trabajo de conciliación de inventario multinodo es un ejemplo de ese enfoque: convertir las comparaciones de stock recurrentes entre sistemas en un flujo de trabajo analítico estandarizado que conecta las discrepancias operativas con sus consecuencias financieras.


## Detalles Técnicos

<details>
<summary>Para revisores técnicos, profesionales de Excel y colaboradores</summary>

### Arquitectura del libro de trabajo

El libro de trabajo está deliberadamente estructurado como un **motor de limpieza y conciliación de datos + dashboard de decisión de pérdidas financieras**, y no como una base de datos de inventario permanente. Cada ciclo de conciliación puede sobrescribir el conjunto de importaciones anterior o guardarse como un libro separado, manteniendo el archivo ligero y evitando dependencias innecesarias de bases de datos o macros.

La arquitectura sigue un flujo simple:

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

El libro de trabajo se divide en seis hojas funcionales:

| Hoja             | Capa          | Responsabilidad                                                           | Usuario principal       |
| ---------------- | ------------- | ------------------------------------------------------------------------- | ---------------------- |
| `Dashboard`      | Decisión      | Resumen de KPI, exposición a pérdidas, comparación de nodos, Top 10 de excepciones | Dirección / Gerencia    |
| `Config_Master`  | Configuración | Lista estándar de SKU, información de producto, coste unitario, umbrales de discrepancia | Operaciones / Finanzas  |
| `Import_Shopify` | Entrada       | Exportación bruta de inventario de Shopify                                 | Operaciones             |
| `Import_WMS`     | Entrada       | Exportación bruta de inventario del WMS interno                            | Almacén / Operaciones   |
| `Import_3PL`     | Entrada       | Exportación bruta de inventario físico del 3PL                             | 3PL / Operaciones       |
| `Calc_Engine`    | Cálculo       | Normalización de datos, emparejamiento de SKU, cálculo de variaciones, impacto financiero | Capa técnica oculta     |

Las tres hojas de importación se mantienen intencionalmente como **zonas de pegado**. La especificación fuente permite a los usuarios pegar las exportaciones originales directamente, incluida la compatibilidad con filas en blanco iniciales, en lugar de obligarlos a reestructurar manualmente los archivos antes de la conciliación.

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

El diseño aborda específicamente el problema de los **datos desordenados**. La arquitectura fuente prevé `TRIM()` para eliminar espacios ocultos o accidentales y `UPPER()` para normalizar las mayúsculas, seguido de `XLOOKUP` o `INDEX + MATCH` para una recuperación cruzada no invasiva entre tablas.

Esto importa porque un SKU como:

```text
ABC-001
```

no debería convertirse en una excepción falsa simplemente porque otra exportación contiene:

```text
 abc-001
```

Por tanto, el motor de conciliación trata la normalización como un prerrequisito de la comparación, en lugar de intentar resolver los problemas de calidad de datos después de que ya se haya generado el informe de variaciones.

### Principio del corte temporal de conciliación

Las instantáneas de inventario deben representar el **mismo momento de corte del negocio**.

Por ejemplo:

```text
Shopify Snapshot     → Sunday 23:59:59
WMS Snapshot         → Sunday 23:59:59
3PL Physical Count   → Sunday 23:59:59
```

Si las instantáneas se toman en momentos materialmente diferentes, los movimientos de inventario, las devoluciones o los pedidos en tránsito pueden crear diferencias aparentes que no son merma real.

La arquitectura fuente identifica explícitamente un tiempo de corte consistente como una restricción operativa central y advierte que las instantáneas desalineadas pueden crear «diferencias falsas».

Por tanto, este es un **requisito de control de negocio**, no meramente un requisito de fórmula de hoja de cálculo.

### El SKU como clave única de conciliación

El SKU se trata como la identidad estándar que conecta los tres sistemas fuente.

La capa de configuración mantiene:

* SKU estándar
* Nombre del producto
* Coste unitario
* Umbral de discrepancia
* Umbral de advertencia

El motor de cálculo usa entonces esa clave estándar para recuperar las cantidades de cada fuente.

Esto evita que la conciliación dependa del orden de las filas de los archivos importados. Shopify puede listar los SKU en una secuencia, WMS en otra y 3PL en una tercera; el motor de cálculo sigue comparando el mismo producto contra el mismo producto.

La especificación fuente enfatiza la unicidad y consistencia del SKU como restricción fundamental: un producto físico no debe estar representado por múltiples identificadores inconsistentes.

### Arquitectura del dashboard

El Dashboard está diseñado intencionalmente para una **gestión de excepciones primero**, no para reproducir las tablas fuente brutas.

La capa principal de KPI contiene:

* Variación total de cantidades
* Pérdida financiera total estimada
* Tasa de discrepancia del 3PL
* Tasa de discrepancia del almacén interno

La capa visual proporciona luego:

* Distribución del valor de pérdida entre el 3PL y el almacén interno
* Los 10 SKU principales clasificados por valor de pérdida
* Identificación de excepciones de alto riesgo

Estos resultados están especificados directamente en la arquitectura fuente.

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

Por eso este libro de trabajo se entiende mejor como una **capa de apoyo a decisiones** que como una simple hoja de cálculo de comparación de inventario.

### Tres trampas que atrapan incluso a operadores de inventario con experiencia

#### Trampa 1 — Tratar cada diferencia de cantidad como merma

**Decisión:**
Un operador ve que Shopify reporta 1.000 unidades mientras el 3PL reporta 970 y registra de inmediato 30 unidades como perdidas.

**Número defectuoso:**
La comparación usa instantáneas tomadas en momentos diferentes.

**Por qué cambia la recomendación:**
La diferencia de 30 unidades puede representar envíos, devoluciones, ajustes u otros movimientos ocurridos entre las dos instantáneas.

**Enfoque correcto:**
Primero establecer un tiempo de corte común y comparar instantáneas de inventario homogéneas.

| Enfoque                        | Resultado                                              |
| ------------------------------ | ------------------------------------------------------ |
| Instantáneas en momentos distintos | Diferencia de 30 unidades tratada como pérdida    |
| Corte común                    | Solo se investiga la variación residual no explicada   |

La fuente identifica específicamente la inconsistencia del corte como causa de discrepancias falsas.

La decisión corregida es por tanto **«investigar la variación residual»**, no **«reclamar la variación completa como merma»**.

<details>
<summary>Lógica de cálculo</summary>

```text
Comparable Variance
= Quantity at Node A
- Quantity at Node B

Only when:
Snapshot_A_Time = Snapshot_B_Time
```

Una discrepancia no debe interpretarse como pérdida financiera hasta que la propia base de comparación sea válida.

</details>

#### Trampa 2 — Clasificar problemas por unidades en lugar de por dinero

**Decisión:**
El operador ordena el informe de conciliación por la mayor discrepancia de cantidad.

**Métrica defectuosa:**
Una variación de 50 unidades se clasifica por encima de una de 10 unidades simplemente porque `50 > 10`.

**Por qué la recomendación es incompleta:**
La cantidad no representa la importancia económica.

Supongamos:

| SKU   | Variación | Coste unitario | Exposición estimada |
| ----- | -------: | --------: | -----------------: |
| SKU-A |       50 |        $2 |               $100 |
| SKU-B |       10 |       $40 |               $400 |

Una clasificación solo por cantidad investigaría primero el SKU-A. Una clasificación por pérdida financiera investigaría primero el SKU-B.

La arquitectura fuente pide explícitamente introducir una matriz de costes de SKU para que las diferencias de cantidad puedan traducirse en pérdida financiera.

**Decisión correcta:** priorizar las excepciones usando tanto la **variación de cantidad como la exposición financiera**, no la cantidad sola.

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

La segunda excepción tiene la cantidad menor pero la consecuencia financiera mayor.

</details>

#### Trampa 3 — Asumir que una coincidencia limpia de SKU significa datos limpios

**Decisión:**
El operador usa una búsqueda directa entre las tres exportaciones y asume que los registros no emparejados representan inventario faltante.

**Suposición defectuosa:**
Se presupone que las cadenas de SKU son idénticas entre sistemas.

**Por qué cambia la recomendación:**
Los datos exportados pueden contener espacios iniciales/finales, mayúsculas inconsistentes, caracteres especiales, filas en blanco o convenciones históricas de nomenclatura de SKU. La fuente identifica específicamente estos como problemas prácticos de calidad de datos.

Por ejemplo:

```text
Shopify → "sku-001"
WMS     → "SKU-001"
3PL     → " SKU-001 "
```

Una coincidencia exacta ingenua puede interpretarlos como productos diferentes.

**Enfoque correcto:** normalizar el identificador antes de la búsqueda entre sistemas.

<details>
<summary>Lógica de normalización</summary>

```excel
=UPPER(TRIM([@SKU]))
```

Luego usar la clave normalizada para la recuperación entre tablas.

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

Esto reduce las excepciones falsas causadas por formato en lugar de por movimiento de inventario.

</details>

### Escenario de ejemplo

Asumamos que se realiza una conciliación semanal para un único SKU después de que los tres sistemas hayan sido capturados en el mismo momento de corte.

Las instantáneas importadas reportan:

| Fuente  | Cantidad |
| ------- | -------: |
| Shopify |    1.000 |
| WMS     |      992 |
| 3PL     |      970 |

El coste unitario configurado del SKU es **$18**.

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

La discrepancia total no es simplemente «30 unidades faltantes». Los datos sugieren que la mayor brecha no explicada está concentrada entre el nodo WMS y el 3PL.

Si la variación de 22 unidades del 3PL permanece sin explicar tras revisar el momento de los envíos, las devoluciones, los ajustes y otros movimientos legítimos, la exposición financiera estimada al coste configurado es:

```text
22 × $18 = $396
```

La implicación para la dirección es por tanto diferente de una advertencia genérica de inventario.

La siguiente acción no es inspeccionar cada SKU por igual. El operador debe investigar primero la **excepción del lado del 3PL**, verificar si la variación representa pérdida física, daño, timing o un problema de reporte, y luego determinar si la discrepancia excede la tolerancia contractual o interna de la empresa.

El dashboard está diseñado para hacer visible esta priorización: la dirección puede ver la exposición financiera total, la distribución de la pérdida entre nodos y las excepciones de SKU de mayor valor sin escanear manualmente las exportaciones brutas.

La herramienta por tanto soporta una secuencia de:

**conciliación → aislamiento de excepciones → cuantificación financiera → investigación operativa → potencial reclamación o corrección de proceso.**

Ella misma no determina si una discrepancia es legalmente recuperable. Eso sigue siendo una decisión de gestión y contractual.

### Referencia de fórmulas

Las fórmulas siguientes describen los patrones de cálculo centrales especificados para la arquitectura de conciliación. Su intención es hacer auditable el razonamiento del libro de trabajo, no convertir el README en un catálogo genérico de fórmulas de Excel.

<details>
<summary>Normalización de SKU</summary>

**Propósito:** estandarizar las cadenas de SKU importadas antes de la comparación.

```excel
=UPPER(TRIM([@SKU]))
```

**Lógica:**

* `TRIM()` elimina los espacios iniciales, finales y redundantes.
* `UPPER()` estandariza las mayúsculas de las letras.
* La clave normalizada resultante queda apta para el emparejamiento entre sistemas.

La fuente recomienda específicamente `TRIM()` y `UPPER()` para este propósito.

</details>

<details>
<summary>Búsqueda entre sistemas</summary>

**Propósito:** recuperar la cantidad correspondiente de una tabla fuente después de estandarizar el SKU.

```excel
=XLOOKUP(
    Normalized_SKU,
    Source_SKU_Column,
    Source_Quantity_Column,
    0
)
```

La arquitectura permite `XLOOKUP` o `INDEX + MATCH` como mecanismo de recuperación entre tablas.

El principio de diseño importante no es la función de búsqueda específica. Es que **la identidad del SKU, y no la posición de la fila, controla la conciliación**.

</details>

<details>
<summary>Cálculo de variaciones</summary>

**Propósito:** cuantificar la diferencia entre posiciones de inventario comparables.

```text
Absolute Variance
= Source Quantity - Reference Quantity
```

La implementación debe conservar el signo cuando la interpretación direccional sea útil y usar valores absolutos al clasificar la magnitud de la discrepancia.

```text
Variance Magnitude
= ABS(Source Quantity - Reference Quantity)
```

Esto soporta ambos:

* conciliación direccional;
* clasificación de excepciones.

</details>

<details>
<summary>Conversión a pérdida financiera</summary>

**Propósito:** convertir la variación de inventario en una exposición financiera estimada.

```text
Estimated Loss Value
= Variance Quantity × Unit Cost
```

El coste unitario se mantiene en `Config_Master`, lo que permite reutilizar el mismo motor de conciliación cuando cambian los costes de los productos.

La fuente define explícitamente la matriz de costes como el mecanismo para traducir las discrepancias de stock en pérdida financiera.

</details>

<details>
<summary>Variación relativa y umbral de riesgo</summary>

**Propósito:** distinguir una pequeña diferencia numérica de una excepción operativa material.

Conceptualmente:

```text
Discrepancy Rate
= Absolute Variance ÷ Reference Inventory
```

La tasa resultante puede compararse contra el umbral de advertencia o tolerancia configurado.

El diseño fuente prevé que `Config_Master` mantenga los umbrales de discrepancia y que el formato condicional marque las filas cuya cantidad o tasa de discrepancia cruce el límite configurado.

</details>

### Reglas de validación

El motor de conciliación depende de un pequeño número de controles que deben respetarse antes de que el resultado pueda tratarse como de grado decisional.

| Campo / Control                  | Regla                                                                                                           | Comportamiento ante error                                                                                                            |
| -------------------------------- | -------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| **SKU**                          | Debe estar estandarizado e identificable de forma consistente entre los archivos fuente.                                        | Los registros no emparejados o mal formados deben tratarse como excepciones de calidad de datos, no clasificarse silenciosamente como merma. |
| **Unicidad del SKU**             | Un producto físico debe corresponder a una única identidad de SKU estándar.                                                  | Los identificadores duplicados o conflictivos requieren corrección de datos maestros antes de una conciliación fiable.                       |
| **Coste unitario**               | Debe existir en `Config_Master` para la valoración financiera.                                                         | La variación de cantidad puede seguir siendo visible, pero la exposición financiera no puede valorarse de forma fiable sin coste.                    |
| **Corte de la instantánea**             | Los datos de Shopify, WMS y 3PL deben representar el mismo punto temporal.                                               | Las marcas de tiempo diferentes pueden crear variaciones falsas y requieren reexportación o ajuste.                                       |
| **Datos fuente importados**         | Las exportaciones brutas deben pegarse consistentemente en sus zonas de importación designadas.                                  | Las anomalías estructurales o de formato fuente deben corregirse antes de interpretar las excepciones resultantes.                   |
| **Umbral de discrepancia**        | Los umbrales de cantidad/tasa deben mantenerse en la configuración en lugar de codificarse en salidas individuales. | Las excepciones que crucen el umbral se destacan para investigación.                                                      |
| **Tolerancia / SLA del 3PL**          | La tolerancia contractual a pérdidas debe considerarse al decidir si una excepción es reclamable.              | El libro proporciona la evidencia; la dirección determina si debe iniciarse una reclamación contractual.                    |
| **Timing de devoluciones**               | Las devoluciones registradas por un 3PL y los reembolsos registrados en Shopify pueden ocurrir en momentos diferentes.                        | Las discrepancias a corto plazo no deben interpretarse automáticamente como merma permanente.                                     |
| **Nomenclatura histórica de SKU**        | Las inconsistencias de nomenclatura heredadas deben normalizarse o mapearse.                                                    | Los SKU históricos sin mapear deben permanecer visibles como excepciones de calidad de datos.                                                |
| **Retardo de sincronización del sistema** | Los problemas temporales de sincronización Shopify/3PL están fuera de la lógica de conciliación de la hoja.               | Tratar como un problema de integración de sistemas en lugar de forzar una solución de hoja de cálculo basada en VBA.                               |

La fuente distingue explícitamente entre los problemas que Excel puede resolver y los que requieren intervención operativa o a nivel de sistema. La conciliación estandarizada, la valoración de pérdidas y los dashboards de excepciones pertenecen al interior del libro; la disciplina de recuento cíclico, la gestión de reclamaciones al 3PL, la sincronización de API y el seguimiento GPS no.



### Lo que este libro de trabajo no intenta resolver

La arquitectura mantiene deliberadamente un límite claro alrededor de la capa de Excel.

**Problemas de gestión operativa:**

* procedimientos de recuento cíclico del 3PL inconsistentes;
* frecuencia insuficiente de recuentos físicos de inventario;
* no iniciar reclamaciones cuando se exceden los límites contractuales de pérdida.

Estos requieren acción de gestión, no otra fórmula.

**Problemas de integración de sistemas:**

* retrasos de sincronización en tiempo real Shopify ↔ 3PL;
* comunicación por API;
* integración automatizada con ERP.

La fuente recomienda específicamente no forzar estos problemas dentro de un libro de Excel ligero mediante VBA.

**Problemas de visibilidad de transporte:**

* seguimiento GPS en tiempo real del inventario en tránsito;
* flujos de trabajo de gestión de transporte.

Estos requieren un TMS dedicado, no una hoja de conciliación de inventario.

Este límite es intencional. El propósito del libro de trabajo es proporcionar una **capa repetible de conciliación y análisis de pérdidas financieras**, no pretender que cada problema de control de inventario sea un problema de Excel.

### Obtener el libro de trabajo

La herramienta está diseñada para conciliaciones recurrentes, no para un análisis de hoja de cálculo de una sola vez.

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

El plano fuente especifica una cadencia semanal o mensual, con los usuarios pegando las tres exportaciones fuente en sus respectivas hojas de entrada y manteniendo los costes de SKU y los umbrales de advertencia al día en `Config_Master`.

**Versión navegador:** usa la versión HTML para una revisión operativa rápida.

**Versión Excel:** usa el libro cuando la conciliación deba actualizarse con exportaciones reales de Shopify, WMS y 3PL.

La herramienta está diseñada intencionalmente para que un usuario de operaciones o finanzas no técnico pueda completar la conciliación recurrente sin reconstruir el modelo analítico cada vez. El objetivo fuente es de aproximadamente **10 minutos** para limpiar, conciliar y revisar las excepciones.

### Limitaciones

Este libro de trabajo es una **capa de conciliación y análisis de pérdidas**, no una plataforma de control de inventario.

No puede:

* garantizar la sincronización en tiempo real Shopify ↔ WMS ↔ 3PL;
* impedir que un operador de almacén envíe físicamente un artículo cuando el stock es insuficiente;
* reemplazar un WMS, ERP o sistema de gestión de inventario;
* imponer procedimientos de recuento cíclico al 3PL;
* determinar automáticamente si una discrepancia es contractualmente recuperable;
* proporcionar seguimiento GPS en tiempo real del inventario en tránsito;
* resolver problemas históricos de datos maestros de SKU sin una decisión de mapeo adecuada.

Estos límites son explícitos en el diseño fuente. La conciliación estandarizada, la valoración de discrepancias, la clasificación de excepciones y el reporte de dashboard se consideran problemas apropiados para Excel. La disciplina de recuento cíclico y la gestión de reclamaciones al 3PL requieren controles de gestión; la sincronización de API en tiempo real pertenece a la integración de sistemas; el seguimiento de envíos físicos pertenece a un TMS.

También hay importantes restricciones de interpretación.

**Una diferencia de cantidad no es automáticamente merma.** Las devoluciones pueden registrarse por un 3PL en un momento distinto del reembolso correspondiente en Shopify, y un timing inconsistente de las instantáneas puede crear diferencias temporales. El operador debe validar el contexto de negocio antes de clasificar una discrepancia como pérdida permanente.

**La cifra de pérdida financiera es una estimación, no un asiento contable.** Depende del coste unitario de SKU configurado y de la interpretación de la diferencia de cantidad subyacente.

**Un resultado limpio de la hoja de cálculo no garantiza datos fuente limpios.** Las inconsistencias históricas de nomenclatura de SKU, las exportaciones incompletas, los registros duplicados o los recuentos físicos incorrectos aún pueden producir conclusiones engañosas.

Por tanto, el libro de trabajo debe usarse como un **mecanismo de investigación de hechos y priorización**, no como un motor de juicio automático.

</details>


## Otras herramientas de esta serie

Una colección de herramientas ligeras de apoyo a decisiones en Excel que cubren control operativo, conciliación, rentabilidad, inventario y análisis financiero.

* **Inventory Planning & Reorder Control** — demanda, reposición, exposición de inventario y decisiones de compra.
* **Order-Level Profit Engine** — ingresos, costes variables, asignación de envío y rentabilidad por pedido.
* **Single-Project Construction Control** — presupuesto de proyecto, compromisos, costes de obra y rentabilidad del proyecto.
* **Contractor Operations & Profitability Management System** — flujo de trabajo Lead → Estimación → Obra → Mano de obra y materiales → Coste de obra → Beneficio → Historial del cliente.

## Licencia

Este proyecto se publica bajo la **Licencia Apache 2.0**.

Puede usar, modificar, distribuir y adaptar el proyecto conforme a los términos y condiciones de la Licencia Apache 2.0.

Consulta el archivo de licencia del repositorio para ver el texto completo de la licencia.
