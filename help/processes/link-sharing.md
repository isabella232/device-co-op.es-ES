---
description: Acerca del uso compartido de vínculos en Device Graph.
seo-description: About link sharing in the Device Graph.
seo-title: Link sharing in the Device Graph
title: Uso compartido de vínculos en Device Graph
uuid: 6c7202f0-c6d9-48a4-82ad-ee57d7a518a0
exl-id: 91ecc493-89d8-40d6-a98b-c2349e25c854
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Uso compartido de vínculos en Device Graph{#link-sharing-in-the-device-graph}

Acerca del uso compartido de vínculos en Device Graph.

El [!DNL Device Graph] comparte vínculos determinísticos y probabilísticos con diferentes miembros de Adobe Experience Cloud Device Co-op. Compartir vínculos es lo que hace que [!DNL Device Co-op] tan poderoso. Amplía lo que cada miembro conoce sobre los dispositivos asociados con una persona anónima, pero solo si ha visto al menos uno de los dispositivos de esa persona anónima anteriormente.

## Resumen de Device Graph {#section-7858e9f61b5644c981ffb53626fcc19d}

Antes de empezar, vamos a dedicar un momento a revisar cómo se utilizan las [!DNL Device Graph] funciona. Miembros de la [!DNL Device Co-op] enviar datos a [!DNL Device Graph]. El [!DNL Device Graph] utiliza estos datos para construir la identidad de una persona a partir de [vínculos determinísticos y probabilísticos](../processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931) entre dispositivos. As a [!DNL Device Co-op] participante, estos vínculos proporcionan información sobre la relación entre los usuarios autenticados, otros usuarios y sus dispositivos. Veamos cómo funciona esto en la sección que aparece a continuación.

## Ejemplo de uso compartido de vínculos {#section-cb410d827cf14f76bc9b0bd4d31ed767}

El siguiente ejemplo muestra el poder del uso compartido de vínculos en Device Co-op. En este ejemplo, tenemos 2 compañías ficticias, la Empresa de noticias y la Empresa financiera. Ambas empresas son miembros de la [!DNL Device Co-op]. La persona A es un consumidor que inicia sesión o explora los sitios web de cada empresa desde varios dispositivos.

![](assets/share1.png)

Debido a que la persona A se ha autenticado en el sitio de noticias con su teléfono móvil y tableta, la compañía de noticias los identifica con un ID de consumidor. Envía ese ID a la [!DNL Device Graph] como hash criptográfico. La empresa de finanzas ya ha visto estos dispositivos anteriormente, pero la persona A no ha iniciado sesión en el sitio. En consecuencia, la Empresa Financiera no sabe si estos dispositivos se relacionan entre sí o cómo se asocian con la Persona A.

![](assets/share2.png)

Dado el hash criptográfico del ID de consumidor, la variable [!DNL Device Graph] reconoce que estos dispositivos están relacionados entre sí y con una persona en particular. A las empresas que no participan en el [!DNL Device Co-op] estas visitas al sitio parecerían provenir de dispositivos independientes y aleatorios. En cualquier caso, una vez que [!DNL Device Graph] tiene el ID con hash:

* Sabe que el teléfono móvil y el portátil están vinculados.
* Reconoce que la Empresa Financiera desea saber si el teléfono móvil y el portátil están vinculados.

Dadas estas condiciones, la variable [!DNL Device Graph] ahora comparte el enlace que conecta estos dispositivos para la Empresa de Noticias con la Empresa Financiera. Durante este proceso, la variable [!DNL Device Graph] duplica y comparte el vínculo de un miembro de la cooperación a otro.

![](assets/share3.png)

En este punto, la variable [!DNL Device Graph] ha desempeñado su función correctamente. Tanto la Empresa de Noticias como la Empresa Financiera tienen una imagen clara de una identidad. Pueden llegar a la persona A de forma precisa en todos sus dispositivos.

## Privacidad y uso compartido de vínculos {#section-7b566018b3304420a4b3e4c079826110}

Mantener la privacidad del consumidor y la integridad de los datos para [!DNL Device Co-op] Los miembros de son cruciales en todo el proceso de uso compartido de vínculos. Durante este proceso de identificación del cliente y uso compartido de vínculos, la variable [!DNL Device Graph] no lo hizo:

* Dígale a la compañía de finanzas que el enlace vino de la compañía de noticias.
* Compartir el ID de cliente utilizado por uno [!DNL Device Co-op] miembro con otro.
* Proporcione cualquier información distinta de la que comparten el dispositivo móvil y el equipo portátil.

## Pasos siguientes {#section-ac6e61f1eb6e45b1bb4be8ece39147c7}

Leer la documentación sobre identidad, vinculación y uso compartido de vínculos debería darle una buena idea de cómo funciona el [!DNL Device Graph] ensambla los datos internamente. Como siguiente paso, recomendamos echar un vistazo a nuestra documentación que describe cómo funciona el concepto de *`known device`* ofrece vínculos entre dispositivos a los miembros de Device Co-op. Consulte [Dispositivos conocidos](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1) y [Dispositivos desconocidos](../processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40).
