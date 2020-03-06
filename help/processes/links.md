---
description: Cómo Device Graph analiza los datos determinísticos y probabilísticos para crear un mapa que vincule los dispositivos.
seo-description: Cómo Device Graph analiza los datos determinísticos y probabilísticos para crear un mapa que vincule los dispositivos.
seo-title: Vínculos determinísticos y probabilísticos
title: Vínculos determinísticos y probabilísticos
uuid: 00693a0a-f73d-460d-84a4-b7c745b9fe0a
translation-type: tm+mt
source-git-commit: c1d0bc05d3f211fa3e899e98fbcc908be7399031

---


# Deterministic and probabilistic links{#deterministic-and-probabilistic-links}

Cómo Device Graph analiza los datos determinísticos y probabilísticos para crear un mapa que vincule los dispositivos.

En [!DNL Device Graph], los procesos internos crean una jerarquía de identidad que toma dispositivos y los conecta con personas concretas anónimas. El resultado del gráfico incluye vínculos entre dispositivos que puede utilizar para dirigir la campaña, junto con datos expuestos en determinadas soluciones de Experience Cloud. The Adobe solutions that work with [!DNL Device Graph] data include Analytics, Audience Manager, Media Optimizer, and Target.

[!DNL Device Graph] analiza datos determinísticos y probabilísticos para construir un mapa que vincula distintos dispositivos. Los datos determinísticos lo hacen en función de la información de inicio de sesión almacenada como hash. Los datos probabilísticos lo hacen empleando información como direcciones IP y otros metadatos. [!DNL Device Graph] asocia los clústeres de dispositivos vinculados a una persona anónima concreta. Estas conexiones permiten a los especialistas en marketing dirigirse a personas, no a dispositivos. En [!DNL Device Graph], el propietario de un dispositivo es la representación anónima de una persona real. Ambas vinculaciones, la determinística y la probabilística, ayudan a crear una estructura de la identidad del usuario.

>[!NOTE]
>
>En Adobe Experience Cloud Device Co-op, términos como *dispositivo*, *persona* e *identidad* tienen significados específicos. For example, *device* can refer to physical hardware such as a phone or tablet and the applications that run on that hardware. Consulte las definiciones en el [glosario](../glossary.md#glossgroup-0f47d7fbd76c4759801f565f341a386c).

## What are links? {#section-2df4c6f01eba49369993146df0661f13}

Cuando hablamos de vínculos, es importante tener en cuenta lo que son realmente en el contexto de Device Graph y [!DNL Experience Cloud]. En este contexto, no se trata de conexiones físicas entre dispositivos. Un vínculo es el modo en que Device Graph asocia distintos dispositivos a una misma persona cuya identidad es desconocida. Por ejemplo, digamos que tenemos un teléfono móvil y un navegador de escritorio. Ambos pueden considerarse &quot;vinculados&quot; cuando Device Graph determina que los dos los utiliza la misma persona anónima. Como verá más adelante, Device Graph crea identidades mediante vínculos de determinación y de probabilidad. En Device Graph, el propietario de un dispositivo es la representación anónima de una persona real.

## Deterministic links {#section-33d41e828a674b398e36fe63da20ac09}

Los vínculos determinísticos asocian un dispositivo a una persona basándose en un evento de autenticación (p. ej., una acción de inicio de sesión en un sitio desde un dispositivo). Esta acción crea un identificador anónimo conocido como ID de consumidor. Veamos cómo funciona la vinculación determinística. En este ejemplo, Persona A inicia sesión en un sitio de noticias mediante una aplicación instalada en su dispositivo móvil. Más tarde, Persona A vuelve a iniciar sesión, pero esta vez desde un navegador de su ordenador portátil.

![](assets/link1.png)

En función de la información de inicio de sesión, Device Graph:

* Sabe que Persona A se ha autenticado en el sitio de noticias con la combinación de dispositivos teléfono móvil/aplicación y portátil/navegador.
* Vincula estos dispositivos a Persona A.
* Crea una identidad basada en los dispositivos vinculados asociados a la persona, que es anónima.

![](assets/link2.png)

>[!NOTE]
>
>Neither the [!DNL Adobe Experience Cloud Device Co-op] or the [!DNL Device Graph] receives actual authentication information or personally identifiable information (PII) in this data. Members of the [!DNL Experience Cloud Device Co-op], pass in cryptographically hashed, unique consumer IDs to the Device Graph. El ID de consumidor representa a un usuario autenticado en el gráfico y la privacidad del consumidor queda protegida.

## Probabilistic links {#section-5f5aa755da984f9d851f7cb380262998}

Los vínculos probabilísticos conectan un dispositivo con una persona de forma algorítmica, en función de características y metadatos como:

* Comportamiento de navegación
* Direcciones IP
* Sistemas operativos
* Identificadores IDFA y GAID

Veamos cómo funciona la vinculación probabilística. En este ejemplo, Persona A navega por un sitio de noticias con su tableta y más tarde con su equipo de escritorio. Lo hace sin iniciar sesión en el sitio de noticias. Durante estas visitas separadas, la tableta y el equipo de escritorio comparten la misma dirección IP.

![](assets/link3.png)

Basándose en esta información, [!DNL Device Graph] evalúa los patrones de uso compartido de la dirección IP entre ambos dispositivos y los vincula si el resultado sugiere que pertenecen a Persona A. El resultado final es una jerarquía de identidad derivada de cálculos estadísticos algorítmicos.

![](assets/link4.png)

En este ejemplo, Device Graph vinculó ambos dispositivos al haber sido utilizados para visitar el mismo sitio de noticias. Sin embargo, no es necesario que dos dispositivos visiten un mismo sitio para ser vinculados. Para ilustrarlo, digamos que con los dos dispositivos del ejemplo se visitaron sitios web totalmente distintos. El algoritmo de [!DNL Device Graph] puede realizar igualmente una vinculación probabilística basándose en la dirección IP compartida y en el análisis de otros datos. Este proceso es lo que ayuda a hacer tan potente la vinculación probabilística para los miembros de [!DNL Experience Cloud] Device Co-op.

## Both types of data provide value {#section-43d22d8c10634edcb261e7bda6fdf323}

Los datos determinísticos y probabilísticos se complementan. En contraste, un gráfico de dispositivos que contiene solo datos determinísticos ofrece una visión limitada de la identidad de una persona. Sin autenticación, un gráfico de dispositivos no puede informarle de otros dispositivos y personas que navegan por su sitio. Los datos probabilísticos pueden realizar estas conexiones y ayudarle a alcanzar dispositivos, personas y domicilios no autenticados.

Sin embargo, los datos determinísticos también son importantes. Pueden, por ejemplo, mejorar la toma estadística de decisiones eliminando falsos vínculos generados en lugares donde abundan y se solapan las señales probabilísticas (p. ej., en cafeterías, bibliotecas, aeropuertos, etc.).

Con ambos tipos de datos, Device Graph proporciona una imagen más completa de la identidad de una persona que con solo uno de los tipos.

![](assets/link5.png)

