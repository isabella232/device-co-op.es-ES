---
description: La métrica Personas es el recuento de personas (o grupos de dispositivos) según Device Graph de Adobe. Puede aplicar la métrica Personas para identificar visitantes en todos sus dispositivos en Analysis Workspace.
seo-description: La métrica Personas es el recuento de personas (o grupos de dispositivos) según Device Graph de Adobe. Puede aplicar la métrica Personas para identificar visitantes en todos sus dispositivos en Analysis Workspace.
seo-title: Métrica Personas
title: Métrica Personas
uuid: 8e731779-044d-4d31-a19a-f579a9c8c471
translation-type: tm+mt
source-git-commit: 822882d4f9bb9eed7cf116597b62d07bbe94376c
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 3%

---


# Métrica Personas{#people-metric}

La métrica Personas es el recuento de personas (o grupos de dispositivos) según Device Graph de Adobe. Puede aplicar la métrica Personas para identificar visitantes en todos sus dispositivos en Analysis Workspace.

## Requisitos y consideraciones de la métrica Personas {#section-34551d0435fb4b3cb3fad736b7961541}

<table id="table_120F7EF50042485391E58B22DD00A2A8"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Requisito previo o consideración </th> 
   <th colname="col2" class="entry"> Descripción </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>Device Co-op </p> </td> 
   <td colname="col2"> <p> Para utilizar la métrica Personas, conviértase en miembro de la <a href="http://landing.adobe.com/en/na/events/summit/275658-summit-co-op.html" format="html" scope="external"> Adobe Experience Cloud Device Co-op</a>. La cooperación identifica los múltiples dispositivos (o ID de Experience Cloud) de una persona. Analytics aprovecha esta información para derivar estadísticamente el número de personas que interactúan con una marca. La métrica tiene una precisión del 5 %. </p> <p><b>Regiones</b>: Device Co-op actualmente solo está disponible en EE. UU. y Canadá. Por lo tanto, al evaluar la métrica Personas, debe aplicar un segmento a la análisis que filtros los datos solo para EE. UU. y Canadá. </p> <p>Cada semana, Device Graph calcula una nueva versión de la cooperación y la publica para su uso. Los martes, el sistema recopila los datos más recientes y publica una versión actualizada del gráfico. A continuación, las soluciones Experience Cloud utilizan la versión más reciente del gráfico. Específicamente para Analytics, los cambios se leen los miércoles y el procesamiento de los cambios suele tardar entre 1 y 2 días hábiles. </p> <p> <p>Importante:  Cuando el gráfico se actualiza semanalmente, puede afectar históricamente a la métrica Personas. En otras palabras, los recuentos históricos de personas pueden cambiar con el tiempo a medida que el gráfico aprende y se actualiza. Por ejemplo: si ejecuta un informe hoy que cuenta Personas el mes pasado y luego ejecuta el mismo informe en una semana después de que se actualice el gráfico, el recuento de Personas histórico puede cambiar ligeramente. </p> </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Permisos de métricas </td> 
   <td colname="col2"> <p>La métrica Personas solo se puede usar si se le ha concedido acceso a ella. Los administradores pueden<a href="https://docs.adobe.com/content/help/en/analytics/admin/user-product-management/customize-report-access/groups-metrics.html" format="html" scope="external"> personalizar los permisos</a> de métricas en las Herramientas de administración. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> Asignación a la organización IMS </td> 
   <td colname="col2"> <p>La métrica Personas se habilitará para todos los grupos de informes que estén <a href="https://docs.adobe.com/content/help/es-ES/core-services/interface/about-core-services/report-suite-mapping.html" format="html" scope="external"> asignados a un IMSORG</a>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Herramientas/proyectos de análisis </p> </td> 
   <td colname="col2"> <p>Utilice la métrica Personas en <span class="wintitle"> Analysis Workspace</span>, <span class="wintitle"> Ad Hoc Analysis</span>, <span class="wintitle"> Report Builder</span>y mediante la API. Puede utilizarla siempre que utilice la métrica Visitantes únicos, incluidas las métricas calculadas. </p> <p>Por ejemplo, cree una métrica de ingresos por persona para reemplazar una métrica de ingresos por visitante único. </p> <p>Hay disponible una plantilla <a href="https://docs.adobe.com/content/help/es-ES/analytics/analyze/analysis-workspace/build-workspace-project/starter-projects.html" format="html" scope="external"></a> de proyecto Personas para empezar a utilizar la métrica Personas en Analysis Workspace. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Activar las reglas de bots </p> </td> 
   <td colname="col2"> <p>Adobe recomienda activar las reglas <a href="https://docs.adobe.com/content/help/en/analytics/admin/admin-tools/bot-removal/bot-rules.html" format="html" scope="external"> de</a>bots, especialmente al usar la métrica Personas. </p> <p>Cuando un bot rastrea su sitio web, aumenta artificialmente el recuento de Visitantes únicos. La eliminación del tráfico de bots del grupo de informes proporciona una medición más precisa de la actividad en las propiedades digitales, tanto en términos de Visitantes únicos como de Personas. </p> <p>Para ello, vaya a <span class="uicontrol"> Analytics</span> &gt; <span class="uicontrol"> Administración</span> &gt; <span class="uicontrol"> Grupos</span>de informes. Select the correct report suite, and then go to <span class="uicontrol"> Edit Settings</span> &gt; <span class="uicontrol"> General</span> &gt; <span class="uicontrol"> Bot Rules</span>. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Consideraciones de segmentación </p> </td> 
   <td colname="col2"> <p> Cuando se utilizan segmentos con la métrica Personas, el sistema de informes de la métrica puede ser considerablemente inferior al esperado. </p> <p>Consulte <a href="../other-solutions/people.md#section-d03525420dbe48379fd95b230ef05885" format="dita" scope="local"> Uso de la métrica Personas con segmentos</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

