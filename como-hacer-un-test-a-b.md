# Cómo hacer un Test A/B

### Crear un test A/B

Desde Modular pages es posible realizar un test A/B para poder testar cómo funciona un cambio en un módulo.

### Antes de empezar...

Es importante que tengas en cuenta que no es posible crear un test A/B sin coordinarlo con el equipo de Digital Analytics dado que la base de un test A/B es poder medir los resultados. Para poder medir esos resultados es necesario el uso de Firebase.

### Pasos a seguir para crear un Test A/B en Modular pages

**Paso 1**. Para empezar es necesario tener permisos de creación de Test A/B en el CMS. Si no lo tienes, contacta con el NOC para que te los dé <img src="https://confluence.tid.es/s/24eubp/9012/15522zw/_/images/icons/emoticons/wink.svg" alt="(guiño)" data-size="line">. También puedes pedir ayuda a tu OBPM o persona de referencia que tengas en Novum para que te ayude.

{% hint style="info" %}
No es un permiso que tengas activado por defecto así que si no lo has solicitado nunca lo normal es que NO lo tengas. 🙋🏾
{% endhint %}

**Paso 2**. Accede a Modular pages y edita la página en la que quieras meter ese Test.

**Paso 3**. En el paso **Content**, busca el módulo que quieres testar. Haz clic en el submenú del módulo y selecciona la opción **A/B Test**

<figure><img src=".gitbook/assets/iniciarABTest.png" alt=""><figcaption></figcaption></figure>

**Paso 4**. Añade el nombre del test. El **Key name** es el nombre que se usará en Firebase para identificar el test. Haz clic en **Continue**.

<figure><img src=".gitbook/assets/FirebaseKey.png" alt=""><figcaption></figcaption></figure>

**Paso 5.** Al añadir el Key name se abre la modal de edición del módulo, exactamente una réplica del módulo sobre el que estás haciendo el test A/B. Haz los cambios relacionados con el test y haz clic en **OK**.

<figure><img src=".gitbook/assets/A_BTestCreado.png" alt=""><figcaption></figcaption></figure>

Como ves, se ha creado otro módulo y ahora cada uno está identificado con A y B, siendo A el módulo de referencia (el módulo origen, el que ya está en Producción) y siendo B el módulo a testar, también llamado Variant A en la herramienta de Firebase.

**Paso 6.** **IMPORTANTE**. Aún no se han llevado los cambios a PROD porque para ello tienes que hacer clic en **Continue**, en el paso **2 Content** en el que estás. Y terminar de publicar, en el paso 3, toda la página modular.\


![(estrella roja)](https://confluence.tid.es/s/24eubp/9012/15522zw/\_/images/icons/emoticons/star\_red.svg) **IMPORTANTE** ![(estrella roja)](https://confluence.tid.es/s/24eubp/9012/15522zw/\_/images/icons/emoticons/star\_red.svg)&#x20;

Hasta que el test no se lance en Firebase el usuario de la app seguirá viendo lo que hay en producción, es decir, el módulo de referencia, con independencia de que ya se haya configurado el test en Modular pages. Por eso es de vital importancia que te coordines con el equipo de Digital Analytics para que sepas cuándo empezará a verse el test. La parte buena es que puedes dejarlo preparado en el CMS de Modular pages para cuando DA pueda activarlo en Firebase.

### Pasos para marcar opción ganadora en Modular pages

El test A/B ha finalizado y ya tienes los resultados en Firebase. Y ahora, ¿qué?

**Paso 1**. Con los datos analizados y la decisión tomada sobre qué módulo es el ganador, accede al CMS de Modular pages dónde está corriendo el test A/B y edita la página que contiene el test.

<figure><img src=".gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

**Paso 2**. Haz clic en el submenú del módulo ganador y selecciona **Set as winner**.

<figure><img src=".gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

\


**Paso 3.** Aparece una ventana de resumen mostrando el módulo ganador y una preview. Confirma el cambio haciendo clic en **Set as Winner**. En ese momento se elimina el módulo descartado.

<figure><img src=".gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

**Paso 4**. **IMPORTANTE**. Aún no se han llevado los cambios a PROD porque para ello tienes que hacer clic en **Continue**, en el paso **2 Content** en el que estás.&#x20;

Ya en el paso **3 Overview** haz clic en **Save and publish**.&#x20;

Se abre una modal para que indiques una descripción para el cambio que vas a llevar a cabo. Haz clic en **Confirm** para terminar la configuración.

### Buenas prácticas

Es importante que crees un ticket al equipo de Digital Analytics describiendo el test. También es importante que os coordinéis porque no sirve de nada que tengas configurado un test A/B en Modular Pages si desde Firebase ese test no se inicia.

[Template Test A/B: \[OB\] Test A/B name](https://confluence.tid.es/pages/viewpage.action?pageId=141016807)\
