---
description: Acerca del uso compartido de vínculos en Device Graph.
seo-description: Acerca del uso compartido de vínculos en Device Graph.
seo-title: Uso compartido de vínculos en Device Graph
title: Uso compartido de vínculos en Device Graph
uuid: 6c7202f0-c6d9-48a4-82ad-ee57d7a518a0
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 0%

---


# Uso compartido de vínculos en Device Graph{#link-sharing-in-the-device-graph}

Acerca del uso compartido de vínculos en Device Graph.

El [!DNL Device Graph] comparte vínculos determinísticos y probabilísticos con diferentes miembros de Adobe Experience Cloud Device Co-op. Compartir vínculos es lo que hace que el [!DNL Device Co-op] vínculo sea tan poderoso. Amplía lo que cada miembro sabe sobre los dispositivos asociados con una persona anónima, pero sólo si ya ha visto al menos uno de los dispositivos de esa persona anónima antes.

## Resumen de Device Graph {#section-7858e9f61b5644c981ffb53626fcc19d}

Antes de comenzar, dediquemos un momento a revisar cómo [!DNL Device Graph] funciona. Los miembros del [!DNL Device Co-op] grupo envían datos al [!DNL Device Graph]. El [!DNL Device Graph] utiliza estos datos para construir la identidad de una persona a partir de vínculos [](../processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931) determinísticos y probabilísticos entre dispositivos. Como [!DNL Device Co-op] participante, estos vínculos proporcionan información sobre la relación entre los usuarios autenticados, otros usuarios y sus dispositivos. Veamos cómo funciona esto en la sección de abajo.

## Ejemplo de uso compartido de vínculos {#section-cb410d827cf14f76bc9b0bd4d31ed767}

En el siguiente ejemplo se muestra el poder de compartir vínculos en Device Co-op. En este ejemplo, tenemos dos compañías ficticias, la Compañía de Noticias y la Compañía de Finanzas. Ambas compañías son miembros del [!DNL Device Co-op]. Persona A es un consumidor que inicia sesión o explora los sitios web de cada compañía desde varios dispositivos.

![](assets/share1.png)

Dado que Persona A se ha autenticado en el sitio de noticias con su teléfono móvil y su tablet, la Compañía de noticias los identifica con un ID de consumidor. Envía esa ID al [!DNL Device Graph] hash criptográfico. La Compañía de Finanzas ya ha visto estos dispositivos antes, pero Persona A no ha iniciado sesión en el sitio. En consecuencia, la Compañía de Finanzas no sabe si estos dispositivos se relacionan entre sí o cómo se asocian con la Persona A.

![](assets/share2.png)

Dado el hash criptográfico del ID de consumidor, el [!DNL Device Graph] reconoce que estos dispositivos están relacionados entre sí y con una persona en particular. Para las compañías que no participan en [!DNL Device Co-op] este sitio, las visitas parecerían provenir de dispositivos distintos y aleatorios. En cualquier caso, una vez que la [!DNL Device Graph] cuenta con la ID con hash, ésta:

* Sabe que el teléfono móvil y el portátil están vinculados.
* Reconoce que la Compañía de Finanzas desea saber si el teléfono móvil y el portátil están vinculados.

Dadas estas condiciones, el [!DNL Device Graph] ahora comparte el enlace que conecta estos dispositivos con la Compañía de Noticias con la Compañía de Finanzas. Durante este proceso, los [!DNL Device Graph] duplicados y comparte el vínculo de un miembro de la cooperación a otro.

![](assets/share3.png)

En este momento, el [!DNL Device Graph] actor cumplió su función correctamente. Tanto la Compañía de Noticias como la Compañía de Finanzas tienen una imagen clara de una identidad. Pueden llegar a Persona A con precisión en todos sus dispositivos.

## Privacidad y uso compartido de vínculos {#section-7b566018b3304420a4b3e4c079826110}

Mantener la privacidad del consumidor y la integridad de los datos para [!DNL Device Co-op] los miembros es crucial a lo largo del proceso de uso compartido de vínculos. Durante este proceso de identificación de clientes y uso compartido de vínculos, [!DNL Device Graph] no:

* Dígale a la Compañía de Finanzas que el enlace vino de la Compañía de Noticias.
* Comparta el ID de cliente utilizado por un [!DNL Device Co-op] miembro con otro.
* Proporcione cualquier información que no sea que el dispositivo móvil y el portátil compartan un vínculo en común.

## Pasos siguientes {#section-ac6e61f1eb6e45b1bb4be8ece39147c7}

Leer la documentación sobre identidad, vinculación y uso compartido de vínculos debería darle una buena idea de cómo [!DNL Device Graph] ensamblan los datos internamente. Como paso siguiente, recomendamos echar un vistazo a nuestra documentación que describe cómo el concepto de un *`known device`* servicio proporciona vínculos entre dispositivos a los miembros de Device Co-op. Consulte Dispositivos [](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1) conocidos y dispositivos [](../processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40)desconocidos.
