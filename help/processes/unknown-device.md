---
description: Cuando una persona tiene dispositivos que no se utilizan para interactuar con su marca, esos dispositivos se denominan dispositivos desconocidos.
seo-description: When a person has devices that are not used to interact with your brand, those devices are called unknown devices.
seo-title: Unknown devices
title: Dispositivos desconocidos
uuid: 18e69dad-bdb3-4ac1-a690-374aba1aa0a6
exl-id: 7841bf32-7327-4981-86a2-600e2bfe5901
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Dispositivos desconocidos{#unknown-devices}

Cuando una persona tiene dispositivos que no se utilizan para interactuar con su marca, esos dispositivos se denominan dispositivos desconocidos.

## Categorías de dispositivo desconocidas {#section-014b83fd0f2e4d50aa19dd9fbb46f6ab}

Existen varias formas o categorías en las que un dispositivo puede considerarse &quot;desconocido&quot; para usted. Se incluyen:

* **Visitas de origen a otros miembros de Device Co-op:** Visitas a otros [!DNL Device Co-op] los sitios de los miembros o la publicidad en un dispositivo no hacen, por sí mismos, un dispositivo conocido para su marca.

* **Inventario de anuncios sin rastrear:** El inventario de anuncios que está disponible, pero que aún no se ha publicado ni ingerido, no hace que un dispositivo sea conocido por su marca.
* **Exclusión del consumidor:** Para respetar el deseo del consumidor, los dispositivos que se han excluido no se consideran dispositivos conocidos.

A diferencia de los dispositivos conocidos, los desconocidos no están vinculados a otros dispositivos ni asociados a personas individuales.

## Reglas para establecer el estado conocido/desconocido {#section-fa5c85e59e2d4f88bb79f27f17f02344}

El [!DNL Device Graph] intenta ser lo más inclusivo posible al clasificar dispositivos como conocidos en comparación con desconocidos. Las reglas que ayudan a determinar el estado conocido/desconocido funcionan en orden de prioridad (1 es el más alto) como se muestra a continuación:

* **Regla 1:** ¿El dispositivo está excluido? Si es así, se desconoce el dispositivo.
* **Regla 2:** Es el dispositivo conocido por *cualquiera* método? Si es así, se conoce el dispositivo.

* **Regla 3: ** Si no se aplican las reglas anteriores, se desconoce el dispositivo.

>[!MORELIKETHIS]
>
>* [Dispositivos conocidos](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1)