## ¿Qué es la métrica Personas? {#section-89e2b8f5e80f480391449fc8d1117a6a}

La métrica Personas es una métrica de sistema de informes de Analytics que le ayuda a atribuir dispositivos a personas. Proporciona una vista de marketing basada en las personas, lo que le permite medir la actividad de los visitantes en todos sus dispositivos. Considérela como una versión desdoblada de Visitantes únicos y puede usar la métrica Personas para la análisis, donde previamente utilizó Visitantes únicos.

**Los dispositivos son personas**

Antes de que la métrica Personas estuviera disponible, una persona (por ejemplo) podría visitar su sitio y participar en una campaña o marca en tres dispositivos diferentes y realizar una compra, incluso en cuestión de minutos. En función de la implementación, Analytics podría informar de cada dispositivo como un visitante único y atribuir 10 $ a tres dispositivos en una compra de 30 $.

La métrica Personas permite atribuir con precisión esa compra de 30 $ a una persona:

![](assets/people-centric-results.png)

**Mayor precisión en los informes**

La métrica Personas permite considerar varios dispositivos como una sola entidad. El siguiente proyecto de Analysis Workspace muestra comparaciones de mayor precisión entre el sistema de informes de Visitantes únicos y el sistema de informes de personas:

![](assets/people_report.png)

Comparar personas y Visitantes únicos en paralelo:

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
   <td colname="col2"> <p>La métrica Personas se basa en la idea de que los consumidores interactúan con su marca utilizando varios dispositivos. Cuanto más fracciona o segmenta los datos, menor es la probabilidad de que la misma persona utilice varios dispositivos dentro de esa fracción de datos. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Visitantes únicos </p> </td> 
   <td colname="col2"> <p>Por ejemplo, cuanto más fracciona los datos por fecha u hora, menor será la diferencia entre Personas y visitantes únicos. Si desea conocer el impacto general de Device Co-op, Adobe recomienda utilizar un intervalo de fechas de los últimos 90 días </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p>Compresión </p> </td> 
   <td colname="col2"> <p>Con una métrica calculada simple puede ver cuánto más pequeña es la métrica Personas como porcentaje de Visitantes únicos. Haga clic en el icono de información al lado de "Compresión" en la tabla de arriba para ver cómo crear esta métrica. </p> <p>Las personas pueden utilizarse en otras métricas calculadas en lugar de Visitantes únicos. </p> </td> 
  </tr> 
 </tbody> 
</table>

