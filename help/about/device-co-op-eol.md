---
keywords: adobe experience cloud;Adobe Experience Cloud;cooperación entre dispositivos;cooperación entre dispositivos;fin de vida útil
title: Preguntas frecuentes sobre el fin de vida útil de Device Co-op
description: Obtenga información sobre los planes de fin de vida útil para Device Co-op.
exl-id: 015ba95c-0c8d-415e-969c-b8670494de98
source-git-commit: c19e8425d5d6c2498186c19929907d2ee5327b31
workflow-type: tm+mt
source-wordcount: '1017'
ht-degree: 2%

---

# Preguntas frecuentes sobre el fin de vida útil de Device Co-op

Este documento proporciona respuestas a las preguntas más frecuentes sobre el plan de fin de vida útil (EOL) de Adobe Experience Cloud Device Co-op. Cuando este plan entre en vigor, Adobe proporcionará un aviso avanzado en las [notas de la versión del Experience Cloud](https://experienceleague.adobe.com/docs/release-notes/experience-cloud/current.html?lang=es) y en [Priority Product Update](https://www.adobe.com/subscription/priority-product-update.html).

## Preguntas frecuentes

La siguiente es una lista de respuestas a las preguntas más frecuentes sobre el plan [!DNL Device Co-op] EOL.

## ¿Por qué [!DNL Device Co-op] está en desuso?

Se espera que los próximos cambios en el entorno AdTech resulten en [!DNL Device Co-op] convertirse en una solución obsoleta en los próximos años. [!DNL Device Co-op] se compone principalmente de cookies de terceros y el  [!DNL Google's] anuncio de que bloquearán cookies de terceros a más tardar  [!DNL Google Chrome] en 2022 disminuirá la eficacia de  [!DNL Device Co-op]. [!DNL Chrome] tiene ~65% de la cuota de mercado del explorador y otros exploradores principales ya han implementado el bloqueo de cookies de terceros. Una vez que [!DNL Chrome] bloquee las cookies de terceros, la mayoría de las cookies de terceros se bloquearán y [!DNL Device Co-op] se volverá obsoleta.

## ¿Por qué el Adobe termina los [!DNL Device Co-op] registros ahora?

Los registros finalizan para evitar riesgos de no satisfacer las expectativas de los clientes debido a los próximos cambios en el sector relacionados con las cookies de terceros. [!DNL Device Co-op] tardan unos meses en prepararse y otros pocos meses en extraer valor del servicio. Cualquier nueva suscripción en este punto podría provocar que las marcas no experimenten el valor completo de [!DNL Device Co-op].

## ¿Pueden registrarse nuevos clientes?

A partir del 11 de junio de 2021, Adobe dejará de aceptar nuevos registros a [!DNL Device Co-op].

## ¿Se están renovando los contratos existentes?

A partir del 11 de junio de 2021, Adobe dejará de renovar los [!DNL Device Co-op] contratos. Si desea seguir utilizando los servicios [!DNL Device Co-op], puede seguir haciéndolo en los términos de licencia actuales hasta que termine el programa.

## ¿Cuál es la fecha exacta de finalización del programa [!DNL Device Co-op]?

El programa [!DNL Device Co-op] finalizará en 2022. El tiempo y la fecha específicos dependen de cuándo [!DNL Google] comienza a bloquear las cookies de terceros.

## ¿Qué aplicaciones se verán afectadas por el fin de vida útil de Device Co-op?

Las siguientes aplicaciones se verán afectadas por los procedimientos de fin de vida útil [!DNL Device Co-op]:

- [Adobe Analytics](https://experienceleague.adobe.com/docs/analytics.html?lang=en)
- [Adobe Audience Manager](https://experienceleague.adobe.com/docs/audience-manager/user-guide/overview/aam-overview.html?lang=en)
- [Adobe Advertising Cloud](https://experienceleague.adobe.com/docs/advertising-cloud.html?lang=en)
- [Adobe Target](https://experienceleague.adobe.com/docs/target/using/introduction/intro.html?lang=en)

## ¿Qué opciones tengo como alternativas a [!DNL Device Co-op]?

### [!DNL Analytics]

Puede utilizar la función [!DNL Analytics] [Análisis entre dispositivos (CDA)](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html) ya que admite el servicio de identidad de Adobe Experience Platform [Private Graph](https://experienceleague.adobe.com/docs/analytics/components/cda/device-graph.html?lang=en) y la [Configuración basada en el campo](https://experienceleague.adobe.com/docs/analytics/components/cda/field-based-stitching.html?lang=en).

### [!DNL Audience Manager]

[!DNL Audience Manager] mantiene integraciones con socios de gráficos de dispositivos de terceros, incluidos  [!DNL LiveRamp] y  [!DNL Tapad], aunque debe establecer relaciones comerciales directamente con socios de gráficos para aprovechar  [!DNL Audience Manager].

### [!DNL Real-time Customer Data Platform]

No hay planes para modificar el [!DNL Audience Manager Data Management Platform] actual (DMP). Sin embargo, la desaprobación de cookies de terceros probablemente creará desafíos de escala para la mayoría de los usuarios de DMP. Para ayudar a los clientes a desarrollar sus prácticas de administración de datos, el Adobe está fomentando la reducción de la dependencia en los identificadores que enfrentarán restricciones el año próximo. Los equipos de marketing deben crear estrategias de datos de origen centradas en identificadores duraderos que incluyan información de identificación personal (PII), que se pueda resolver con [!DNL Real-time Customer Data Platform] (CDP en tiempo real).

[!DNL Real-time CDP] reduce las dependencias con cookies de terceros y los ID de dispositivo al expandir el conjunto de identificadores disponibles para la creación de audiencias para incluir PII. La base de [!DNL Real-time CDP] es el Perfil del cliente en tiempo real, que reúne los datos de atributos de las personas con los datos de comportamiento en tiempo real y permite a los especialistas en marketing crear segmentos de audiencia enriquecidos con controles patentados de control de datos. Al igual que [!DNL Audience Manager], [!DNL Real-time CDP] potencia los casos de uso de perspectivas y personalización, pero también genera perspectivas de nivel personal más detalladas y puede activar audiencias en una amplia gama de destinos que abarque tecnologías publicitarias y tecnologías de marketing, incluidos medios de pago, medios sociales, correo electrónico y sistemas de clientes.

[!DNL Real-time CDP] también incluirá el acceso a  [Adobe Experience Platform Segment Match (Alpha)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match.html?lang=en), que permite a las marcas expandir sus propios conjuntos de datos de origen mediante asociaciones y lograr perspectivas y personalización mejoradas.

### [!DNL Target]

Actualmente no hay alternativas disponibles para [!DNL Target] porque [!DNL Target] proporciona una función determinística de vinculación de identidad entre dispositivos conocida como `mbox3rdPartyId`, que funciona de manera similar al ID de cliente de Adobe. Esta capacidad permite a los clientes [!DNL Target] combinar perfiles y participación de actividad en pruebas [!DNL Target] y personalización que se está realizando en canales entrantes.

### Adobe Advertising Cloud

[!DNL Advertising Cloud] los clientes de ya no podrán usar  [!DNL Device Co-op] para la segmentación y medición de audiencias entre dispositivos. Con [!DNL Advertising Cloud], aún podrá aprovechar la asociación [!DNL Device Graph] del Adobe con [!DNL LiveRamp] para seguir realizando estas funciones en la medida de la capacidad y escala [!DNL LiveRamp’s]. Debe permitir que las campañas que utilicen [!DNL Device Co-op] terminen y, a continuación, cambiar al proveedor de gráficos de dispositivos [!DNL LiveRamp] o dejar de aprovechar la segmentación basada en personas.

## ¿Qué capacidades e implementaciones existentes pueden ayudar a prepararme para un futuro sin cookies?

La implementación del servicio de ID de visitante existente potencia Analytics [CDA](https://experienceleague.adobe.com/docs/analytics/components/cda/overview.html). Si el ID declarado existente es un correo electrónico con hash, se puede utilizar para activar las siguientes capacidades:

- [!DNL Audience Manager] [People-Based Destinations](https://experienceleague.adobe.com/docs/audience-manager/user-guide/features/destinations/people-based/people-based-destinations-overview.html).
- [Coincidencia de segmento del Experience Platform (Alpha)](https://experienceleague.adobe.com/docs/experience-platform/segmentation/ui/segment-match.html?lang=en).

## ¿Conseguiré mantener los datos de [!DNL Device Co-op]?

Para los usuarios de [!DNL Audience Manager] y [!DNL Advertising Cloud] , los datos de [!DNL Device Co-op] no estarán disponibles para su transferencia a gráficos de terceros. [!DNL Device Co-op] los datos solo se migrarán para los  [!DNL Analytics Ultimate] usuarios que utilicen CDA y  [!DNL Device Co-op] cambien a la configuración basada en el campo. No se migrarán los datos de todas las demás soluciones.

## ¿Es obligatorio adoptar otras características?

Aunque la adopción de otras funciones de Adobe no es obligatoria, debe comenzar la implementación de otras funciones lo antes posible para permitir tiempo y una coordinación adecuada antes de la [!DNL Device Co-op] desaprobación.

## ¿Cuándo tengo que adoptar soluciones alternativas si opto por ello?

La adopción de otras funciones no es obligatoria. Solo se recomienda si desea seguir ocupándose de los casos de uso que fueron abordados por [!DNL Device Co-op]. Si decide adoptar otras funciones, debe hacerlo antes de 2022 (fecha exacta por anunciar) antes de que finalice el programa [!DNL Device Co-op].

## ¿Cuánto tardará la adopción?

Esto dependerá de la función . Por ejemplo, si un cliente de Analytics Ultimate que utiliza Análisis entre dispositivos con [!DNL Device Co-op] necesita migrar a Gráfico de dispositivos privados en tiempo real o a Configuración basada en campo, la adopción tardará algún tiempo.
