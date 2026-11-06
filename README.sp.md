[ 🌐 عربي ](README.ar.md) | [ 🇩🇪 Deutsch ](README.de.md) | [ 🇫🇷 Français ](README.fr.md) | [ 🇳🇱 Nederlands ](README.nl.md) | [ 🇪🇸 Español ](README.sp.md) | [ 🇬🇧 English ](README.md)

# Plantilla Excel de conciliación de inventarios Shopify y 3PL: discrepancias de stock en almacén, variación de recuento cíclico y calculadora de costes de merma
<img width="1102" height="790" alt="image" src="https://github.com/user-attachments/assets/3a637973-b460-4160-a098-eed931e2dc18" />



[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](#license)
[![Platform: Web Browser + Microsoft Excel (.xlsx)](https://img.shields.io/badge/Platform-Web%20Browser%20%2B%20Microsoft%20Excel%20(.xlsx)-217346.svg)](#quick-start-tutorial-how-to-reconcile-shopify-wms--3pl-inventory-in-4-steps)
[![Tool Type: Plug-and-Play Ecommerce Inventory Spreadsheet](https://img.shields.io/badge/Tool%20Type-Plug--and--Play%20Inventory%20Spreadsheet-2251FF.svg)](#what-it-helps-you-track-ecommerce-inventory-pain-points-vs-solutions)

**Una plantilla Excel (`.xlsx`) de conciliación de inventarios Shopify y 3PL lista para usar y una calculadora online gratuita de discrepancias de stock, diseñadas para marcas de ecommerce, operadores DTC y gestores de almacén que necesitan auditar los recuentos de inventario sin escribir fórmulas.** Compara **las cantidades del escaparate de Shopify**, los **registros internos del sistema de gestión de almacén (WMS)** y **los recuentos físicos cíclicos del operador logístico (3PL)** lado a lado, calcula la **merma de inventario ponderada por COGS ($)**, detén la **sobreventa por inventario fantasma** y genera **reclamaciones de reembolso al 3PL documentadas** en una sola hoja de cálculo preconfigurada.

**Prueba tus datos de SKU gratis en tu navegador ahora mismo, o descarga el archivo Excel desbloqueado para auditorías mensuales.**

Cada regla de emparejamiento de SKU, fórmula de limpieza de texto y cálculo de diferencias en dólares ya está incorporado. Copia y pega tus exportaciones CSV en bruto desde Shopify, tu WMS y tu 3PL para ver tus discrepancias de stock exactas y tu exposición a pérdidas financieras en segundos — con una garantía de devolución de 30 días sin preguntas.

> 🌐 **Prueba primero la calculadora de conciliación online**  
> [Lanza la calculadora web interactiva gratuita de conciliación de inventarios Shopify y 3PL (demo en navegador, sin configuración previa)](https://hyvoid.github.io/multi-node-inventory-reconciliation/)
> 
> 📥 **Descarga la plantilla Excel lista para usar**  
> [Obtén la plantilla Excel desbloqueada de conciliación multinodo de inventarios y auditoría de mermas (.xlsx con fórmulas de actualización automática)](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)
>
> *Tanto la calculadora gratuita del navegador como el libro de trabajo de Microsoft Excel descargable funcionan sobre exactamente las mismas tablas preconfiguradas de emparejamiento de SKU a tres bandas y de variaciones de COGS.*

---

## Qué te ayuda a seguir: puntos de dolor de inventario en ecommerce vs. soluciones

Descubrir que tus cifras de stock no cuadran es solo la mitad del problema — también necesitas saber dónde fueron a parar las unidades y cuánto dinero está en juego. Esta **hoja de cálculo de auditoría de inventario plug-and-play** resuelve los cinco puntos ciegos más comunes del control de inventario para marcas de ecommerce multicanal:

| Tema de búsqueda frecuente y objetivo de seguimiento | El punto de dolor diario de inventario en ecommerce (donde se filtra el dinero) | Cómo esta plantilla Excel preconfigurada lo corrige y lo sigue |
| :--- | :--- | :--- |
| **Discrepancias de stock Shopify vs. 3PL vs. WMS (`emparejamiento de inventario a 3 bandas`)** | Shopify dice que tienes 120 unidades, tu WMS dice 100 y tu 3PL dice 85 — sin que sepas qué sistema contiene el recuento real de stock. | Alinea **las cantidades de Shopify, WMS y 3PL lado a lado** por SKU para que puedas separar los retrasos de sincronización de TI de las pérdidas físicas reales del almacén. |
| **Coste de merma de inventario y castigo contable por COGS (`impacto en $` vs. recuento de unidades)** | Tratar un faltante de 20 unidades en un inserto de embalaje de $2 con la misma urgencia que una pérdida de 20 unidades en un producto estrella de $75. | Multiplica las variaciones de unidades por el **coste unitario (COGS)** de cada SKU para calcular la **exposición exacta de merma en dólares ($)** destinada a castigos contables. |
| **Stock perdido del 3PL y reclamaciones de reembolso SLA (auditoría de la `tolerancia de merma`)** | Sabes que tu centro de fulfillment pierde mercancía, pero careces de la prueba de variaciones a nivel de SKU necesaria para presentar una reclamación contractual. | Sigue las **tasas de discrepancia (%) entre el 3PL y el almacén interno** frente a tu límite contractual de merma para construir un registro de reembolsos basado en hechos. |
| **Inventario fantasma y sobreventa en temporada alta (`prevención de quiebres de stock`)** | Shopify muestra más unidades disponibles de las que realmente hay en las estanterías del 3PL, lo que hace que los anuncios de pago generen pedidos que debes cancelar y reembolsar. | Marca cada SKU en el que **el stock digital del escaparate supera el stock físico del 3PL** para que corrijas los niveles de inventario antes de la sobreventa. |
| **Parálisis por análisis del recuento cíclico (`Top 10 SKU por valor de pérdida`)** | Recorrer miles de filas de hojas de cálculo tras un recuento cíclico de almacén mientras se pasan por alto los 5 SKU que generan el 80% de tu pérdida financiera. | Filtra automáticamente las filas coincidentes y clasifica los **10 SKU con mayor pérdida en dólares** en un dashboard resumen para una acción inmediata. |

---

## Tutorial de inicio rápido: cómo conciliar el inventario de Shopify, WMS y 3PL en 4 pasos

No necesitas habilidades avanzadas de Excel ni fórmulas `VLOOKUP` manuales para realizar una auditoría de almacén. Sigue estos cuatro pasos para convertir exportaciones CSV en bruto en un claro **informe de discrepancias y merma de inventario**:

### Paso 1: Introduce tu lista maestra de SKU, el COGS unitario y los umbrales de alerta (`Config_Master`)
Abre la pestaña `Config_Master` para establecer tus reglas de inventario de referencia:
- Pega tu **lista maestra de SKU** y tu **coste de bienes vendidos unitario (COGS)**.
- Configura tus **umbrales de advertencia de discrepancia personalizados** (por ejemplo, marcar cualquier SKU con un faltante de más de `5 unidades` o más de `$100` en valor de inventario faltante).

*Vista previa en vivo:* mira cómo funciona la tabla de configuración maestra ahora mismo en la [calculadora de navegador gratuita de conciliación de inventarios 3PL](https://hyvoid.github.io/multi-node-inventory-reconciliation/).

---

### Paso 2: Copia y pega tus exportaciones CSV en bruto de Shopify, WMS y 3PL
Olvídate del formateo manual de columnas y de la limpieza de texto. Pega tus exportaciones de inventario en bruto directamente en las tres pestañas de entrada:
- `Import_Shopify`: tu CSV de inventario de productos de Shopify (niveles de stock del escaparate).
- `Import_WMS`: tu informe de stock interno del sistema de gestión de almacén o del ERP.
- `Import_3PL`: el recuento físico cíclico o el informe de inventario final de tu socio de fulfillment (compatible con exportaciones de ShipBob, ShipMonk, Flexport, Amazon MCF y portales 3PL personalizados).
- **Cero arrastre manual de fórmulas:** las tablas preconfiguradas limpian los espacios sobrantes, alinean los códigos SKU y se expanden automáticamente al pegar nuevas filas.

---

### Paso 3: Consulta tu dashboard de merma y el Top 10 de SKU por valor de pérdida (`Dashboard`)
Cambia a la pestaña `Dashboard` para ver los resultados completos de tu auditoría:
- Consulta el **valor total de merma de inventario ($)**, la **variación neta de unidades** y las **tasas de exactitud entre sistemas (%)** calculadas automáticamente.
- Revisa la lista de **Top 10 SKU por valor de pérdida** para ver qué productos exactos necesitan un nuevo recuento físico en el almacén o un ajuste urgente de stock en Shopify.

---

### Paso 4: Descarga la plantilla Excel desbloqueada para auditorías mensuales con un clic
Usa la herramienta gratuita del navegador para probar tu flujo de trabajo y detectar huecos de stock inmediatos hoy mismo. Para guardar tus costes de SKU de referencia en local, ejecutar cierres contables mensuales recurrentes y construir un historial de reclamaciones al 3PL, descarga la hoja de cálculo `.xlsx` desbloqueada.

> 💡 **Por qué las marcas de ecommerce en crecimiento usan esta plantilla Excel en lugar de construirla desde cero:**  
> Limpiar cadenas de SKU desordenadas de tres exportaciones distintas, alinear filas no coincidentes y ponderar variaciones de stock por el COGS unitario implica una engorrosa ingeniería de hojas de cálculo. **En esta plantilla Excel, cada regla de emparejamiento a tres bandas, normalizador de texto y fórmula de actualización automática ya está construido para ti.**  
> 
> Ni siquiera necesitas hacer doble clic en las esquinas de las celdas ni arrastrar fórmulas hacia abajo. Descarga el libro de trabajo a tu ordenador, pega tus exportaciones mensuales de Shopify y del 3PL sobre los datos del mes anterior y obtén una auditoría financiera de merma actualizada con un clic. Incluso sin experiencia técnica en hojas de cálculo, obtienes visibilidad instantánea de la salud de tu inventario — liberándote para centrarte en el marketing, reabastecer los superventas y cerrar ventas durante los picos del Q4 y Black Friday mientras una sencilla plantilla de copiar y pegar se encarga de la conciliación de datos.  
> 
> 👉 **[Descarga hoy la plantilla Excel desbloqueada de conciliación de inventarios Shopify y 3PL (.xlsx) y automatiza tus auditorías de stock](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)**

---

## La lógica de negocio y la metodología: 4 puntos ciegos de inventario que esta plantilla Excel resuelve por ti

La mayoría de las marcas de ecommerce pierden miles de dólares por merma de inventario y sobreventa, no porque olviden contar el stock, sino porque las comprobaciones estándar a dos bandas y las hojas de cálculo básicas de unidades ocultan dónde se produce el daño financiero real. Así protege esta plantilla tu inventario y tu flujo de caja, en términos sencillos:

### 1. Comparar solo dos sistemas oculta si se trata de un bug de TI o de un robo en el almacén (triangulación de inventario a 3 bandas)
**El hecho objetivo:** si solo comparas Shopify (100 unidades) con tu 3PL (80 unidades), sabes que faltan 20 unidades, pero no sabes *por qué*. Esas 20 unidades pueden estar en pedidos no enviados porque falló un webhook de API, o 20 cajas físicas pudieron salir del almacén por la puerta trasera.  
**Tu beneficio directo:** al emparejar **Shopify (escaparate digital) + WMS (registro interno) + 3PL (recuento físico de estanterías)** lado a lado en una misma fila, la plantilla aísla el punto exacto de ruptura:
- Si `Shopify ≠ WMS`, pero `WMS = 3PL`: tienes un retraso de sincronización del escaparate o de pedidos pendientes de envío. Corrige la configuración de tu integración.
- Si `Shopify = WMS`, pero `3PL < WMS`: el stock físico se perdió, se dañó o se contó mal en el centro de fulfillment. Presenta una reclamación al 3PL.

### 2. Contar unidades faltantes en lugar de dólares faltantes desperdicia mano de obra de almacén (clasificación de variaciones ponderada por COGS)
**El hecho objetivo:** una hoja de recuento cíclico estándar trata todas las unidades por igual. Si tu equipo ordena las discrepancias solo por número de unidades, pasará horas contando de nuevo suministros de embalaje baratos mientras ignora productos de alto coste que drenan silenciosamente tu margen. Mira cómo los recuentos brutos de unidades engañan a los equipos de almacén frente a la merma ponderada por COGS:

```text
SKU-A (Branded Poly-Mailer):   -50 Units Missing  ×  $0.20 Unit COGS  =   -$10.00 Financial Loss
SKU-B (Wireless Headphones):    -4 Units Missing  × $115.00 Unit COGS =  -$460.00 Financial Loss

```

En una hoja de cálculo básica por número de unidades, `SKU-A` (-50 unidades) parece una emergencia mientras `SKU-B` (-4 unidades) parece un simple error de redondeo — a pesar de que `SKU-B` cuesta a tu negocio **46 veces más dinero**.

**Tu beneficio directo:** la plantilla multiplica automáticamente cada discrepancia de unidades por su COGS unitario y clasifica tus **Top 10 SKU por valor de pérdida según impacto en dólares**. Tu equipo investiga primero la pérdida de $460 en lugar de perseguir $10 en sobres de envío.

### 3. Los contratos de fulfillment con 3PL tienen plazos estrictos de reclamación y límites de merma (prueba documentada de reclamación SLA)

**El hecho objetivo:** casi todos los contratos de logística tercerizada (3PL) incluyen una "tolerancia de merma" incorporada (normalmente el 0,5% al 2,0% del total de unidades gestionadas) y exigen que los comerciantes presenten pruebas de variación SKU por SKU dentro de los 15 a 30 días posteriores a un recuento cíclico para optar al reembolso. Las quejas enviadas por correo electrónico sin registros de variaciones estructurados son rechazadas de forma rutinaria por los gestores de cuenta del 3PL.

**Tu beneficio directo:** la plantilla calcula **porcentajes exactos de discrepancia entre nodos** y genera una tabla limpia de variaciones a nivel de SKU que muestra el stock esperado, el recuento físico, el déficit de unidades y el valor en COGS — dándote documentación lista para enviar y recuperar dinero de tu 3PL.

### 4. El "inventario fantasma" en Shopify quema el gasto publicitario pagado y desencadena reclamaciones de contracargo (detección de stock fantasma)

**El hecho objetivo:** cuando tu tienda de Shopify cree que tienes 50 unidades en stock, tus anuncios de shopping de Meta y Google siguen gastando dinero para atraer tráfico a esa página de producto. Si tu 3PL en realidad tiene 0 unidades en la estantería ("inventario fantasma"), cada nuevo pedido de cliente se traduce en un retraso de fulfillment, una cancelación manual, comisiones de procesamiento de pago perdidas y tickets de soporte de clientes furiosos.

**Tu beneficio directo:** la plantilla resalta cada SKU en el que la disponibilidad del escaparate supera el stock físico del almacén para que ajustes las cantidades de inventario de Shopify antes de sobrevender en eventos de venta de alto tráfico.

---

## Hojas de cálculo de inventario manuales (`VLOOKUP`) vs. esta plantilla automatizada de conciliación Shopify y 3PL

| Factor de comparación de almacén y contabilidad | Hojas Excel manuales (`VLOOKUP` / `INDEX-MATCH` desde cero) | Plantilla estandarizada de conciliación de inventarios multinodo (esta herramienta) |
| --- | --- | --- |
| **Alineación de stock entre 3 sistemas (`Shopify` + `WMS` + `3PL`)** | El personal une manualmente tres archivos CSV distintos cada mes, con riesgo de referencias de celda rotas y SKU omitidos. | El **motor de emparejamiento a 3 bandas** preconfigurado alinea automáticamente las cantidades de Shopify, WMS y 3PL en cuanto pegas tus exportaciones. |
| **Formato CSV desordenado y SKU no coincidentes** | Los espacios finales, los ceros iniciales y los códigos SKU en mayúsculas/minúsculas generan falsos errores `#N/A` en miles de filas. | Una **capa de normalización de texto** integrada limpia los espacios en blanco y estandariza las cadenas de SKU antes de calcular las diferencias de stock. |
| **Valoración financiera de la merma (`castigo contable por COGS`)** | Los informes solo muestran cantidades de unidades faltantes, obligando a los contables a buscar costes de producto manualmente en el cierre mensual. | Una **matriz de costes de SKU** integrada convierte cada escasez de unidades en una **exposición exacta de merma en dólares ($)** para asientos contables. |
| **Filtrado de excepciones (`SKU con mayores pérdidas`)** | Los gestores recorren más de 5.000 filas coincidentes intentando detectar qué productos tienen huecos de stock peligrosos. | El **dashboard de excepciones automatizado** filtra las filas normales y clasifica automáticamente los **10 SKU con mayor pérdida en dólares**. |
| **Documentación de reembolsos SLA del 3PL** | Las unidades faltantes del almacén se discuten informalmente por correo electrónico, sin porcentajes de exactitud históricos ni totales en dólares. | Produce un **registro de variaciones y tasas de discrepancia del 3PL** listo para auditoría para sustanciar reclamaciones formales de crédito y reembolso SLA. |

---

## Para quién es: roles de ecommerce, casos de uso de inventario y flujos de trabajo de hojas de cálculo

Esta caja de herramientas cierra la brecha entre las estanterías físicas del almacén y los estados financieros del ecommerce. Está construida para **marcas DTC en crecimiento, vendedores multicanal de Shopify, usuarios de 3PL y equipos financieros de ecommerce** que quieren un control de inventario fiable sin pagar más de $30.000 al año por un ERP empresarial:

* **Propietarios de tiendas Shopify y fundadores de marcas DTC (`plantilla Excel de conciliación de inventarios Shopify`):** detecta stock fantasma e inventario faltante en el almacén en minutos, sin contratar a un analista de datos ni aprender fórmulas complejas de hojas de cálculo.
* **Gestores de operaciones y fulfillment de ecommerce (`hoja de cálculo de auditoría de discrepancias de stock y SLA del 3PL`):** exija responsabilidades a los centros de fulfillment externos (como ShipBob, ShipMonk o 3PL regionales) siguiendo las tasas de merma mensuales frente a los límites SLA contractuales.
* **Gestores de almacén y encargados de control de inventario (`calculadora plug-and-play de variación de recuento cíclico`):** concilia los recuentos físicos de ubicaciones con los registros del WMS tras recuentos cíclicos semanales o mensuales, priorizando los nuevos recuentos por el mayor valor en dólares en riesgo.
* **Contables de ecommerce y CFOs externos (`modelo contable de merma de inventario y castigo por COGS`):** calcula ajustes exactos de valoración del inventario final y castigos contables de merma por COGS a fin de mes para QuickBooks Online, Xero o NetSuite.
* **Vendedores multicanal de Amazon, Walmart y Shopify (`hoja de comparación de stock multialmacén`):** audita la distribución de stock y las cantidades de SKU sin vincular entre almacenes internos, nodos 3PL y canales de venta online desde un único archivo.

*Nota: este libro de trabajo de Excel no sustituye a los escáneres de códigos de barras en tiempo real, a las aplicaciones de sincronización de inventario por API en vivo ni a tu WMS. Actúa como tu **capa independiente de auditoría y conciliación** para detectar los fallos de sincronización y la merma física que el software automatizado pasa por alto.*

---

## Escenarios del mundo real: cómo resolver problemas comunes de inventario de Shopify y 3PL

Si tu equipo de operaciones o finanzas se encuentra con cualquiera de estos dolores de cabeza recurrentes de inventario, esta hoja de cálculo está estructurada para resolverlos de inmediato:

* **Cómo prevenir la sobreventa durante el Black Friday / Cyber Monday (temporada alta del Q4):** Shopify muestra 100 unidades disponibles, pero tu 3PL solo tiene 20 en la estantería. Ejecuta esta conciliación semanalmente durante el Q4 para detectar el "inventario fantasma" y sincronizar los recuentos de tu escaparate antes de que los clientes compren artículos agotados.
* **Cómo probar el inventario perdido del 3PL y reclamar reembolsos SLA:** tu socio de fulfillment pierde SKU de alto valor por encima de su tolerancia contractual de merma del 1,5%. Pega tus registros de envíos del WMS y el recuento físico del 3PL en la plantilla para generar un informe detallado de pérdidas en dólares para tu reclamación.
* **Cómo calcular la merma de inventario a fin de mes para la contabilidad de ecommerce:** tu contable necesita una cifra exacta en dólares del stock perdido o dañado para cerrar el P&L mensual. Usa el total ponderado por COGS del dashboard para registrar asientos contables de castigo de inventario precisos en minutos.
* **Cómo conciliar exportaciones CSV de almacén desordenadas sin fórmulas `VLOOKUP` rotas:** los distintos sistemas exportan códigos SKU con espacios de más o formato inconsistente. Suelta las exportaciones en bruto en las pestañas de importación y deja que la plantilla alinee y compare cada SKU automáticamente.

---

## Acerca de Theseus Workshop

**Theseus Workshop** construye modelos de Microsoft Excel plug-and-play y herramientas de decisión basadas en navegador para operadores que necesitan números claros y fiables hoy mismo — sin software empresarial inflado ni programación compleja de hojas de cálculo.

Cada herramienta está diseñada en torno a una pregunta práctica:

> **"¿Qué cifras operativas y financieras exactas deben estar en una tabla preconfigurada para que tu próxima decisión de negocio tarde segundos en lugar de horas?"**

Si quieres dejar de luchar contra hojas `VLOOKUP` rotas, quiebres de stock inesperados y pérdidas de inventario del 3PL sin compensar, descarga la plantilla Excel completa a continuación o explora nuestra biblioteca completa de hojas de cálculo operativas:

* 📥 **Descarga esta plantilla de conciliación de inventarios:** [Descarga la plantilla Excel desbloqueada de conciliación de inventarios Shopify y 3PL (.xlsx)](https://www.theseusworkshop.com/l/ddongr?utm_source=github&utm_medium=GitHub%20README&utm_campaign=readme%20new%20launch&utm_content=inventory-reconciliation-shrinkage)
* 🌐 **Prueba la calculadora web gratuita:** [Abre el simulador de navegador interactivo de conciliación de inventarios 3PL](https://hyvoid.github.io/MULTI-NODE-INVENTORY-RECONCILIATION/)
* 🧰 **Explora todos los modelos Excel listos para usar y cajas de herramientas de negocio:** [Visita la tienda oficial de Theseus Workshop en TheseusWorkshop.com](https://www.google.com/search?q=https://www.theseusworkshop.com%3Futm_source%3Dgithub%26utm_medium%3DGitHub%2520README%26utm_campaign%3Dreadme%2520new%2520launch%26utm_content%3Dinventory-readme-store-link)

---


## Detalles técnicos

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
| `Dashboard`      | Decisión      | Resumen de KPI, exposición a pérdidas, comparación de nodos, Top 10 de excepciones            | Dirección / Gerencia    |
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

Por eso este libro de trabajo se entiende mejor como una **capa de apoyo a decisiones** que como una simple hoja de cálculo de comparación de inventarios.

### Tres trampas que atrapan incluso a operadores de inventario con experiencia

#### Trampa 1 — Tratar cada diferencia de cantidad como merma

**Decisión:**
Un operador ve que Shopify reporta 1,000 unidades mientras el 3PL reporta 970 y registra de inmediato 30 unidades como perdidas.

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
| Shopify |    1,000 |
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

La siguiente acción no es inspeccionar cada SKU por igual. El operador debe investigar primero la **excepción del lado del 3PL**, verificar si la variación representa pérdida física, daño, un problema de timing o de reporte, y luego determinar si la discrepancia excede la tolerancia contractual o interna de la empresa.

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

Estos requieren un TMS dedicado, no una hoja de conciliación de inventarios.

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

Estos límites son explícitos en el diseño fuente. La conciliación estandarizada, la valoración de discrepancias, la clasificación de excepciones y el reporte del dashboard se consideran problemas apropiados para Excel. La disciplina de recuento cíclico y la gestión de reclamaciones al 3PL requieren controles de gestión; la sincronización de API en tiempo real pertenece a la integración de sistemas; el seguimiento de envíos físicos pertenece a un TMS.

También hay importantes restricciones de interpretación.

**Una diferencia de cantidad no es automáticamente merma.** Las devoluciones pueden registrarse por un 3PL en un momento distinto del reembolso correspondiente en Shopify, y un timing inconsistente de las instantáneas puede crear diferencias temporales. El operador debe validar el contexto de negocio antes de clasificar una discrepancia como pérdida permanente.

**La cifra de pérdida financiera es una estimación, no un asiento contable.** Depende del coste unitario de SKU configurado y de la interpretación de la diferencia de cantidad subyacente.

**Un resultado limpio de la hoja de cálculo no garantiza datos fuente limpios.** Las inconsistencias históricas de nomenclatura de SKU, las exportaciones incompletas, los registros duplicados o los recuentos físicos incorrectos aún pueden producir conclusiones engañosas.

Por tanto, el libro de trabajo debe usarse como un **mecanismo de investigación de hechos y priorización**, no como un motor de juicio automático.

</details>


## Otras herramientas de esta serie

Una colección de herramientas ligeras de apoyo a decisiones en Excel que cubren control operativo, conciliación, rentabilidad, inventario y análisis financiero.

* **[inventory-planning-reorder-point-excel](https://github.com/HyVoid/inventory-planning-reorder-point-excel)** — ¿Qué decisión de compra debe tomarse hoy dadas las tendencias de demanda, los plazos de entrega y las restricciones de caja? — Prevé las necesidades de inventario combinando señales de demanda, riesgo de plazo, recomendaciones de compra y exposición del capital de trabajo.
* **[Retail-SKU-Concentration-Assortment-Diagnostic-Console](https://github.com/HyVoid/Retail-SKU-Concentration-Assortment-Diagnostic-Console)** — ¿Qué productos dominan el riesgo de inventario o diluyen la calidad del surtido? — Identifica el riesgo de concentración de SKU y la eficiencia del surtido en catálogos de productos minoristas.
* **[Retail-and-Maquila-Inventory-Ledger](https://github.com/HyVoid/Retail-and-Maquila-Inventory-Ledger)** — ¿Dónde se mueve el inventario entre las operaciones minoristas y de maquila? — Sigue los movimientos de inventario, las pérdidas de procesamiento y la exposición de stock entre fábricas, almacenes y tiendas.
* **[Universal-3D-Cargo-Loading-Optimization-Simulator](https://github.com/HyVoid/Universal-3D-Cargo-Loading-Optimization-Simulator)** — ¿Cómo debe cargarse la mercancía para reducir el espacio desperdiciado y la fricción operativa? — Simula configuraciones de carga 3D para maximizar la capacidad de contenedores y la eficiencia de envío.
* **[Cross-Border-DTC-Inventory-Governance-Console](https://github.com/HyVoid/Cross-Border-DTC-Inventory-Governance-Console)** — ¿Cuál es la demanda real de compra tras eliminar los compromisos de preventa y las devoluciones esperadas? — Reconstruye señales de demanda reales aislando las obligaciones de preventa y el comportamiento de devolución de los datos de ventas brutos.
* **[inventory-allocation-fulfillment-excel](https://github.com/HyVoid/inventory-allocation-fulfillment-excel)** — ¿Puede cada pedido de cliente entregarse realmente a tiempo dado el stock físico, las reservas, los contenedores en tránsito y las órdenes de compra abiertas en todas nuestras ubicaciones? — Calcula las cantidades disponibles para prometer y las necesidades netas de aprovisionamiento conciliando el stock físico, las reservas de pedidos, el inventario en tránsito y las órdenes de compra abiertas en múltiples ubicaciones.

## Licencia

Este proyecto se publica bajo la **Licencia Apache 2.0**.

Puede usar, modificar, distribuir y adaptar el proyecto conforme a los términos y condiciones de la Licencia Apache 2.0.

Consulta el archivo de licencia del repositorio para ver el texto completo de la licencia.

