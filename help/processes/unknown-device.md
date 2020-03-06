---
description: Si una persona tiene dispositivos que no emplea para interactuar con dicha marca, se los denomina dispositivos desconocidos.
seo-description: Si una persona tiene dispositivos que no emplea para interactuar con dicha marca, se los denomina dispositivos desconocidos.
seo-title: Dispositivos desconocidos
title: Dispositivos desconocidos
uuid: 18e69dad-bdb3-4ac1-a690-374aba1aa0a6
translation-type: tm+mt
source-git-commit: 4f972a4ae3f0c5ee11b21876bd8a6966cad90371

---


# Unknown devices{#unknown-devices}

Si una persona tiene dispositivos que no emplea para interactuar con dicha marca, se los denomina dispositivos desconocidos.

## Unknown device categories {#section-014b83fd0f2e4d50aa19dd9fbb46f6ab}

Hay varios motivos (o categorías) por los que un dispositivo puede considerarse &quot;desconocido&quot; para usted. Son:

* **Visitas personales a otros miembros de :** las visitas a sitios de otros miembros de [!DNL Device Co-op]Device Co-op o sus anuncios en un dispositivo no bastan por sí mismos para que un dispositivo pase a ser conocido por su marca.

* **Inventario de anuncios no rastreados:** un inventario de anuncios que está disponible pero aún no se ha servido o introducido no basta para que un dispositivo sea conocido por su marca.
* **Exclusión de consumidor:** para respetar los deseos del consumidor, los dispositivos que han sido excluidos no se consideran dispositivos conocidos.

Al contrario que los dispositivos conocidos, los desconocidos no están vinculados a otros ni se asocian a una persona concreta.

## Rules for setting known/unknown status {#section-fa5c85e59e2d4f88bb79f27f17f02344}

[!DNL Device Graph] trata de ser lo más incluyente posible al clasificar los dispositivos como conocidos. Las reglas que ayudan a determinar el estado conocido/desconocido operan por orden de prioridad (1 es la máxima prioridad), como se muestra abajo:

* **Regla 1:** ¿el dispositivo ha sido excluido por el usuario? Si es así, el dispositivo es desconocido.
* **Regla 2:** ¿el dispositivo es conocido por *cualquier* otro método? Si es así, el dispositivo es conocido.

* **Regla 3: ** Si no se aplican los anteriores, el dispositivo es desconocido.

>[!MORELIKETHIS]
>
>* [Dispositivos conocidos](../processes/known-device.md#concept-8e87c276819a48bfac5cef10b45216d1)

