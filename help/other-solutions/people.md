---
description: La métrica Personas es el recuento de personas (o grupos de dispositivos) según el gráfico de dispositivos del Adobe. Puede aplicar la métrica Personas para identificar a los visitantes en sus dispositivos en Analysis Workspace.
seo-description: The People metric is the count of people (or groups of devices) based on Adobe's Device Graph. You can apply the People metric to identify visitors across their devices in Analysis Workspace.
seo-title: People metric
title: Métrica Personas
uuid: 8e731779-044d-4d31-a19a-f579a9c8c471
exl-id: e2e70461-19ab-49db-bd65-a3eb26c2d4a8
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '1374'
ht-degree: 4%

---

# Métrica Personas{#people-metric}

La métrica Personas es el recuento de personas (o grupos de dispositivos) según el gráfico de dispositivos del Adobe. Puede aplicar la métrica Personas para identificar a los visitantes en sus dispositivos en Analysis Workspace.

## Requisitos previos y consideraciones de la métrica Personas {#section-34551d0435fb4b3cb3fad736b7961541}

<table id="table_120F7EF50042485391E58B22DD00A2A8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Requisito previo para la consideración </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Device Co-op </p> </td> 
   <td colname="col2"> <p> Para usar la métrica Personas, conviértase en miembro de <a href="http://landing.adobe.com/en/na/events/summit/275658-summit-co-op.html" format="html" scope="external"> Cooperación entre dispositivos de Adobe Experience Cloud</a>. La cooperación identifica los múltiples dispositivos (o ID de Experience Cloud) de una persona. Analytics aprovecha esta información para derivar estadísticamente la cantidad de personas que interactúan con una marca. La métrica tiene una precisión de dentro del 5 %. </p> <p><b>Regiones</b>: en este momento, Device Co-op solo está disponible en EE. UU. y Canadá. Por lo tanto, al evaluar la métrica Personas, debe aplicar un segmento al análisis que filtre los datos solo para EE. UU. y Canadá. </p> <p>Cada semana, Device Graph calcula una nueva versión de la cooperación y la publica para su uso. Los martes, el sistema recopila los datos más recientes y publica una versión actualizada del gráfico. A continuación, las soluciones de Experience Cloud utilizan la última versión del gráfico. Específicamente para Analytics, los cambios se leen los miércoles y su procesamiento suele tardar entre 1 y 2 días hábiles. </p> <p> <p>Importante: Cuando el gráfico se actualiza semanalmente, puede afectar históricamente a la métrica Personas. En otras palabras, los recuentos históricos de personas pueden cambiar con el tiempo a medida que el gráfico aprende y se actualiza. Por ejemplo, si ejecuta hoy un informe que cuenta Personas el mes pasado y, a continuación, ejecuta el mismo informe en una semana después de que se haya actualizado el gráfico, el recuento histórico de Personas puede cambiar ligeramente. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Permisos de métricas </td> 
   <td colname="col2"> <p>Solo puede usar la métrica Personas si se le ha concedido acceso. Los administradores pueden<a href="https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/customize-report-access/groups-metrics.html" format="html" scope="external"> personalizar permisos de métricas</a> en las Herramientas de administración. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Asignación a la organización de IMS </td> 
   <td colname="col2"> <p>La métrica Personas se habilitará para todos los grupos de informes que <a href="https://docs.adobe.com/content/help/es-ES/core-services/interface/about-core-services/report-suite-mapping.html" format="html" scope="external"> asignado a un IMSORG</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Herramientas/proyectos de análisis </p> </td> 
   <td colname="col2"> <p>Uso de la métrica Personas en <span class="wintitle"> Analysis Workspace</span>, <span class="wintitle"> Ad Hoc Analysis</span>, <span class="wintitle"> Report Builder</span>y a través de la API. Puede usarlo dondequiera que utilice la métrica Visitantes únicos, incluidas las Métricas calculadas. </p> <p>Por ejemplo, cree una métrica de ingresos por persona para reemplazar una métrica de ingresos por visitante único. </p> <p>A <a href="https://docs.adobe.com/content/help/es-ES/analytics/analyze/analysis-workspace/build-workspace-project/starter-projects.html" format="html" scope="external"> Plantilla del proyecto Personas</a> está disponible para empezar a utilizar la métrica Personas en Analysis Workspace. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activar reglas de bots </p> </td> 
   <td colname="col2"> <p>El Adobe recomienda activar <a href="https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/bot-removal/bot-rules.html" format="html" scope="external"> Reglas de bots</a>, especialmente al usar la métrica Personas. </p> <p>Cuando un bot rastrea el sitio web, aumenta artificialmente el recuento de visitantes únicos. La eliminación del tráfico de bots del grupo de informes ofrece una medición más precisa de la actividad en sus propiedades digitales, tanto en términos de visitantes únicos como de personas. </p> <p>Para ello, vaya a <span class="uicontrol"> Analytics</span> &gt; <span class="uicontrol"> Administrador</span> &gt; <span class="uicontrol"> Grupos de informes</span>. Seleccione el grupo de informes correcto y vaya a <span class="uicontrol"> Editar configuración</span> &gt; <span class="uicontrol"> General</span> &gt; <span class="uicontrol"> Reglas de bots</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Consideraciones de segmentación </p> </td> 
   <td colname="col2"> <p> Cuando utiliza segmentos con la métrica Personas, los informes de la métrica pueden ser considerablemente inferiores a lo esperado. </p> <p>Consulte <a href="../other-solutions/people.md#section-d03525420dbe48379fd95b230ef05885" format="dita" scope="local"> Uso de la métrica Personas con segmentos</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## ¿Qué es la métrica Personas? {#section-89e2b8f5e80f480391449fc8d1117a6a}

