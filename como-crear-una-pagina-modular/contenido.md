# Contenido

El contenido de una página modular se configura mediante la inserción de módulos, la elección del orden de esos módulos dentro de la página así como la configuración de las secciones que los contienen.

Este paso está dividido en dos partes:

* En la parte **izquierda** están los **módulos ordenados** tal y como quieras que se vean en la app.
* En la parte **derecha** una **previsualización**, lo más fiel posible, de lo que verá el usuario de la app.

{% hint style="info" %}
Es importante que tengas en cuenta que además de lo que veas en la previsualización de la derecha, los módulos pueden estar configurados para mostrarse a los usuarios en función de una serie de premisas, entre otras, las audiencias. Por lo tanto, que tú lo veas en esa previsualización no tiene por qué ser exactamente cómo lo vea el usuario.

Si quieres visualizar exactamente cómo ve un usuario concreto una página modular puedes hacer un [Test](../como-probar-el-contenido.md).
{% endhint %}

Además, la página esta dividida en dos partes, una seción **Header**, que siempre verás al crear una nueva página, y el resto de la página que podrá contener una o más secciones, en función de cómo quieras organizar el contenido.

## Cómo crear una sección

Para crear una nueva sección haz clic en **+New section**. Rellena los campos necesarios en la modal que se abre.

<figure><img src="../.gitbook/assets/NewSectionWindow.png" alt=""><figcaption></figcaption></figure>

**Internal name**. Este campo es de uso interno y sirve para que puedas identificar y diferenciar correctamente cada sección de la página modular. Es un campo obligatorio.

💡Intenta que el nombre sea lo más descriptivo posible lo cual te ayudará a saber qué tipo de módulos y qué información va contenida en la sección.

### Design

En esta pestaña indica el color de fondo de la sección. Usa el desplegable **Background color**.

### Content

En esta pestaña configura los campos de sección que sí verá el usuario de la app.

<figure><img src="../.gitbook/assets/section_content.png" alt=""><figcaption></figcaption></figure>

* **Section title (optional)**. Indica el título de sección que verá el usuario de la app cuando se le muestre la página modular que estás creando o editando. Es un campo opcional y por tanto no se verá si no indicas un valor.

{% hint style="success" %}
Una sección puede o no llevar título de sección. Igualmente el contenido (módulos) de la sección se verán siempre que le apliquen al usuario.
{% endhint %}

* **Section description (optional)**. Indica una descripción sobre el contenido de la sección. Esta descripción la verá el usuario de la app. Es un campo opcional.
* **No link**. Opción seleccionada por defecto. Indica que la sección no llevará un enlace.
* **With link**. Selecciona esta opción para añadir un enlace en la sección.&#x20;
  * **Link text action**. Indica el texto del enlace
  * **Select type URL**:
    * **URL**. Selecciona esta opción para rellenar manualmente el siguiente campo **URL**.
    * **Preconfigured**. Selecciona esta opción para seleccionar una de las URL preconfiguradas del campo URL.

<figure><img src="../.gitbook/assets/section_URL.png" alt="" width="563"><figcaption></figcaption></figure>

{% hint style="warning" %}
**¿Por qué no veo la sección que acabo de configurar en la previsualización?**

Hasta que una sección no contenga al menos un módulo esa sección no se verá en la previsualización de la página modular que estás creando o editando.

Así es justamente cómo se comporta una página modular para el usuario de la app. Si una sección tiene módulos pero ninguno le aplica a ese usuario entonces esa sección no aparecerá, aunque tenga módulos dentro y contenga título de sección, descripción y/o enlace.
{% endhint %}

## Cómo añadir un módulo

