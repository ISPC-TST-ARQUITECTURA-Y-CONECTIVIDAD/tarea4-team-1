# ¿Qué es un archivo JSON y para qué sirve?  
JSON es una notación para expresar datos con el formato de los literales de objeto de JavaScript. Los archivos JSON son simples archivos de texto que contienen datos que se pueden consumir desde las aplicaciones.

Estos archivos sirven para compartir datos estructurados de manera simple y fácil de leer, tanto para los sistemas informáticos y los lenguajes de programación como para las personas. En la práctica lo podrían usar las aplicaciones de cualquier tipo pero donde más ha tenido impacto es en el desarrollo de aplicaciones o sitios web, donde tenemos separadas las distintas capas de aplicación (frontend / backend). Gracias a JSON los datos que necesitan ambas capas de aplicación pueden ser fácilmente definidos y transferidos a través de Internet.

Por supuesto ese es solo un marco de los muchos posibles, ya que por su potencial de almacenamiento es posible sacarle partido también para la persistencia de los datos en las aplicaciones, definir su configuración, etc. Además, no solamente lo podemos usar en el ámbito web, sino también en el desarrollo de aplicaciones de escritorio, aplicaciones móviles, etc.

Su simplicidad, versatilidad y la compatibilidad con la mayoría de los lenguajes de programación lo han colocado en una posición predominante dentro de los formatos de intercambio de datos. 

**Características del archivo .JSON**
Ahora queremos hacer un recorrido a las características principales de los archivos de datos con notación JSON.

**Estructura básica de un archivo JSON**
Un archivo JSON se organiza en pares de clave / valor. La clave es el nombre del dato, su significado. Por su parte, el valor puede ser de distintos tipos, principalmente aquellos que incorpora el propio lenguaje JavaScript.

Para que nos entendamos, si es que no conoces los literales de objeto de JavaScript, los pares clave / valor serían similar al concepto de diccionario o mapa, disponibles en múltiples lenguajes de programación. 

Veamos un ejemplo de JSON para definir algunos datos de una receta de cocina.

{  
    "nombre": "Gazpacho",  
    "tipo": "Sopa fría",  
    "origen": "España",  
}  

Esta estructura permite trabajar muy fácilmente con los datos, tanto para la recuperación de la información como para su generación.

Además, los datos en JSON pueden ser anidados, permitiendo estructuras de datos tan complejas como sea necesario. Por ejemplo, nuestra receta de cocina podría tener una definición más compleja:

{  
    "nombre": "Gazpacho",  
    "tipo": "Sopa fría",  
    "origen": {  
        "pais": "España",  
        "region": "Andalucía"  
    },  
    "ingredientes": [  
        {  
            "nombre": "Tomate",  
            "cantidad": "1 kg"  
        },  
        {  
            "nombre": "Pimiento verde",  
            "cantidad": "100 g"  
        }  
    ]  
}  

**Formato ligero y legible:**  
Por qué JSON se ha convertido en un estándar de intercambio de datos.  
Dos de las cualidades más importantes de los archivos en JSON son la su facilidad de lectura y su poco peso, al menos frente a otros formatos de intercambio. Ello ha contribuido a mejorar su popularidad y a posicionarse como un estándar de intercambio de datos. 

Los datos se presentan de manera clara y concisa, con una estructura bien definida, donde queda perfectamente declarada la función que hace cada uno de los datos en el documento.  

Además, gracias al tamaño pequeño de los archivos JSON se pueden transferir rápidamente por la red y ahorran consumo de datos en las comunicaciones.

**Compatibilidad con múltiples lenguajes de programación**  
Sin duda otra de sus características más relevantes es la compatibilidad existente con la mayoría de los lenguajes de programación. No solo se pueden usar de manera nativa en JavaScript, sino también en muchos otros lenguajes como PHP o Python. Por tanto, no se requieren librerías adicionales en la mayor parte de los lenguajes. 

Además, JSON es una notación también muy usada para almacenar información en las bases de datos. No solo lo soportan las bases de datos NoSQL, sino también otros sistemas gestores como MySQL, que han evolucionado ofreciendo soporte nativo.