La métrica Personas es una métrica para informes de Analytics que le ayuda a atribuir dispositivos a personas. Proporciona una vista del marketing basada en personas, lo que permite medir la actividad de los visitantes en todos sus dispositivos. Considérelo como una versión deduplicada de Visitantes únicos y puede utilizar la métrica Personas para el análisis en la que anteriormente utilizaba Visitantes únicos.

**Los dispositivos son personas**

Antes de que la métrica Personas estuviera disponible, una persona (por ejemplo) podría visitar su sitio, interactuar con una campaña o marca en tres dispositivos diferentes y realizar una compra, incluso en cuestión de minutos. Según la implementación, Analytics podría informar cada dispositivo como un visitante único y atribuir 10 $ a tres dispositivos en una compra de 30 $.

La métrica Personas le permite atribuir con precisión esa compra de 30 $ a una persona:

![](assets/people-centric-results.png)

**Mayor precisión en los informes**

La métrica Personas permite pensar en varios dispositivos como una sola entidad. El siguiente proyecto de Analysis Workspace muestra comparaciones de mayor precisión entre los informes de Visitantes únicos y Personas:

![](assets/people_report.png)

Comparar personas y visitantes únicos en paralelo:

![](assets/people-report.png)

**Definiciones**

<table id="table_F8171AF15DA64607B427E3739EF004D6"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Elemento </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Personas </p> </td> 
   <td colname="col2"> <p>La métrica Personas se basa en la idea de que los consumidores interactúan con su marca mediante varios dispositivos. Cuanto más se segmentan o se segmentan los datos, menor es la probabilidad de que la misma persona utilice varios dispositivos dentro de ese segmento de datos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Visitantes únicos </p> </td> 
   <td colname="col2"> <p>Por ejemplo, cuanto más corte los datos por fecha u hora, menor será la diferencia entre Personas y Visitantes únicos. Si desea comprender bien el impacto general de la cooperación entre dispositivos, Adobe recomienda utilizar un intervalo de fechas de los últimos 90 días </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Compresión </p> </td> 
   <td colname="col2"> <p>Con una métrica calculada simple puede ver cuánto más pequeña es la métrica Personas como porcentaje de Visitantes únicos. Haga clic en el icono de información junto a "Compresión" en la tabla anterior para ver cómo crear esta métrica. </p> <p>Se pueden usar personas en otras métricas calculadas en lugar de Visitantes únicos. </p> </td> 
  </tr> 
 </tbody> 
</table>

## ¿Cómo se calcula la métrica Personas? {#section-0dfb762867e14a7f927796ef3c50592b}

