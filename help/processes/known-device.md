---
description: Acerca de los dispositivos conocidos en Device Graph.
seo-description: Acerca de los dispositivos conocidos en Device Graph.
seo-title: Dispositivos conocidos
title: Dispositivos conocidos
uuid: 53c21105-45b1-4bed-a473-d3ccc4bae965
translation-type: tm+mt
source-git-commit: 4f972a4ae3f0c5ee11b21876bd8a6966cad90371
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 1%

---


# Dispositivos conocidos{#known-devices}

Acerca de los dispositivos conocidos en Device Graph.

En Device Graph, tenemos el concepto de un *`known device`*. Un dispositivo conocido es un dispositivo que un cliente utiliza para interactuar con su marca.

>[!NOTE]
>
>En el [!DNL Adobe Experience Cloud Device Co-op], términos como *`device`*, *`person`*, *`identity`* etc. tienen significados específicos. Por ejemplo, &quot;dispositivo&quot; puede referirse a hardware físico como un teléfono o una tablet y a las aplicaciones que se ejecutan en ese hardware. Consulte las definiciones en el [glosario](../glossary.md#glossgroup-0f47d7fbd76c4759801f565f341a386c) .

## Objetivos de compatibilidad con el dispositivo conocido {#section-80deae33660e4280ac65c659ceff5601}

El concepto de dispositivo conocido admite algunos objetivos esenciales para la creación y el mantenimiento de un [!DNL Device Co-op] programa eficaz. Un dispositivo conocido es aquel del que un [!DNL Device Co-op] miembro conoce por alguna interacción con un consumidor (por ejemplo, una visita al sitio o mediante una aplicación móvil). En función de estas acciones, el [!DNL Device Graph] vincula los dispositivos conocidos de un [!DNL Device Co-op] miembro con los dispositivos que otros [!DNL Device Co-op] miembros han contribuido. Estos vínculos pueden ser [determinísticos o probabilísticos](../processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931). Esto beneficia a [!DNL Device Co-op] los miembros porque reciben:

* Más datos sobre sus dispositivos conocidos.
* Nueva información sobre otros dispositivos vinculados.

![](assets/known-device.png)

El [!DNL Device Graph] no proporcionará información sobre clústeres de dispositivos que un miembro de Device Co-op no haya visto.

## Objetivos de Device Co-op {#section-75aea5a102d54733aae2a7c6ee9ec6c7}

Tres objetivos principales animan el [!DNL Device Co-op]. Se incluyen:

* **Escala:** Comparta el número máximo de vínculos posibles en una variedad de casos de uso.
* **Equidad:** Asegurar que cada miembro de las [!DNL Device Co-op] prestaciones sea proporcional a sus contribuciones.

* **Confianza del consumidor:** Mantener y fomentar la confianza de los consumidores asegurándose de que la experiencia entre dispositivos de los consumidores involucre marcas que ya conocen y en las que confían.

## Escalar y el dispositivo conocido {#section-67f734109762457ca62ec306284ea082}

Los siguientes métodos son las formas más comunes en que un dispositivo se califica como un dispositivo conocido. Dados estos métodos, los miembros casi siempre tendrán al menos un dispositivo conocido. [!DNL Device Co-op] Esto apoya el objetivo de proporcionar la máxima escala a todos los miembros del [!DNL Device Co-op].

**Orgánica**

* Desde la visita de un cliente a su sitio o mediante la aplicación. Se trata de la calificación de datos de origen.
* A través de los clientes incorporados desde un sistema CRM.

**Marketplace**

* Comprar datos de segmentos del Audience Marketplace.
* De la compra de datos a un proveedor de datos de terceros.

**Publicidad**

Ganando el inventario en una subasta y enviando una publicidad a un dispositivo. El dispositivo se convierte en un dispositivo conocido si ese anuncio contiene un [!DNL Audience Manager] píxel.

## Dispositivos conocidos y casos de uso justos {#section-0543188729d845d6b95db70b8b25e9f8}

Los miembros del [!DNL Device Co-op] grupo obtienen vínculos proporcionales a sus contribuciones al [!DNL Device Graph]. Las compañías que contribuyen con muchos dispositivos a la [!DNL Device Graph] recepción reciben más vínculos que los miembros que contribuyen con sólo unos pocos. Creemos que esto ayuda a que todos sus miembros sean [!DNL Device Co-op] justos. Veamos cómo funciona esto con los casos de uso grandes y pequeños que se describen a continuación.

**Marca A: caso de uso grande**

En este ejemplo, Marca A tiene 100 visitantes de sitio al mes y inicio una nueva campaña de marca entre dispositivos. Para simplificar, supongamos que [!DNL Device Graph] sabe que todos los visitantes de la marca A están vinculados a 1 dispositivo adicional. Esto significa que Marca A podría alcanzar otros 100 dispositivos. Además, [!DNL Device Graph] contiene unos 200 dispositivos vinculados entre sí.

<table id="table_78C38DC522F94BC38C1DB73740C058AC"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Dispositivos conocidos/mes </th> 
   <th colname="col2" class="entry"> Dispositivos vinculados recibidos de Device Co-op </th> 
   <th colname="col3" class="entry"> Total de dispositivos para Campaña </th> 
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

**Marca B: Caso de uso pequeño**

En este ejemplo, Marca B tiene 100 visitantes de sitio al mes y inicio una nueva campaña de marca entre dispositivos. Para simplificar, supongamos que [!DNL Device Graph] sabe que todos los visitantes de la Marca B están vinculados a 50 dispositivos adicionales. Esto significa que Marca B podría llegar a 150 dispositivos. Además, [!DNL Device Graph] contiene unos 1000 dispositivos vinculados entre sí.

<table id="table_A6C9CCF9C6564A89BA7060E075A8E73C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> Dispositivos conocidos/mes </th> 
   <th colname="col2" class="entry"> Dispositivos vinculados recibidos de Device Co-op </th> 
   <th colname="col3" class="entry"> Total de dispositivos para Campaña </th> 
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