**Facilidad de uso y manipulación**  
Usar un archivo JSON es algo prácticamente inmediato. Una vez recuperada la información somos capaces de acceder a cualquiera de las propiedades con una sintaxis directa y sin la necesidad de hacer complejos recorridos en el árbol de datos. 

Esta sencilla manipulación de los datos no solo impacta en el menor consumo de tiempo de procesamiento en las aplicaciones, sino además es muy importante la claridad del código que aporta a la hora de usar las estructuras de datos.

**Tipos de datos en archivos .JSON**  
Los tipos de datos que admite JSON para sus valores son básicamente los que podemos encontrar en el lenguaje JavaScript, con algunas limitaciones.

**Números**  
Como valor de las propiedades JSON podemos usar simples números, ya sean números enteros (3) como números reales (4.67).

**Strings**  
Los Strings son secuencias de caracteres. También las llamamos simplemente «cadenas» en español y se representan siempre entre comillas dobles.

**Array**  
Los arrays, también llamados arreglos, tablas o listas, son colecciones de elementos que pueden a su vez ser de cualquier tipo de los soportados en JSON. Se representan entre corchetes ([]).

**Objetos**  
Los objetos en JSON son como otros JSON, es decir, otras colecciones de pares de clave / valor. Se representan entre llaves ({}). Por ello, el valor de una propiedad de un objeto JSON puede ser otro objeto JSON.

**Booleanos**  
Los booleanos son un tipo de datos habitual en los lenguajes de programación representan valores positivos o verdaderos (valor true) y valores negativos o falsos (valor false).

**Null**  
Adicionalmente, un archivo JSON también puede tener el valor null o propiedades con valor null. Este es un valor especial que tiene como significado vacío.

**¿Cómo abrir un archivo .JSON?**  
Como ya hemos señalado, los archivos JSON están formados por simple texto plano. Por ello los podemos abrir con cualquier editor de texto. Sin embargo, es importante que el editor escogido sea capaz de trabajar con texto plano y no texto enriquecido como ocurre en editores como Word.

Ejemplos de programas que podemos usar son Visual Studio Code, Notepad++, Sublime Text, etc. También podríamos abrirlos con otros editores de texto sencillos como el Bloc de Notas de Windows, sin embargo recomendamos editores enfocados a la programación ya que JSON es importante que se codifique con archivos de texto con el juego de caracteres UTF-8 y los editores para programadores trabajan con este formato de manera predeterminada.

Si fuera necesario, también existen programas y herramientas online especializadas para trabajar con JSON, como JSONLint, que proporcionan una visualización bien estructurada y además permiten también verificar y validar la estructura de los datos en el archivo .JSON.

JSON vs. otros archivos de intercambio de datos: ¿Qué lo hace único?
No podemos hablar de JSON sin compararlo con otros lenguajes de intercambio de datos. Las comparaciones más habituales son las siguientes:

**Comparación con XML: ¿Por qué JSON ha ganado popularidad sobre XML?**  
XML fue durante mucho tiempo el formato de intercambio de datos más estándar en el desarrollo de software. Sin embargo JSON ha ganado terreno por su simplicidad y eficiencia. 

JSON requiere menos texto que XML para expresar lo mismo. Esto es porque en XML se requieren etiquetas de inicio y de cierre para cada dato y a menudo hay que repetir las mismas etiquetas para declarar los elementos de colecciones, algo que conseguimos en JSON con unos simples corchetes y comas.  
Al usar menos texto consigue ser más ligero y rápido de transferir.  
JSON es además más fácil de manipular y no requiere complejos recorridos a las estructuras.  
Los desarrolladores web se sienten muy confortables, ya que JSON tiene una notación usada habitualmente en JavaScript.  
XML a menudo requiere librerías adicionales para el tratamiento en los lenguajes de programación, mientras que JSON es nativo en la mayoría de los casos.    