<!--
<p>Analytics uses the HyperLogLog statistical algorithm to calculate People. This means that the smaller the data set, the margin for error may increase. No more than 5% of the numbers should be off by more than 5% </p>
-->

La siguiente imagen muestra cómo se calcula la métrica Personas y cómo puede disminuir con el tiempo para el mismo intervalo de fechas del informe en el pasado.

![](assets/people-calculations.png)

En este ejemplo, supongamos que hay un conjunto fijo de visitantes. Si ejecuta un informe durante un período de tiempo fijo en el pasado, mostrará un conjunto fijo de visitantes. Si Device Graph genera los datos mostrados en el gráfico izquierdo en la semana 1, el resultado es 90 personas. Una semana después, después de la siguiente ejecución de Device Graph, se tiene en cuenta nueva información. Si se ejecuta el mismo informe que hace una semana, el número de personas se ha reducido a 84. El historial ha cambiado porque Device Graph proporciona nueva información sobre los dispositivos que deben agruparse.

## Uso de la métrica Personas con segmentos {#section-d03525420dbe48379fd95b230ef05885}

Cuando utiliza segmentos con la métrica Personas, los resultados de la métrica pueden ser considerablemente inferiores a lo esperado. Este problema se produce porque, en la segmentación, no hay *`person`* contenedor. La segmentación utiliza el contenedor de visitante, que es el contenedor de nivel superior en la definición y se basa en el dispositivo, no en la persona.

Este problema se produce principalmente al apilar segmentos con la métrica Personas.

![](assets/people-stacked-segments.png)

El apilamiento de segmentos crea un nuevo segmento que representa la combinación de los mismos. El apilamiento de segmentos se produce siempre que:

* Coloque un segmento sobre otro segmento en Analysis Workspace. (Se unen automáticamente usando la variable *`And`* operador.)
* Aplique un solo segmento que contenga *`And`* operador.
* Aplique un segmento tanto en el nivel de proyecto como en el de tabla.
* Utilice un grupo de informes virtuales con otro segmento.

Por ejemplo, imaginemos que apilamos los siguientes segmentos en la métrica Personas:

* `Campaign = Spring Promotion`
* `Site Section = Product Overview`

Solo el número de personas que cumplen los requisitos en ambos segmentos *`using a single device`* se cuentan. (La métrica Personas no muestra el número de personas aptas entre dispositivos).

Además, el uso de *`Or`* no se recomienda el uso del operador en esta situación. Al hacerlo, se generaría un recuento de las personas que vieron uno de los segmentos o el otro, sin forma de contar cuántas personas cumplen los requisitos para ambos.

Consulte [Generación de segmentos](https://docs.adobe.com/content/help/es-ES/analytics/components/segmentation/segmentation-workflow/seg-build.html) en la ayuda de Segmentación para obtener más información.

## Tipos de dispositivos {#section-8ab378c84ff34574b9c20fecb3848a86}

La métrica Cooperación entre dispositivos y Personas funciona mejor en Adobe Analytics cuando el grupo de informes contiene datos de varios tipos de dispositivos. Por ejemplo, la combinación de datos web y de aplicaciones en el mismo grupo de informes hace que la métrica Personas sea más potente y eficaz. Cuanto más cruce de dispositivos tenga los datos, más buena será la posibilidad de que varios visitantes únicos se agrupen como una sola persona.

![](assets/people-device-types.png)

## Cobertura del servicio de ID de Experience Cloud {#section-bbf0098cac2e467289e7a644a1dea05c}

Device Co-Op requiere que las propiedades digitales se instrumenten mediante el servicio de ID de Experience Cloud (MCID). Si los datos del grupo de informes contienen un número significativo de visitantes sin ECID, la eficacia de Device Co-op y de la métrica Personas disminuye.

<!--
mcdc-people-metric-apply.xml
-->

En Analysis Workspace, cree un [proyecto](https://docs.adobe.com/content/help/es-ES/analytics/analyze/analysis-workspace/build-workspace-project/t-freeform-project.html), luego arrastre el **[!UICONTROL People]** métrica a la tabla del proyecto:

![](assets/people-metric.png)