## ¿Cómo se calcula la métrica Personas? {#section-0dfb762867e14a7f927796ef3c50592b}

<!--
<p>Analytics uses the HyperLogLog statistical algorithm to calculate People. This means that the smaller the data set, the margin for error may increase. No more than 5% of the numbers should be off by more than 5% </p>
-->

La siguiente imagen muestra cómo se calcula la métrica Personas y cómo puede disminuir con el tiempo para el mismo intervalo de fechas del informe en el pasado.

![](assets/people-calculations.png)

En este ejemplo, supongamos que hay un conjunto fijo de visitantes. Si ejecuta un informe para un intervalo de tiempo fijo en el pasado, muestra un conjunto fijo de visitantes. Si Device Graph genera los datos mostrados en el gráfico izquierdo en la semana 1, el resultado es 90 personas. Una semana después, después de la siguiente ejecución de Device Graph, se tiene en cuenta nueva información. Si ejecuta el mismo informe que hace una semana, el número de personas ha bajado a 84. El historial ha cambiado porque Device Graph ha proporcionado nueva información sobre los dispositivos que deben agruparse.

## Uso de la métrica Personas con segmentos {#section-d03525420dbe48379fd95b230ef05885}

Cuando se utilizan segmentos con la métrica Personas, los resultados de la métrica pueden ser considerablemente menores de lo esperado. Este problema se debe a que, en la segmentación, no hay ningún *`person`* contenedor. La segmentación utiliza el contenedor de Visitante, que es el contenedor de nivel más alto en la definición y se basa en el dispositivo, no en la persona.

Este problema se produce principalmente al apilar segmentos con la métrica Personas.

![](assets/people-stacked-segments.png)

El apilamiento de segmentos crea un nuevo segmento que representa la combinación de los segmentos. El apilamiento de segmentos se produce siempre que:

* Coloque un segmento sobre otro en Analysis Workspace. (Se unen automáticamente mediante el *`And`* operador).
* Aplique un solo segmento que contenga el *`And`* operador.
* Aplique un segmento tanto a nivel de proyecto como de tabla.
* Utilice un grupo de informes virtuales con otro segmento.

Por ejemplo, supongamos que apila los siguientes segmentos en la métrica Personas:

* `Campaign = Spring Promotion`
* `Site Section = Product Overview`

Solo se cuenta el número de personas que cumplen los requisitos en ambos segmentos *`using a single device`* . (La métrica Personas no muestra el número de personas que cumplen los requisitos en todos los dispositivos).

Además, en este caso no se recomienda utilizar el *`Or`* operador. Al hacerlo, se produciría un recuento de personas que vieron una u otra, sin contar cuántas personas cumplen los requisitos para ambos segmentos.

Consulte [Generación de segmentos](https://docs.adobe.com/content/help/es-ES/analytics/components/segmentation/segmentation-workflow/seg-build.html) en la ayuda de Segmentación para obtener más información.

## Tipos de dispositivos {#section-8ab378c84ff34574b9c20fecb3848a86}

La métrica Device Co-op y Personas funciona mejor en Adobe Analytics cuando el grupo de informes contiene datos de varios tipos de dispositivos. Por ejemplo, la combinación de datos de aplicaciones y web en el mismo grupo de informes hace que la métrica Personas sea más potente y eficaz. Cuanta más cruce de dispositivos tenga sus datos, la buena posibilidad de que varios visitantes únicos se agrupen como una sola persona.

![](assets/people-device-types.png)

## Experience Cloud ID Service Coverage {#section-bbf0098cac2e467289e7a644a1dea05c}

Device Co-op requiere que las propiedades digitales se instrumenten mediante el servicio de ID de Experience Cloud (MCID). Si los datos de su grupo de informes contienen un número significativo de visitantes sin un MCID, la eficacia de Device Co-op y de la métrica Personas se ve disminuida.

<!--
mcdc-people-metric-apply.xml
-->

En Analysis Workspace, cree un [proyecto](https://docs.adobe.com/content/help/es-ES/analytics/analyze/analysis-workspace/build-workspace-project/t-freeform-project.html)y, a continuación, arrastre la **[!UICONTROL People]** métrica a la tabla del proyecto:

![](assets/people-metric.png)

