---
description: Obtenga información sobre cómo usar datos de Device Co-op en actividades de Adobe Target.
seo-description: Obtenga información sobre cómo usar datos de Device Co-op en actividades de Adobe Target.
seo-title: 'Destinatario: pruebas A/B, pruebas multivariadas y segmentación de experiencias'
title: 'Destinatario: pruebas A/B, pruebas multivariadas y segmentación de experiencias'
uuid: c1b478a4-812e-41ee-913f-29666c5c7ec4
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 0%

---


# Destinatario: pruebas A/B, pruebas multivariadas y segmentación de experiencias{#target-a-b-tests-multivariate-tests-and-experience-targeting}

Obtenga información sobre cómo usar datos de Device Co-op en actividades de Adobe Target.

Puede utilizar datos de Device Co-op en pruebas A/B, pruebas multivariadas (MVT) y actividades de segmentación de experiencias. The Device Co-op option is available during activity creation on the [!DNL Goals & Settings] page in the [!DNL Target] three-step guided workflow.

No se pueden usar datos de Device Co-op en actividades de Automated Personalization, actividades de recomendación o actividades que utilicen [!DNL Adobe Analytics] como origen de sistema de informes (la integración [!DNL Target] y [!DNL Analytics] , conocida como A4T).

>[!NOTE]
>
>Asegúrese de que dispone de la versión requerida de `mbox.js`. Puede utilizar cualquier versión de `at.js`. Para obtener más información, consulte Requisitos [de pertenencia](../about/requirements.md#concept-31d3d165d22546afbedf023d32ad3a43).

## Distribuya contenido relevante independientemente del dispositivo {#section-bba8d41e96914c82a6d267a54f776354}

Los especialistas en marketing desean ofrecer la experiencia más relevante a cada visitante, independientemente del dispositivo que el visitante esté utilizando para interactuar con su compañía o marca.

Los usuarios interactúan con la misma compañía o marca desde diferentes dispositivos: trabaje con portátiles, equipos domésticos, iPad, iPhone, distintos navegadores, etc. Si no puede reconocer que cada dispositivo o navegador específico está siendo utilizado por la misma persona que interactuó anteriormente con su marca en otro dispositivo o navegador, no podrá ofrecer una experiencia coherente y dirigida a esa persona.

Con Device Co-op, los distintos dispositivos de un usuario pueden identificarse como utilizados por el mismo usuario. Cuando ese usuario ve una página con [!DNL Target] actividades, ya sea actividades o contenido de destino [!DNL Target] puede garantizar que el usuario vea la misma experiencia en otro dispositivo.

## Analizar las actividades de Destinatario por personas en lugar de por visitantes {#section-c25cf4f8483942d7836d60756235e62c}

Los especialistas en marketing quieren analizar [!DNL Target] las actividades por &quot;personas&quot; en lugar de por &quot;visitantes&quot;.

Es probable que cada persona interactúe con la misma compañía o marca en todos los dispositivos y navegadores, pero sin Device Co-op, cada dispositivo o navegador individual se considera un &quot;visitante&quot; independiente en [!DNL Target] los informes.

Al ver los informes por dispositivos y exploradores individuales, se infla el recuento de &quot;visitantes&quot; a un número mayor que el número de personas diferentes que interactúan con la compañía o marca. Estas personas suelen realizar una conversión única en estos distintos dispositivos y navegadores, por lo que la tasa de conversión será menor que en la realidad, ya que se contarán más &quot;visitantes&quot; para una sola conversión.

Con Device Co-op, el envío de contenido y el sistema de informes se realizan en el nivel de &quot;personas&quot;, de modo que los informes muestran con precisión cuántas personas distintas vieron la actividad y cuántas de las personas se convirtieron.

Sin Device Co-op, puede determinar que una actividad en particular es la ganadora; sin embargo, como el sistema de informes es más preciso con Device Co-op, otra actividad podría tener una tasa de conversión mayor y, por lo tanto, ser la ganadora.

Para obtener más información sobre este concepto, consulte [Análisis: Métrica](../other-solutions/people.md#concept-8c57cd3904974e078d7fbf84ac9c2d63)Personas.

## Usar datos de Device Co-op por actividad {#section-fb46fae482654023abb1a1e26564db9a}

Los especialistas en marketing pueden elegir utilizar los datos de Device Co-op por actividad. Algunas [!DNL Target] actividades podrían no ser apropiadas para datos de Device Co-op, como:

* Contenido específico adecuado para usuarios en un iPad.

   Los usuarios que inicien la vista de una experiencia en un iPad seguirán viendo esa experiencia en sus equipos domésticos.

* Una oferta de tipo de interés disponible solo para un segmento estricto de visitantes.
* Productos que solo pueden anunciarse en un estado específico (por ejemplo, una póliza de seguro con restricciones de licencia).

Cuando los especialistas en marketing crean audiencias en [!DNL Target], se les alerta si la audiencia no es adecuada para actividades habilitadas para datos de Device Co-op. Las audiencias apropiadas incluyen todos los visitantes, nuevos visitantes y visitantes que regresan.
