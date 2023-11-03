# Crear páginas alternativas

Del mismo modo que es posible configurar [módulos alternativos](como-crear-una-pagina-modular/contenido.md#crear-un-grupo-de-modulos-alternativos), sucede parecido con las páginas.&#x20;

Puede ser que necesites crear la misma página pero con apariencia significativamente diferente para un grupo de usuarios.

En ese caso, sobre la página que necesites, desde la pantalla principal de páginas, haz clic en **+Add new page**.

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

La condición necesaria es que añadas una audiencia para esta nueva página para que tenga sentido que tengas esa nueva "versión" de la página para una audiencia determinada.

Ejemplo:

_Alice está creando una página de inicio de la app con varios módulos. Pero sabe que para un determinado grupo de usuarios, aquellos que aún no disponen de su usuario porque acaban de darse de alta con la app, esa página de inicio es totalmente distinta._

_¿Cómo lo hace Alice?_

_Una vez creada la página de inicio con los módulos crea una página alternativa en la que indica que esa página es para los usuarios con la audiencia `new-user`. En esa página incluye un único módulo, que lleva solo el módulo de acceso a preguntas frecuentes._

_De esa manera Alice puede gestionar mucho mejor el contenido que ven unos y otros usuarios._

Otro ejemplo de uso muy frecuente es cuando las páginas están relacionadas con productos en cuyo caso puede ser muy útil, e incluso necesario, crear páginas alternativas.

_Ejemplo_

_Alice necesita crear la página de principal de línea móvil pero esas páginas están relacionadas con el producto móvil y son diferentes si el usuario es prepago, si el usuario es postpago y además tiene un plan contratado o si el usuario tiene una línea postpago suelta._

_Para ello Alice crea tres páginas alternativas, una para cada situación, a las que indica las audiencias correspondientes y sobre las que añadirá los módulos que considere._

### Cómo ordenar las páginas alternativas

Para que el sistema evalúe qué página muestra al usuario de la app, necesita ordenar esas páginas.&#x20;

{% hint style="info" %}
Recuerda que **el sistema evalúa de arriba abajo**, es decir, la primera que coincida con el usuario, empezando por arriba, será la que muestre en la app, sin evaluar las siguientes.

Ten muy en cuenta esto de cara a decidir el orden en que colocas estas páginas.
{% endhint %}

Mueve las páginas con _Drag\&Drop_ y cuando las tengas colocadas como consideras haz clic en **Save order.**

{% hint style="warning" %}
Solo puedes tener una página que **no contenga audiencias** y esa página tiene que estar siempre en **último lugar**. El sistema te avisa si esto no se cumple e intentas guardar un orden incorrecto.
{% endhint %}

<figure><img src=".gitbook/assets/MovePages.gif" alt=""><figcaption></figcaption></figure>
