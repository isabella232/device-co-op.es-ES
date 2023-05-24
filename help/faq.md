---
description: Respuestas a preguntas comunes sobre Device Co-op (Identity Services Cooperative y Identity Graph).
title: Preguntas frecuentes sobre Device Co-op
uuid: 490566e1-4d35-468c-8389-678f9ff02cc8
exl-id: 6511e247-76a7-4960-944c-b49fd046fb28
source-git-commit: 399a4fe2d34957eafe8c4eebed465df8770a9239
workflow-type: tm+mt
source-wordcount: '477'
ht-degree: 1%

---

# Preguntas frecuentes{#faq}

Descripciones y respuestas a preguntas comunes sobre Identity Services Cooperative y Identity Graph.

**¿Qué es el [!DNL Device Co-op]?**

Device Co-op es una cooperativa digital para que los clientes de Adobe Experience Cloud participantes trabajen juntos para identificar mejor a sus consumidores en todos los dispositivos.

**¿Qué tecnologías se utilizan en Device Co-op?**

Device Co-op consta de dos tecnologías:

* **Servicio de ID de Experience Cloud:** Este servicio principal de Adobe Experience Cloud proporciona un ID común para identificar a los consumidores de forma coherente en todas las soluciones, canales, experiencias y dispositivos.
* **Cooperación entre dispositivos de Adobe Experience Cloud:** Esta tecnología vincula diferentes dispositivos utilizados por un consumidor o un hogar.

**¿Cómo funciona [!DNL Device Co-op] ¿trabajar?**

A medida que las marcas lanzan su parte del rompecabezas entre dispositivos a través de inicios de sesión anónimos y visitas al sitio, Adobe procesa estos datos para formar clústeres de dispositivos que representan un grupo de dispositivos utilizados por una persona desconocida. Estos clústeres de dispositivos se proporcionan a los miembros de Device Co-op y se utilizan para proporcionar a sus consumidores una experiencia entre dispositivos mejor y más coherente.

**¿Cómo funciona [!DNL Device Co-op] ¿vincular dispositivos?**

Consulte [Vínculos determinísticos y probabilísticos](processes/links.md#concept-58bb7ab25f904f5f98d645e35205c931).

**Qué datos proporcionan los participantes [!DNL Adobe]?**

Consulte [Herramienta de exclusión del consumidor, privacidad y gráfico del dispositivo](privacy.md#concept-fa1346e6b95a484eaeafc9bebe3cd6be).

**Qué datos se comparten entre [!DNL Device Co-op] ¿miembros?**

Consulte [Uso compartido de vínculos en Device Graph](processes/link-sharing.md#concept-7168053105a94649a3f092d375d79eaf).

<!--
Removed at Asa's request.
<p><b>What does <span class="keyword"> Adobe </span> see via the <span class="wintitle"> Device Graph </span>?</b> </p>
<p>Adobe can see which devices are most likely being used by the same person, using probabilistic and deterministic device graph algorithms. This match between a group of devices and a person is really two numbers that are linked to each other. One number represents a group of devices believed to belong to the same person while the other number represents a person. Adobe makes this linked device information available to consumers as well, so they can correct misinformation and/or opt-out one or all devices from the Device Co-op. </p>
-->

**Puede ser [!DNL Device Co-op] ¿el miembro ve vínculos a dispositivos que nunca antes había visto?**

No. Los miembros de Device Co-op solo pueden obtener datos basados en dispositivos que hayan visitado uno de los dominios web de su marca. Consulte [Dispositivos conocidos](processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1) y [Dispositivos desconocidos](processes/unknown-device.md#concept-95090d341cdc4c22ba4319d79d8f6e40).

**¿Debo compartir la información de marketing de mi empresa?**

No. Las marcas solo proporcionan datos anónimos del dispositivo al Adobe.

**Does [!DNL Adobe] usar información de identificación personal (PII) en [!DNL Device Co-op]?**

No. Toda la información de identificación personal tiene un cifrado hash antes de introducirse en cualquier sistema de Adobe, por lo que la información de sus clientes nunca se transfiere a los sistemas de Adobe.

**¿Las marcas más pequeñas que aportan menos datos de dispositivos a Device Co-op obtienen más valor que lo que aportan en comparación con sus homólogas de mayor tamaño?**

No. Todos los miembros de la Cooperativa recuperan valor en relación a lo que ponen. Por ejemplo, si una marca aporta 10 000 dispositivos, podrá recibir información adicional de los dispositivos vinculados asociada con esos 10 000. Si miramos el panorama general, esta contribución puede parecer mínima; pero a medida que más y más marcas de todos los tamaños se unen, la contribución agregada es significativa, y proporcionará el vínculo que falta para muchos dispositivos que muchas otras marcas, tal vez más grandes, están buscando. Consulte [Equidad y dispositivo conocido](processes/known-device.md#section-0543188729d845d6b95db70b8b25e9f8).

**¿Cómo? [!DNL Adobe] administrar direcciones IP si algunos países consideran una dirección IP como información personal.**

Device Co-Op se lanza por primera vez en Estados Unidos y Canadá, donde la dirección IP no se considera información personal. Cuando la Cooperativa se libera en países donde la dirección IP se considera información personal, la dirección IP no se utiliza.
