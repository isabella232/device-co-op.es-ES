---
description: Cuando una persona tiene dispositivos que no se utilizan para interactuar con su marca, estos se denominan dispositivos desconocidos.
seo-description: Cuando una persona tiene dispositivos que no se utilizan para interactuar con su marca, estos se denominan dispositivos desconocidos.
seo-title: Dispositivos desconocidos
title: Dispositivos desconocidos
uuid: 18e69dad-bdb3-4ac1-a690-374aba1aa0a6
translation-type: tm+mt
source-git-commit: 4f972a4ae3f0c5ee11b21876bd8a6966cad90371
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 0%

---


# Dispositivos desconocidos{#unknown-devices}

Cuando una persona tiene dispositivos que no se utilizan para interactuar con su marca, estos se denominan dispositivos desconocidos.

## Categorías de dispositivos desconocidas {#section-014b83fd0f2e4d50aa19dd9fbb46f6ab}

Existen varias formas o categorías por las que un dispositivo puede considerarse &quot;desconocido&quot; para usted. Se incluyen:

* **Visitas individuales a otros miembros de Device Co-op:** Las visitas a otros [!DNL Device Co-op] sitios miembros o la publicidad en un dispositivo no hacen que un dispositivo sea conocido por su marca.

* **Inventario de anuncios no rastreados:** El inventario de publicidad que está disponible, pero que aún no se ha servido ni ingestado, no hace que un dispositivo sea conocido por su marca.
* **Desactivación del consumidor:** Para respetar el deseo del consumidor, los dispositivos que han sido excluidos no se consideran dispositivos conocidos.

A diferencia de los dispositivos conocidos, los dispositivos desconocidos no están vinculados a otros dispositivos ni asociados a personas individuales.

## Reglas para configurar el estado conocido/desconocido {#section-fa5c85e59e2d4f88bb79f27f17f02344}

El [!DNL Device Graph] intenta ser lo más inclusivo posible al clasificar dispositivos como conocidos en comparación con los desconocidos. Las reglas que ayudan a determinar el estado conocido/desconocido funcionan en orden de prioridad (1 es el más alto) como se muestra a continuación:

* **Artículo 1:** ¿Se ha excluido el dispositivo? Si es así, el dispositivo es desconocido.
* **Artículo 2:** ¿El dispositivo es conocido por *algún* método? Si es así, se conoce el dispositivo.

* **Regla 3: ** Si no se aplican los anteriores, el dispositivo es desconocido.

>[!MORELIKETHIS]
>
>* [Dispositivos conocidos](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1)

