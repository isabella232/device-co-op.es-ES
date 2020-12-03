---
description: Cómo Device Graph analiza los datos determinísticos y probabilísticos para crear un mapa que vincule los dispositivos.
seo-description: Cómo Device Graph analiza los datos determinísticos y probabilísticos para crear un mapa que vincule los dispositivos.
seo-title: Vínculos determinísticos y probabilísticos
title: Vínculos determinísticos y probabilísticos
uuid: 00693a0a-f73d-460d-84a4-b7c745b9fe0a
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031
workflow-type: tm+mt
source-wordcount: '866'
ht-degree: 0%

---


# Vínculos determinísticos y probabilísticos{#deterministic-and-probabilistic-links}

Cómo Device Graph analiza los datos determinísticos y probabilísticos para crear un mapa que vincule los dispositivos.

En el [!DNL Device Graph], los procesos internos crean una jerarquía de identidad que asigna dispositivos y los conecta a personas individuales y anónimas. El resultado del gráfico incluye vínculos entre dispositivos que se pueden utilizar para direccionar junto con datos expuestos en soluciones de Experience Cloud seleccionadas. Las soluciones de Adobe que funcionan con [!DNL Device Graph] datos incluyen Analytics, Audience Manager, Media Optimizer y Destinatario.

El [!DNL Device Graph] analiza datos determinísticos y probabilísticos para crear un mapa que vincule dispositivos. Los datos determinísticos vinculan los dispositivos en función de la información de inicio de sesión con hash. Los datos probabilísticos vinculan los dispositivos en función de información como direcciones IP y otros metadatos. El [!DNL Device Graph] asocia los clústeres de dispositivos vinculados a una persona individual anónima Estas conexiones permiten que los especialistas en marketing digital lleguen a personas en lugar de a dispositivos. En la [!DNL Device Graph], el propietario de un dispositivo es la representación anónima de una persona real. Los vínculos determinísticos y probabilísticos ayudan a crear una estructura de identidad de usuario.

>[!NOTE]
>
>En Adobe Experience Cloud Device Co-op, términos como *dispositivo*, *persona* e *identidad* tienen significados específicos. Por ejemplo, el *dispositivo* puede hacer referencia a hardware físico como un teléfono o una tableta y a las aplicaciones que se ejecutan en ese hardware. Consulte las definiciones en el [glosario](../glossary.md#glossgroup-0f47d7fbd76c4759801f565f341a386c) .

## ¿Qué son los vínculos? {#section-2df4c6f01eba49369993146df0661f13}

Cuando hablamos de vínculos, es importante tener en cuenta cuáles son realmente en el contexto de Device Graph [!DNL Experience Cloud] . En este contexto, los vínculos no son conexiones físicas entre dispositivos. En su lugar, un vínculo es cómo Device Graph asocia distintos dispositivos a la misma persona desconocida. Por ejemplo, supongamos que tenemos un teléfono móvil y un navegador de escritorio. El teléfono y el navegador se pueden considerar &quot;vinculados&quot; una vez que Device Graph determina que ambos dispositivos son utilizados por la misma persona desconocida. Como leerá a continuación, Device Graph crea identidades con vínculos determinísticos y probabilísticos. Y, en Device Graph, el propietario de un dispositivo es la representación anónima de una persona real.

## Vínculos determinísticos {#section-33d41e828a674b398e36fe63da20ac09}

Los vínculos determinísticos asocian un dispositivo a una persona en función de un evento de autenticación (por ejemplo, una acción de inicio de sesión en un sitio desde un dispositivo). Esta acción crea un identificador anónimo conocido como ID de consumidor. Veamos cómo funciona la vinculación determinística. En este ejemplo, Persona A inicia sesión en un sitio de noticias a través de una aplicación en su dispositivo móvil. Más tarde ese mismo día, Persona A volverá a iniciar sesión, pero esta vez a través de un navegador en su portátil.

![](assets/link1.png)

En función de la información de inicio de sesión, Device Graph:

* Sabe que Persona A se ha autenticado en el sitio de noticias con una combinación de teléfono móvil/aplicación y dispositivo portátil/navegador.
* Vincula estos dispositivos a Persona A.
* Crea una identidad basada en dispositivos vinculados asociados a una persona anónima.

![](assets/link2.png)

>[!NOTE]
>
>Ni el [!DNL Adobe Experience Cloud Device Co-op] ni el [!DNL Device Graph] recibe información de autenticación real o información personal identificable (PII) en estos datos. Los miembros del [!DNL Experience Cloud Device Co-op]grupo pasan ID de consumidor únicos con hash criptográfico a Device Graph. El ID de consumidor representa a un usuario autenticado en el gráfico y protege la privacidad del consumidor.

## Vínculos probabilísticos {#section-5f5aa755da984f9d851f7cb380262998}

Los vínculos probabilísticos conectan un dispositivo a una persona de forma algorítmica, en función de características y metadatos como:

* Comportamiento de exploración
* Direcciones IP
* Sistemas operativos
* Identificadores IDFA y GAID

Veamos cómo funciona la vinculación probabilística. En este ejemplo, Persona A se desplaza a un sitio de noticias en su tablet y, posteriormente, desde un equipo de escritorio. Durante la navegación, Persona A no inicia sesión en el sitio de noticias. Durante cada visita por separado, la tablet y el escritorio comparten la misma dirección IP.

![](assets/link3.png)

En base a esta información, el [!DNL Device Graph] evaluará los patrones de uso compartido de direcciones IP entre ambos dispositivos y los vinculará si los resultados sugieren que pertenecen a Persona A. El resultado final es una jerarquía de identidad derivada de cálculos de probabilidad algorítmicos.

![](assets/link4.png)

En este ejemplo, Device Graph vinculó ambos dispositivos después de que se utilizaran para acceder al mismo sitio de noticias. Pero no es necesario ver dispositivos en el mismo sitio para vincularlos. Para ilustrar este punto, digamos que cada dispositivo de este ejemplo visita sitios web completamente diferentes. El [!DNL Device Graph] algoritmo puede seguir creando un vínculo probabilístico basado en su dirección IP compartida y en una análisis de otros datos. Este proceso es lo que ayuda a que la vinculación probabilística sea tan eficaz para los miembros de Device Co-op [!DNL Experience Cloud] .

## Ambos tipos de datos proporcionan valor {#section-43d22d8c10634edcb261e7bda6fdf323}

Los datos determinísticos y probabilísticos se complementan entre sí. Por el contrario, un gráfico de dispositivos que solo incluye datos determinísticos proporciona una vista limitada de la identidad de una persona. Sin autenticación, un gráfico de dispositivos no puede informarle sobre otros dispositivos y personas que exploran el sitio. Los datos probabilísticos pueden realizar estas conexiones y ayudarle a alcanzar dispositivos, personas y hogares no autenticados.

Sin embargo, los datos determinísticos también son importantes. Puede, por ejemplo, mejorar la toma de decisiones probabilísticas eliminando enlaces falsos generados en lugares donde las señales probabilísticas son abundantes y se superponen (por ejemplo, cafeterías, bibliotecas, aeropuertos, etc.).

Con ambos tipos de datos, Device Graph proporciona una imagen más completa de la identidad de una persona que con cualquiera de los dos tipos por separado.

![](assets/link5.png)

