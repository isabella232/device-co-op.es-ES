---
description: Su compañía debe cumplir estos estándares mínimos antes de poder realizar el inicio mediante la cooperación entre dispositivos de Experience Cloud.
seo-description: Su compañía debe cumplir estos estándares mínimos antes de poder realizar el inicio mediante la cooperación entre dispositivos de Experience Cloud.
seo-title: Requisitos de afiliación
title: Requisitos de afiliación
uuid: 4295fa4e-1b9e-4323-bb79-48e548ca1167
translation-type: tm+mt
source-git-commit: 1ab7be570ea63645c6d6065341d31bf170f79715
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 16%

---


# Requisitos de pertenencia{#membership-requirements}

Su compañía debe cumplir estos estándares mínimos antes de poder realizar el inicio mediante la cooperación entre dispositivos de Experience Cloud.

## Requisitos {#section-9cbcee3c7b4e4c49b4c0e2b26aec5fe9}

Hable con su [!DNL Adobe representative to get started]. Adobe se reserva el derecho de denegar a Device Co-op cualquier posible pertenencia de cliente a Experience Cloud si el Adobe determina que la participación de un cliente potencial en Device Co-op puede (1) violar cualquier ley aplicable; o (2) causar un riesgo importante a la seguridad o a las operaciones de Adobe o a cualquiera de sus clientes.

## Requisitos del Experience Cloud {#section-76218a50385d43e6b9323e49f598394a}

Debe estar habilitado para [!DNL Adobe Experience Cloud] y utilizar las siguientes soluciones y servicios para participar en la cooperación.

**Soluciones**

Los solicitantes deben utilizar al menos una de las siguientes [!DNL Adobe]soluciones:

* [Analytics](http://www.adobe.com/es/marketing-cloud/web-analytics.html)
* [Audience Manager](http://www.adobe.com/es/marketing-cloud/data-management-platform.html)
* [Media Optimizer](http://www.adobe.com/marketing-cloud/online-advertising-management.html)
* [Target](http://www.adobe.com/marketing-cloud/testing-targeting.html)

**Servicios principales**

Los solicitantes deben implementar el [servicio de ID de Experience Cloud](https://docs.adobe.com/content/help/es-ES/id-service/using/home.html).

## Requisitos de biblioteca de códigos de Adobe {#section-931a3fca1ce54afd90b88ba032e75f05}

La siguiente tabla lista las versiones mínimas de las bibliotecas de código o los SDK utilizados por diversas soluciones y servicios [!DNL Experience Cloud]. Si utiliza cualquiera de estos códigos y desea participar en Device Co-op, asegúrese de cumplir estos requisitos mínimos.

>[!TIP]
>
>Se recomienda utilizar las versiones de código más recientes en lugar de los mínimos requeridos.

**AppMeasurement (Flash)**

Requiere la versión 4.1. Consulte [AppMeasurement para Flash, Flex y AIR](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/data-insertion-api/index.md).

**AppMeasurement (JavaScript)**

Requiere la versión 1.5.4. Consulte [AppMeasurement para Flash, Flex y AIR](https://docs.adobe.com/content/help/es-ES/analytics/implementation/js/migrate-from-hcode.html).

**SDK para móvil**

Requisitos mínimos del SDK móvil:

* Android versión 4.8.3.
* iOS versión 4.8.5.

El código SDK debe estar habilitado para el servicio de ID [!DNL Experience Cloud]. Habilite y descargue el código SDK más reciente para cada aplicación en su cuenta [Adobe Mobile Services](https://mobilemarketing.adobe.com/). Consulte [Configuración de las opciones del servicio de ID de Visitante del SDK](https://docs.adobe.com/content/help/es-ES/mobile-services/using/manage-app-settings-ug/configuring-app/t-config-visitor.html).

Para cada SDK, utilice el método `visitorSyncIdentifier` apropiado que se ajuste a sus necesidades. Consulte:

* [Métodos del servicio de ID de Experience Cloud de Android](https://docs.adobe.com/content/help/en/mobile-services/android/experience-cloud-android/mcvid.html)
* [Métodos del servicio de ID de Experience Cloud de iOS](https://docs.adobe.com/content/help/en/mobile-services/ios/exp-cloud-ios/mcvid.html)

**VisitorAPI.js**

Requiere la versión 1.5.4.

[!DNL Analytics] los clientes pueden descargar la biblioteca VisitorAPI.js desde  [!DNL Code Manager]. Se encuentra en los archivos JavaScript (nuevo) o JavaScript (heredado). Póngase en contacto con [Servicio de atención al cliente](https://helpx.adobe.com/es/marketing-cloud/contact-support.html) si no tiene acceso a [!DNL Code Manager].

**Biblioteca de destinatarios**

Requiere cualquiera de las siguientes [!DNL Target] bibliotecas de JavaScript:

* at.js (cualquier versión)
* mbox.js versión 58 o posterior

