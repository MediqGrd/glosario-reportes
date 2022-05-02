Indicadores Egresos
================
Med-iQ GRD
2021-11-24

# 1. Indicadores Análisis Clínica

Corresponde a indicadores utilizados en primera pestaña y mayoría del
reporte.

-   **Egresos**: Cantidad de Egresos.

#Total Episodios

-   **% Outliers**: Proporción de de casos marcados como Outlier
    Superior.

$$
\\frac{\\text{\\# Episodios Outlier Superior}}{\\text{\\# Total Episodios}}
$$

-   **% Reingresos (Generados)**: Proporción de de casos marcados
    predecesor de un reingreso en urgencia dentro de 30 días, para misma
    Categoría Diagnóstica Mayor (CDM).

$$
\\frac{\\text{\\# Episodios predecesores de reingreso}}{\\text{\\# Total Episodios}}
$$

-   **Peso GRD**: Peso GRD promedio de la muestra

$$
 \\frac{\\sum\_{}^{}\\text{Peso GRD por Episodio}}{\\text{\\# Total Episodios}}
$$

-   **Índice de Días de Estada**: Total de Días observados contra total
    de días en norma de referencia, ajustado por GRD.

$$
 \\frac{\\sum\_{}^{}\\text{Total Días Ajustados por GRD}}{\\sum\_{}^{}\\text{Total Días Ajustados por GRD en Referencia}}
$$

-   **Índice de Gasto**: Total de Gasto cargado a sistema contra total
    de gasto según norma de referencia, ajustado por GRD. El Gasto viene
    del vector de costo o facturación, configurable en panel lateral.

$$
 \\frac{\\sum\_{}^{}\\text{Total Gasto Ajustado por GRD}}{\\sum\_{}^{}\\text{Total Gasto Ajustado por GRD en Referencia}}
$$

-   **Ingresos Ganados**: Diferencial entre ingresos hospitalarios a
    favor o en contra de la casuística observada contra la referencia.
    Si es negativo, son cantidad de ingresos hospitalarios perdidos
    respecto a esta referencia, siempre ajustado por GRD.

$$
 \\frac{\\text{Impacto}}{\\text{EMAF}} \* -1
$$

# 2. Indicadores Funcionales

Indicadores clásicos contenidos en pestaña 6 de reporte.

-   **Estancia Media ajustada por funcionamiento (EMAF)**: EM que
    hubiera la clínica aplicando en cada GRD a sus propios casos la
    estancia media del estándar.

$$
 \\frac{\\sum\_{}^{}\\text{EM Norma \* Altas Clínica}}{\\sum\_{}^{}\\text{Total Altas Observadas}}
$$

-   **Estancia Media ajustada por casuística (EMAC)**: EM que hubiera
    tenido la clínica atendiendo a la casuística del estándar en lugar
    de la propia, ajustado por GRD.

$$
 \\frac{\\sum\_{}^{}\\text{EM Clínica \* Altas Norma}}{\\sum\_{}^{}\\text{Total Altas Norma}}
$$

-   **Impacto**: Número de estancias evitables si la estancia media
    observada por GRD hubiese sido igual a la estándar. Al contrario de
    *Días Ganados*, si es negativo son días ganados o ahorrados respecto
    a referencia.

$$
 {\\sum\_{}^{}\\text{Altas Clínica \* (EM Clínica - EMAF)}}
$$

-   **Ingresos Potenciales**: Número de ingresos que podrían haberse
    evitado o que se han ahorrado con las estancias evitables, según
    proceda para cada GRD.

$$
 \\frac{\\text{Impacto}}{\\text{EMAF}}
$$

-   **Índice Funcional (IF)**: Razón entre la EM ajustada por la
    casuística y la EM de la norma. Entrega información sobre el patrón
    funcional de la clínica respecto al estándar, cuando es superior a 1
    habla de que lo observado es menos eficiente que el estándar.

$$
 \\frac{\\text{EMAC}}{\\text{EM Norma}}
$$

-   **IEMA**: Compara, para la casuística de la clínica, su
    funcionamiento con respecto al funcionamiento de la norma.

$$
 \\frac{\\text{EM Clínica}}{\\text{EMAF}}
$$
