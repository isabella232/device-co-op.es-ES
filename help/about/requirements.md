---
description: Su compañía debe cumplir estos estándares mínimos para poder realizar el inicio mediante la cooperación entre dispositivos de Experience Cloud.
seo-description: Su compañía debe cumplir estos estándares mínimos para poder realizar el inicio mediante la cooperación entre dispositivos de Experience Cloud.
seo-title: Requisitos de afiliación
title: Requisitos de afiliación
uuid: 4295fa4e-1b9e-4323-bb79-48e548ca1167
translation-type: tm+mt
source-git-commit: 822882d4f9bb9eed7cf116597b62d07bbe94376c

---


# Requisitos de afiliación{#membership-requirements}

Su compañía debe cumplir estos estándares mínimos para poder realizar el inicio mediante la cooperación entre dispositivos de Experience Cloud.

## Requisitos {#section-9cbcee3c7b4e4c49b4c0e2b26aec5fe9}

Habla con tu [!DNL Adobe representative to get started]. Si no tiene un representante de Adobe, visite el portal [de membresía de](http://landing.adobe.com/en/na/events/summit/275658-summit-co-op.html) Device Co-op y complete el formulario en línea.

Adobe se reserva el derecho de denegar la pertenencia de cualquier cliente potencial a la cooperación entre dispositivos de Experience Cloud si Adobe determina que la participación de un cliente potencial en Device Co-op puede (1) infringir cualquier ley aplicable; o (2) causar un riesgo importante para la seguridad o las operaciones de Adobe o de cualquiera de sus clientes.

## Requisitos de Experience Cloud {#section-76218a50385d43e6b9323e49f598394a}

Debe estar habilitado para la cooperación [!DNL Adobe Experience Cloud] y utilizar las siguientes soluciones y servicios para participar en ella.

**Soluciones**

Los solicitantes deben utilizar al menos una de las siguientes [!DNL Adobe]soluciones:

* [Analytics](http://www.adobe.com/es/marketing-cloud/web-analytics.html)
* [Audience Manager](http://www.adobe.com/es/marketing-cloud/data-management-platform.html)
* [Media Optimizer](http://www.adobe.com/marketing-cloud/online-advertising-management.html)
* [Target](http://www.adobe.com/es/marketing-cloud/testing-targeting.html)

**Servicios principales**

Los solicitantes deben implementar el servicio [de ID de](https://docs.adobe.com/content/help/es-ES/id-service/using/home.html)Experience Cloud.

## Requisitos de la biblioteca de códigos de Adobe {#section-931a3fca1ce54afd90b88ba032e75f05}

La siguiente tabla lista las versiones mínimas de las bibliotecas de código o los SDK utilizados por varias [!DNL Experience Cloud] soluciones y servicios. Si utiliza cualquiera de estos códigos y desea participar en Device Co-op, asegúrese de cumplir estos requisitos mínimos.

>[!TIP]
>
>Se recomienda utilizar las versiones de código más recientes en lugar de los mínimos requeridos.

**AppMeasurement (Flash)**

Requiere la versión 4.1. Consulte [AppMeasurement para Flash, Flex y AIR](https://github.com/AdobeDocs/analytics-1.4-apis/blob/master/docs/data-insertion-api/index.md).

**AppMeasurement (JavaScript)**

Requiere la versión 1.5.4. Consulte [AppMeasurement para Flash, Flex y AIR](https://docs.adobe.com/content/help/en/analytics/implementation/js/migrate-from-hcode.html).

**SDK para móvil**

Requisitos mínimos del SDK móvil:

* Android versión 4.8.3.
* iOS versión 4.8.5.

Your SDK code must be enabled for the [!DNL Experience Cloud] ID service. Enable and download the latest SDK code for each app in your [Adobe Mobile Services](https://mobilemarketing.adobe.com/) account. See [Configure SDK Visitor ID Service Options](https://docs.adobe.com/content/help/en/mobile-services/using/manage-app-settings-ug/configuring-app/t-config-visitor.html).

Para cada SDK, utilice el `visitorSyncIdentifier` método adecuado que se adapte a sus necesidades. Consulte:

* [Métodos del servicio de ID de Android Experience Cloud](https://docs.adobe.com/content/help/en/mobile-services/android/experience-cloud-android/mcvid.html)
* [Métodos del servicio de ID de iOS Experience Cloud](https://docs.adobe.com/content/help/en/mobile-services/ios/exp-cloud-ios/mcvid.html)

**VisitorAPI.js**

Requiere la versión 1.5.4.

[!DNL Analytics] los clientes pueden descargar la biblioteca VisitorAPI.js desde [!DNL Code Manager]. Se encuentra en los archivos JavaScript (nuevo) o JavaScript (heredado). Póngase en contacto con [el Servicio de atención](https://helpx.adobe.com/es/marketing-cloud/contact-support.html) al cliente si no tiene acceso a [!DNL Code Manager].

**Biblioteca de Destinatarios**

Requiere cualquiera de las siguientes bibliotecas [!DNL Target] JavaScript:

* at.js (cualquier versión)
* mbox.js versión 58 o posterior

