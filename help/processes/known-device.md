---
description: Acerca de los dispositivos conocidos en Device Graph.
seo-description: Acerca de los dispositivos conocidos en Device Graph.
seo-title: Dispositivos conocidos
title: Dispositivos conocidos
uuid: 53c21105-45b1-4bed-a473-d3ccc4bae965
translation-type: tm+mt
source-git-commit: 4f972a4ae3f0c5ee11b21876bd8a6966cad90371

---


# Known devices{#known-devices}

Acerca de los dispositivos conocidos en Device Graph.

Device Graph opera con el concepto de *`known device`*. Se trata de un dispositivo que un cliente emplea para interactuar con una marca.

>[!NOTE]
>
>En el [!DNL Adobe Experience Cloud Device Co-op], términos como *`device`*, *`person`*, *`identity`* etc. tienen significados específicos. Por ejemplo, &quot;dispositivo&quot; puede referirse a hardware físico, como un teléfono o tableta, y a una aplicación que se ejecuta en dicho hardware. Consulte las definiciones en el [glosario](../glossary.md#glossgroup-0f47d7fbd76c4759801f565f341a386c).

## Supporting goals with the known device {#section-80deae33660e4280ac65c659ceff5601}

El concepto de dispositivo conocido sirve a algunos objetivos esenciales para la creación y mantenimiento de un programa [!DNL Device Co-op] efectivo. Un dispositivo conocido es aquel del que un miembro de [!DNL Device Co-op] tiene conocimiento por medio de alguna interacción con un consumidor (p. ej., por una visita a un sitio web o por el uso de una aplicación móvil). Based on these actions, the [!DNL Device Graph] links the known devices of a [!DNL Device Co-op] member to devices contributed by other [!DNL Device Co-op] members. Estos vínculos pueden ser [determinísticos o probabilísticos](../processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931). This benefits [!DNL Device Co-op] members because they receive:

* Más datos acerca de sus dispositivos conocidos.
* Nueva información acerca de otros dispositivos vinculados.

![](assets/known-device.png)

[!DNL Device Graph] no proporciona información acerca de clústeres de dispositivos de los que un miembro de Device Co-op no tiene conocimiento.

## Device Co-op goals {#section-75aea5a102d54733aae2a7c6ee9ec6c7}

Three main goals animate the [!DNL Device Co-op]. Son:

* **Escala:** compartir el máximo número de posibles vínculos procedentes de distintos casos de uso.
* **Justicia:** asegurar que cada miembro de [!DNL Device Co-op] se beneficia de manera proporcionada a su contribución.

* **Confianza del consumidor:** mantener y fomentar la confianza del consumidor asegurando que su experiencia entre dispositivos involucre marcas que ya conoce y en las que confía.

## Scale and the known device {#section-67f734109762457ca62ec306284ea082}

Los siguientes métodos son las formas más comunes en que un dispositivo se califica como un dispositivo conocido. Dados estos métodos, los miembros de [!DNL Device Co-op] tendrán casi siempre al menos un dispositivo conocido. Esto abunda en el objetivo de proporcionar la máxima escala a todos los miembros de [!DNL Device Co-op].

**Orgánico**

* Visita de un cliente a su sitio web o uso de su aplicación. Es una cualificación con datos de primera mano.
* Captación de clientes mediante un sistema CRM.

**Marketplace**

* Compra de datos de segmentos en Audience Marketplace.
* Compra de datos a un proveedor de datos de terceros.

**Publicidad**

Obtención de inventario en una subasta y servicio de un anuncio al dispositivo. El dispositivo se vuelve conocido si dicho anuncio contiene un píxel de [!DNL Audience Manager].

## Known devices and fairness use cases {#section-0543188729d845d6b95db70b8b25e9f8}

Members of the [!DNL Device Co-op] get links commensurate with their contributions to the [!DNL Device Graph]. Las empresas que contribuyen con muchos dispositivos a [!DNL Device Graph] reciben más vínculos que los miembros que solo aportan unos pocos. Consideramos que esto ayuda a lograr que [!DNL Device Co-op] sea justo para todos sus miembros. Veamos cómo funciona con los casos de uso grande y pequeño siguientes.

**Marca A: caso de uso grande**

En este ejemplo, Marca A tiene 100 visitantes en su sitio web cada mes y comienza una nueva campaña de marca entre dispositivos. For simplicity, assume the [!DNL Device Graph] knows all of the visitors to Brand A are linked to 1 additional device. Esto significa que Marca A podría alcanzar otros 100 dispositivos. Additionally, the [!DNL Device Graph] contains about 200 devices linked together.

<table id="table_78C38DC522F94BC38C1DB73740C058AC"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Dispositivos conocidos/mes </th> 
   <th colname="col2" class="entry"> Dispositivos vinculados recibidos de Device Co-op </th> 
   <th colname="col3" class="entry"> Dispositivos totales para la campaña </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>100 </p> </td> 
   <td colname="col2"> <p>100 </p> </td> 
   <td colname="col3"> <p>200 </p> </td> 
  </tr> 
 </tbody> 
</table>

**Marca B: caso de uso pequeño**

En este ejemplo, Marca B tiene 100 visitantes en su sitio web cada mes y comienza una nueva campaña de marca entre dispositivos. For simplicity, assume the [!DNL Device Graph] knows all of the visitors to Brand B are linked to 50 additional devices. Esto significa que Marca B podría alcanzar 150 dispositivos. Additionally, the [!DNL Device Graph] contains about 1,000 devices linked together.

<table id="table_A6C9CCF9C6564A89BA7060E075A8E73C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Dispositivos conocidos/mes </th> 
   <th colname="col2" class="entry"> Dispositivos vinculados recibidos de Device Co-op </th> 
   <th colname="col3" class="entry"> Dispositivos totales para la campaña </th> 
  </tr>
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p>100 </p> </td> 
   <td colname="col2"> <p>50 </p> </td> 
   <td colname="col3"> <p>150 </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!MORELIKETHIS]
>
>* [Dispositivos desconocidos](../processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40)