Los módulos van siempre dentro de una sección y por tanto, antes de añadir un módulo, tienes que [crear al menos una sección](contenido.md#como-crear-una-seccion). Si lo que necesitas es incluir un módulo en el **Header**, esa sección ya está creada por defecto siempre.

Haz clic en **+Add module** dentro de la sección en la que quieras incluir un módulo.

* **Select module**. Selecciona el módulo que vas a añadir.
* **Module Id**. El sistema te ofrece, en función del módulo que has seleccionado, un ID para identificar de manera unívoca el módulo que estás añadiendo. Puedes cambiar el ID del módulo siempre y cuando uses uno nombre que no esté en uso.

<figure><img src="../.gitbook/assets/New_Module.png" alt=""><figcaption></figcaption></figure>

Consulta el Catálogo de módulos disponibles desde el propio CMS. Desde la pantalla principal haz clic en **Module catalog**.&#x20;

¿Necesitas más información sobre cómo consultar el **Catálogo de módulos**? 👇🏼

{% content-ref url="../catalogo-de-modulos-disponibles.md" %}
[catalogo-de-modulos-disponibles.md](../catalogo-de-modulos-disponibles.md)
{% endcontent-ref %}

### Estructura de edición de un módulo

En función del módulo que añadas se muestran los campos que permiten configuración adicional en el CMS. Para ayudarte, esos campos están divididos en pestañas según su tipología:&#x20;

#### Content

En esta pestaña están disponibles todos los campos relacionados con el contenido del módulo.

{% hint style="info" %}
Recuerda que estos campos varían por cada tipo de módulo que añades. Algunos módulos permiten mayor configurabilidad que otros 😉.
{% endhint %}

Si el módulo que incluyes dispone de un CMS específico entonces tendrás un enlace directo para acceder a la edición del elemento.

<figure><img src="../.gitbook/assets/CMSpropio.png" alt=""><figcaption></figcaption></figure>

Si realizar cambios sobre el módulo es necesario que refresques el elemento para que la previsualización sea más fiel. Haz clic en <img src="../.gitbook/assets/image (4).png" alt="" data-size="line">para realizar ese refresco de información.

{% hint style="warning" %}
🚨 En esta guía de uso no se detalla cada campo que puede editarse en un módulo dado que depende del contenido añadido.
{% endhint %}

#### Audience

Desde esta pestaña configura, si lo necesitas, las audiencias que deben ver el módulo que estás creando.

Puedes usar el compositor de audiencias para definir las condiciones que debe cumplir el usuario para ser candidato a ver el módulo.

<figure><img src="../.gitbook/assets/Audience.png" alt=""><figcaption></figcaption></figure>

Haz clic en **+Add condition** para añadir una condición nueva.&#x20;

* Selecciona **Is** en el desplegable para indicar que sí cumpla la audiencia
* Selecciona **Is Not** para indicar que no cumpla la audiencia.
* En el desplegable **Audience** selecciona la audiencia que corresponda.

{% hint style="success" %}
Si no seleccionas **ninguna audiencia** entonces das por hecho que el módulo será visible para **todos los usuarios**.
{% endhint %}

#### Tracking

En esta pestaña puedes configurar los campos de tracking que necesites. Actualmente, muchos de  los campos se trackean de manera automática pero estos son los campos que puedes añadir:

* **module\_id (optional)**. Campo de texto abierto relacionado con el ID del módulo y que atiende al tracking de Universal Analytics\*
* module\_name (optional). Campo de texto abierto relacionado con el nombre del módulo y que atiende al tracking de Universal Analytics\*

_\*Campo que quedaránobsoletos cuando desaparezca Universal Analytics._

* **Content group (optional)**. Selecciona uno de los disponibles en el desplegable.
* **Content\_category (optional)**. En función del valor que hayas seleccionado en el desplegable **Content\_group** se acotan los valores que puedes seleccionar para el **Content\_category**.

**Analytics tracking preview**. Usa esta opción para conocer el tracking de los elementos y los valores que tienen por defecto. Haz clic en la previsualización del módulo sobre los elementos que cuyo tracking quieras conocer.

<figure><img src="../.gitbook/assets/PreviewTracking.gif" alt=""><figcaption></figcaption></figure>

Haz clic en **x Closing preview** para dejar de ver esta información y poder navegar por otras pestañas de la modal de edición.

#### QA

Pestaña dedicada a poder indicar un ID concreto la módulo para ser usado en los test automáticos o manuales del equipo de QA.

**Testing ID (optional)**. Desde el equipo de pruebas usan este campo para comprobar la información mostrada en pantalla.

Por lo general este campo no tienes que rellenarlo 🤓.



Haz clic en **OK** en la modal de creación/edición del módulo cuando hayas rellenado todos los campos necesarios.

{% hint style="danger" %}
**IMPORTANTE**: recuerda que los cambios no se salvan hasta llegar al último paso, en donde podrás publicar los cambios o guardarlos.

Si cierras la pantalla en este momento perderás toda la configuración que hayas realizado.
{% endhint %}



***

## Acciones comunes en la creación/edición de una página

Antes de detallar qué acciones comunes puedes llevar a cabo dentro de una página modular, recuerda que dispones siempre de acciones secundarias, tanto en la sección como en el módulo.

Haz clic en <img src="../.gitbook/assets/image (3).png" alt="" data-size="line"> para abrir el menú secundario.

<figure><img src="../.gitbook/assets/menu_secundario (1).png" alt=""><figcaption></figcaption></figure>

### Mover un módulo dentro de una sección

Usa la opción _Drag\&Drop_ para mover el módulo a la posición deseada.&#x20;

<figure><img src="../.gitbook/assets/move_module_in_the_same_section.gif" alt=""><figcaption></figcaption></figure>

### Mover un módulo a otra sección

Usa la opción _Drag\&Drop_ para mover el módulo a la posición deseada. También dispones del menú secundario **Move to another section**. Se abre una modal para que indiques a qué sección lo quieres mover. Haz clic en **Move module** para confirmar el movimiento a la sección que has indicado. El módulo se sitúa en último lugar de esa sección.

<figure><img src="../.gitbook/assets/move_to_another_section.png" alt=""><figcaption></figcaption></figure>



### Desactivar/Activar un módulo

Desactivar un módulo te permite que no sea visible para los usuarios de la app mientras ese módulo está desactivado. Del mismo modo, activarlo hará que sea visible de nuevo.

😉 Ten en cuenta que cuando desactivas un módulo entonces no se ve en la preview de la parte derecha.

Desactivar un módulo es una acción menos destructiva que eliminarlo dado que en ese caso, para recuperarlo, tendrías que añadirlo de nuevo y configurarlo de cero.

Usa el interruptor que hay junto al módulo para activarlo/desactivarlo:

<figure><img src="../.gitbook/assets/activardesactivar.png" alt=""><figcaption></figcaption></figure>

### Crear un grupo de módulos alternativos

Existen casos en lo que en función de la audiencia de los usuarios necesites que en un determinado punto de la app se muestre un módulo para unos usuarios u otro módulo diferente para los otros. La manera de hacer esto es mediante los módulos alternativos. Esos módulos funcionan como uno solo, es decir, se configuran varios pero en la app solo se muestra uno, el que le aplique al usuario.

Ten en cuenta que el orden en el que estén los módulos alternativos es importante dado que el sistema evalúa, de arriba abajo el primer módulo que le aplique al usuario. Ese será el módulo que se mostrará.

<figure><img src="../.gitbook/assets/image (7).png" alt=""><figcaption><p>Ejemplo de módulos alternativos</p></figcaption></figure>

#### Cómo crear un grupo de módulos alternativos

Lo primero es tener ya uno de los módulos metidos en una sección. A continuación, haz clic en el menú secundario de ese módulo y selecciona **+Add alternative**.

<figure><img src="../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

Configura el nuevo módulo alternativo que quieras. Puedes repetir la operación tantas veces como módulos alternativos necesites.&#x20;

{% hint style="warning" %}
Ten en cuenta que solo un módulo puede no contener audiencia y ese módulo debes colocarlo en última posición dado que si no nunca se evaluaría la condición del resto de módulos.
{% endhint %}

### Crear un test A/B

Desde modular pages es posible realizar un test A/B para poder testar cómo funciona un cambio en un módulo.

Aquí tienes toda la información necesaria 👇🏼

{% content-ref url="../como-hacer-un-test-a-b.md" %}
[como-hacer-un-test-a-b.md](../como-hacer-un-test-a-b.md)
{% endcontent-ref %}

***

Cuando hayas terminado de configurar todo el contenido de la página haz clic en **Continue** para pasar al siguiente paso.

{% hint style="success" %}
Recuerda que los cambios no se guardan de manera automática y que necesitas llegar al último paso para guardarlos o para publicar los cambios. 🤓
{% endhint %}



