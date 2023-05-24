---
description: Aprenda a utilizar los datos de Device Co-op en las actividades de Adobe Target.
seo-description: Learn how to use Device Co-op data in Adobe Target activities.
seo-title: Target - A/B tests, multivariate tests, and experience targeting
title: 'Target: pruebas A/B, pruebas multivariable y segmentación de experiencias'
uuid: c1b478a4-812e-41ee-913f-29666c5c7ec4
exl-id: 6e630adf-faff-4fe4-b560-febd59964a5f
source-git-commit: 573744525fcc00f35540af9ffec46530111940ed
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 0%

---

# Target: pruebas A/B, pruebas multivariable y segmentación de experiencias{#target-a-b-tests-multivariate-tests-and-experience-targeting}

Aprenda a utilizar los datos de Device Co-op en las actividades de Adobe Target.

Puede utilizar datos de Device Co-op en pruebas A/B, pruebas multivariable (MVT) y actividades de segmentación de experiencias. La opción Device Co-op está disponible durante la creación de actividades en [!DNL Goals & Settings] página en la [!DNL Target] flujo de trabajo guiado de tres pasos.

Los datos de Device Co-op no se pueden usar en actividades de Automated Personalization, actividades de Recommendations ni actividades que utilicen [!DNL Adobe Analytics] como fuente de informes (la variable [!DNL Target] y [!DNL Analytics] integración de, conocida como A4T).

>[!NOTE]
>
>Asegúrese de que tiene la versión requerida de `mbox.js`. Puede utilizar cualquier versión de `at.js`. Para obtener más información, consulte [Requisitos de abono](../about/requirements.md#concept-31d3d165d22546afbedf023d32ad3a43).

## Ofrecer contenido relevante independientemente del dispositivo {#section-bba8d41e96914c82a6d267a54f776354}

Los especialistas en marketing desean ofrecer la experiencia más relevante a cada visitante, independientemente del dispositivo que utilice actualmente el visitante para interactuar con su compañía o marca.

Los usuarios interactúan con la misma compañía o marca desde muchos dispositivos diferentes: portátiles de trabajo, equipos domésticos, iPads, iPhone, varios exploradores, etc. Si no puede reconocer que la misma persona que ha interactuado anteriormente con su marca en otro dispositivo o explorador está utilizando cada dispositivo o explorador específico, no puede ofrecer una experiencia coherente y segmentada a esa persona.

Con la cooperación entre dispositivos, se puede identificar que los distintos dispositivos de un usuario los utiliza el mismo usuario. Cuando ese usuario ve una página con [!DNL Target] actividades (actividades o contenido de destino) [!DNL Target] puede garantizar que el usuario vea la misma experiencia en otro dispositivo.

## Analizar actividades de Target por personas en lugar de por visitantes {#section-c25cf4f8483942d7836d60756235e62c}

Los especialistas en marketing desean analizar [!DNL Target] actividades por &quot;personas&quot; en lugar de &quot;visitantes&quot;.

Es probable que cada persona interactúe con la misma compañía o marca en distintos dispositivos y exploradores, pero sin Device Co-op, cada dispositivo o explorador individual se considera un &quot;visitante&quot; independiente en [!DNL Target] informes.

Ver informes por dispositivos y exploradores individuales infla el recuento de &quot;visitantes&quot; a un número mayor que el número de personas diferentes que interactúan con la compañía o marca. Por lo general, estas personas solo convierten una vez en estos dispositivos y navegadores, por lo que la tasa de conversión será menor que en la realidad, ya que se contará a más &quot;visitantes&quot; para una sola conversión.

Con Device Co-op, la entrega de contenido y la creación de informes se realizan en el nivel de &quot;personas&quot;, por lo que los informes muestran con precisión cuántas personas diferentes vieron la actividad y cuántas personas se convirtieron.

Sin los datos de Device Co-op, podría determinar que una actividad en particular es la ganadora; sin embargo, como los informes son más precisos con Device Co-op, otra actividad podría tener una tasa de conversión más alta y, por lo tanto, ser la ganadora.

Para obtener más información sobre este concepto, consulte [Analytics: Métrica Personas](../other-solutions/people.md#concept-8c57cd3904974e078d7fbf84ac9c2d63).

## Uso de datos de Device Co-op por actividad {#section-fb46fae482654023abb1a1e26564db9a}

Los especialistas en marketing pueden elegir utilizar los datos de Device Co-op por actividad. Cierto [!DNL Target] Es posible que las actividades de no sean apropiadas para los datos de Device Co-op, como:

* Contenido específico apropiado para los usuarios de un iPad.

   Los usuarios que vean por primera vez una experiencia en un iPad, seguirán viendo esa experiencia en sus equipos domésticos.

* Una oferta de tasa de interés disponible solo para un segmento estricto de visitantes.
* Los productos pueden anunciarse solo en un estado específico (por ejemplo, una póliza de seguro con restricciones de licencia).

Cuando los especialistas en marketing crean audiencias en [!DNL Target]Sin embargo, se les alerta si la audiencia no es adecuada para las actividades habilitadas para datos de Device Co-op. Las audiencias apropiadas incluyen todos los visitantes, los nuevos visitantes y los visitantes que regresan.