**Ventajas sobre formatos más antiguos, como CSV y YAML**  
Existen otros formatos que han ofrecido soporte al intercambio de datos de manera tradicional, como CSV. En JSON encontramos también ventajas relevantes:

Los CSV solo pueden representar estructuras de datos tabulares con filas y columnas mientras que JSON admite cualquier estructura de datos tan compleja como sea necesario.  
En CSV hay muy poca flexibilidad en lo que respecta a la variabilidad de los datos, algo que sí ofrece JSON
Los lenguajes de programación no soportan CSV de manera nativa.  
 Con respecto a YAML, JSON tiene tanto ventajas como desventajas.   

JSON es más legible de manera general  
YAML suele ser más ligero y no requiere llaves, pero el hecho de tenerlas en JSON ofrece una mejor comprensión de la estructura de los archivos  
YAML requiere una indentación rígida o el sistema no es capaz de interpretarlo bien.  Por su parte JSON puede ser escrito con mayor libertad, lo que beneficia la edición manual de los datos.  
JSON es mucho más compatible con los lenguajes de programación habituales.  
Escenarios comunes de uso de archivos JSON en el desarrollo de aplicaciones  
Los archivos JSON se utilizan en una variedad de contextos. Podemos encontrar innumerables ejemplos en el marco del desarrollo de software. Algunos de los usos más comunes incluyen:

**Almacenamiento de configuraciones y preferencias de usuario**  
JSON es una opción popular para almacenar configuraciones y preferencias de usuario en las aplicaciones, debido a su simplicidad y facilidad de edición.

**Comunicación entre servicios web y APIs**  
La utilidad más destacada de los datos con notación JSON la encontramos en la comunicación entre servicios web. Es habitual que las APIs envíen y reciban datos en archivos .JSON como primera opción.

**Intercambio de datos entre diferentes plataformas y sistemas**  
El hecho de JSON estar escrito en archivos de texto plano lo hace ideal para su transporte en todo tipo de redes, como Internet. Por ello es muy habitual su uso para comunicar datos entre diferentes sistemas.

**Herramientas y librerías para trabajar con archivos JSON**  
Existen numerosas herramientas y librerías que facilitan la creación, edición y manipulación de archivos JSON. La mayoría de ellas pertenecen de manera nativa a los lenguajes, por lo que no es necesario que se desplieguen componentes de terceros para acceder a los datos.

Librerías populares en diferentes lenguajes de programación: Python, JavaScript, etc.  
En JavaScript podemos usar las funciones JSON.parse() y JSON.stringify() para interpretar cadenas de texto en JSON y para serializar datos en archivos .JSON.

Otros lenguajes tienen también soporte con las librerías que se ofrecen de base. Por ejemplo en Python tenemos que usar la librería «json», haciendo el correspondiente import. Una vez importada la librería usamos json.load() para leer e interpretar un dato escrito en JSON.

Por su parte, en PHP disponemos principalmente de dos funciones para el tratamiento de JSON. Por un lado tenemos json_decode() para decodificar una cadena con un JSON y convertirla en un objeto PHP y json_encode() que devuelve una cadena con JSON a partir de cualquier dato disponible en PHP.

**Editores y validadores de JSON que facilitan la creación y edición de archivos**  
Para trabajar con JSON no necesitamos ninguna herramienta en especial, más allá del propio editor para programadores de nuestra preferencia. Sin embargo existen algunas herramientas online que permiten editar y validar JSON, así como corregir su formato. Algunos ejemplos son https://jsonlint.com/ o https://jsonformatter.org/ 

De todos modos, como hemos dicho, la mayoría de los editores modernos ofrece una interfaz amigable para la creación y edición de archivos JSON, así como una validación implícita de su estructura gracias a los intérpretes de JavaScript que llevan incorporados.

Como puedes comprobar JSON se ha introducido de manera generalizada en el mundo del desarrollo, no solamente en la web sino en la mayoría de las plataformas modernas. Si te dedicas al mundo del desarrollo lo habrás podido comprobar por ti mismo y, si no es así, lo podrás apreciar a poco que vayas adquiriendo experiencia.