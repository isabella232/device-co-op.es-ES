---
description: Obtenga información sobre cómo usar datos de Device Co-op en actividades de Adobe Target.
seo-description: Obtenga información sobre cómo usar datos de Device Co-op en actividades de Adobe Target.
seo-title: 'Target: pruebas A/B, pruebas multivariadas y segmentación de experiencias'
title: 'Target: pruebas A/B, pruebas multivariadas y segmentación de experiencias'
uuid: c1b478a4-812e-41ee-913f-29666c5c7ec4
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031

---


# Target - A/B tests, multivariate tests, and experience targeting{#target-a-b-tests-multivariate-tests-and-experience-targeting}

Obtenga información sobre cómo usar datos de Device Co-op en actividades de Adobe Target.

Puede utilizar datos de Device Co-op en pruebas A/B, pruebas multivariadas (MVT) y actividades de segmentación de experiencias. The Device Co-op option is available during activity creation on the [!DNL Goals & Settings] page in the [!DNL Target] three-step guided workflow.

No puede utilizar datos de Device Co-op en actividades de Personalización automatizada, actividades de Recomendación o actividades que emplean [!DNL Adobe Analytics] como origen de los informes (la integración de [!DNL Target] y [!DNL Analytics], conocida como A4T).

>[!NOTE]
>
>Ensure that you have the required version of `mbox.js`. Puede utilizar cualquier versión de `at.js`. Para obtener más información, consulte Requisitos [de pertenencia](../about/requirements.md#concept-31d3d165d22546afbedf023d32ad3a43).

## Deliver relevant content regardless of the device {#section-bba8d41e96914c82a6d267a54f776354}

Los expertos en marketing buscan ofrecer la experiencia más relevante a cada visitante, no importa qué dispositivo esté utilizando para interactuar con su empresa o marca.

Los usuarios pueden interactuar con una misma empresa o marca desde muchos dispositivos diferentes: portátiles del trabajo, equipos domésticos, iPad, iPhone, distintos navegadores, etc. Si no es capaz de reconocer el uso de cada dispositivo o navegador específico que hace una persona que ya ha interactuado anteriormente con su marca empleando métodos distintos, no podrá ofrecerle una experiencia coherente y dirigida.

Con Device Co-op es posible identificar los distintos dispositivos que utiliza un mismo usuario. Cuando dicho usuario ve una página con actividades de [!DNL Target], ya sean actividades o contenido dirigido, [!DNL Target] puede asegurarse de que tenga la misma experiencia que tendría en otro dispositivo.

## Analyze Target activities by people instead of by visitors {#section-c25cf4f8483942d7836d60756235e62c}

Los expertos en marketing buscan analizar las actividades de [!DNL Target] por “persona”, no por “visitantes”.

Es probable que cada persona esté interactuando con la misma empresa o marca desde varios dispositivos y navegadores, pero, sin Device Co-op, cada dispositivo o navegador individual se considera un “visitante” separado al realizar informes en [!DNL Target].

Al ver informes por dispositivos o navegadores individuales, el recuento  de “visitantes” se infla y arroja un número mayor que el de personas distintas que están interactuando con la empresa o marca. Estas personas suelen convertir una sola vez entre los distintos dispositivos y navegadores, por lo que la tasa de conversión será menor a la real porque se cuentan más “visitantes” para una única conversión.

Con Device Co-op, la entrega de contenido y la realización de informes se realiza en el nivel de la “persona”, de modo que los informes reflejen con precisión cuántas personas distintas han visto la actividad y cuántas de ellas han convertido.

Sin Device Co-op, podría determinar que una actividad particular es la ganadora, pero, como la realización de informes es más precisa con Device Co-op, podría haber en realidad otra actividad con una tasa de conversión mayor que sea la ganadora.

Para obtener más información acerca de este concepto, consulte [Analytics: Métrica](../other-solutions/people.md#concept-8c57cd3904974e078d7fbf84ac9c2d63)Personas.

## Use Device Co-op data per activity {#section-fb46fae482654023abb1a1e26564db9a}

Los expertos en marketing pueden optar por utilizar los datos de Device Co-op por actividad. Determinadas actividades de [!DNL Target] podrían no ser apropiadas para Device Co-op, como:

* Contenido específico apropiado para usuarios de iPad.

   Usuarios que ven primero una experiencia en un iPad y la continúan en su equipo doméstico.

* Una oferta de tipo de interés disponible solo para un segmento estricto de visitantes.
* Productos que solo tienen permiso para anunciarse en un estado concreto (por ejemplo, una póliza de seguro con restricciones de licencia).

Cuando los expertos en marketing crean audiencias en [!DNL Target], se les alerta si la audiencia no es apropiada para actividades con datos de Device Co-op. Las audiencias apropiadas incluyen a todos los visitantes, a los nuevos y a los que regresan.
