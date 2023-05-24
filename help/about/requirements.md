---
description: Su empresa debe cumplir estos estándares mínimos para poder empezar a utilizar la cooperación entre dispositivos de Experience Cloud.
seo-description: Your company must meet these minimum standards before you can start using the Experience Cloud Device Co-op.
seo-title: Membership requirements
title: Requisitos de abono
uuid: 4295fa4e-1b9e-4323-bb79-48e548ca1167
exl-id: 923ce9c5-7716-4c5a-95f2-05a81a05c9cf
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 17%

---

# Requisitos de abono{#membership-requirements}

Su empresa debe cumplir estos estándares mínimos para poder empezar a utilizar la cooperación entre dispositivos de Experience Cloud.

## Requisitos {#section-9cbcee3c7b4e4c49b4c0e2b26aec5fe9}

Hable con su [!DNL Adobe representative to get started]. Adobe se reserva el derecho de negar cualquier membresía potencial de clientes al Experience Cloud Device Co-op si Adobe determina que la participación de un cliente potencial en Device Co-op puede (1) violar cualquier ley aplicable; o (2) causar un riesgo material a la seguridad u operaciones del Adobe o cualquiera de sus clientes.

## requisitos del Experience Cloud {#section-76218a50385d43e6b9323e49f598394a}

Debe estar habilitado para el [!DNL Adobe Experience Cloud] y utilice las siguientes soluciones y servicios para participar en la cooperación.

**Soluciones**

Los solicitantes deben utilizar al menos uno de los siguientes [!DNL Adobe]soluciones:

* [Analytics](http://www.adobe.com/es/marketing-cloud/web-analytics.html)
* [Audience Manager](http://www.adobe.com/es/marketing-cloud/data-management-platform.html)
* [Media Optimizer](http://www.adobe.com/marketing-cloud/online-advertising-management.html)
* [Target](http://www.adobe.com/es/marketing-cloud/testing-targeting.html)

**Servicios principales**

Los solicitantes deben implementar la [Servicio de ID de Experience Cloud](https://docs.adobe.com/content/help/es-ES/id-service/using/home.html).

## Requisitos de biblioteca de códigos de Adobe {#section-931a3fca1ce54afd90b88ba032e75f05}

En la tabla siguiente se enumeran las versiones mínimas de las bibliotecas de código o SDK utilizados por varios [!DNL Experience Cloud] soluciones y servicios. Si utiliza cualquiera de estos códigos y desea participar en Device Co-op, asegúrese de cumplir estos requisitos mínimos.

>[!TIP]
>
>Se recomienda utilizar las versiones de código más recientes, en lugar del mínimo requerido.

**AppMeasurement (Flash)**

Requiere la versión 4.1. Consulte [AppMeasurement para Flash, Flex y AIR](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/data-insertion-api/index.md).

**AppMeasurement (JavaScript)**

Requiere la versión 1.5.4. Consulte [AppMeasurement para Flash, Flex y AIR](https://docs.adobe.com/content/help/es-ES/analytics/implementation/js/migrate-from-hcode.html).

**SDK para móvil**

Requisitos mínimos del SDK móvil:

* Android versión 4.8.3.
* iOS versión 4.8.5.

Su código SDK debe estar habilitado para [!DNL Experience Cloud] Servicio de ID. Habilite y descargue el último código SDK disponible para cada aplicación de su [Adobe Mobile Services](https://mobilemarketing.adobe.com/) cuenta. Consulte [Configurar las opciones del servicio de ID de visitante de SDK](https://docs.adobe.com/content/help/es-ES/mobile-services/using/manage-app-settings-ug/configuring-app/t-config-visitor.html).

Para cada SDK, utilice el correspondiente `visitorSyncIdentifier` método que se adapte a sus necesidades. Consulte:

* [Métodos del servicio de ID del Experience Cloud de Android](https://docs.adobe.com/content/help/en/mobile-services/android/experience-cloud-android/mcvid.html)
* [Métodos de servicio de ID de Experience Cloud de iOS](https://docs.adobe.com/content/help/en/mobile-services/ios/exp-cloud-ios/mcvid.html)

**VisitorAPI.js**

Requiere la versión 1.5.4.

[!DNL Analytics] Los clientes de pueden descargar la biblioteca VisitorAPI.js desde [!DNL Code Manager]. Se encuentra en los archivos JavaScript (nuevo) o JavaScript (heredado). Contacto [Atención al cliente](https://helpx.adobe.com/es/marketing-cloud/contact-support.html) si no tiene acceso a [!DNL Code Manager].

**Biblioteca de destino**

Requiere cualquiera de las siguientes opciones [!DNL Target] Bibliotecas de JavaScript:

* at.js (cualquier versión)
* Versión 58 o posterior de mbox.js
