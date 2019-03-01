In progress !!!

Tutorial: Cómo crear módulos para VCV-Rack
Entrenamientos y consejos sobre cómo construir su propio instrumento virtual para la plataforma VCV Rack , escrito por uriel Deveaud - 2019

Introducción
Por lo tanto, desea crear sus propios instrumentos o módulos para tocar en VCV Rack . La bienvenida a bordo !

Antes de comenzar a hablar sobre programación de computadoras , veamos el perfil general y los conocimientos básicos que puede necesitar durante el proceso de creación de su complemento. En este momento, tienes una idea, y estoy seguro, ¡la mejor! Como músico, es posible que hayas estado buceando en algún tipo de código ... ¡o no! O tal vez, como programador, ¿quieres aprender a hacer instrumentos musicales y dispositivos de audio ? Esta serie de tutoriales está hecha para ti. Veamos el contexto general:

Básicamente, a los músicos no les gusta perder su tiempo en el trabajo de codificación, pero hay excepciones, por supuesto. En este caso, quieres unirte al grupo de desarrolladores de músicos , y eso está bien. Avanzaremos paso a paso y pasaremos de un módulo básico a uno muy complejo.

Si eres muy nuevo en la programación de audio, c ++ y SVG design , aún puedes seguir esos tutoriales, pero te sugiero que tengas mucha curiosidad y participes con respecto al aprendizaje de las bases o cualquier introducción que puedas ver en youtube u otros foros y páginas de Facebook. ... pregunte, busque y tome notas;) Al ingresar en la creación del módulo, hay un 99% de posibilidades de que produzca más de un complemento, así que, tómelo en serio, aprenda por el método, manténgase organizado, vaya paso a paso , respétate ... y verás, lentamente, ¡tu instrumento cobrará vida! El precio no es nada comparado con la plena satisfacción de crear el dispositivo de tus sueños y encenderlo por primera vez :)

Bueno, echemos un vistazo al menú de este tutorial. Cada sección presenta varias tareas que desea repetir según sea necesario, dependiendo de su proyecto personal. Entonces, primero debe conocer la "estructura del código API de los módulos VCV", saber cómo compilar un complemento y, finalmente, probar su creación "en vivo" en VCV Rack . Una vez que se entienda este ciclo, estará listo para desarrollar las características de su módulo y la interfaz de usuario (UI) . Como acabo de decir, estamos progresando, siguiendo estos 3 pasos en bucle:

Buscando expresiones de código y entendiendo las "reglas"
Adaptar las reglas del código a las necesidades reales.
Secciones de código duplicadas y limpias.
¡Por supuesto, después de algunas veces, construirá su propia biblioteca de códigos y podrá saltar rápidamente al siguiente nivel! Una sugerencia común, y es muy importante, si usted no es un programador experimentado, "explorar" los códigos de otros Módulos desde las páginas de sus autores. De ellos, aprenderá qué solución eligieron y cuál es el resultado. Puede descargar sus repositorios y construirlos en su máquina local. Buena enseñanza, pero al menos, necesitas entender lo que estás leyendo :) Alcancemos este objetivo junto con esta serie de tutoriales. Disfrutar

 Resumen
Prerrequisitos
Tutorial 01: Configure su entorno de desarrollo en Win10 > Lea el tutorial
Instalar un compilador y un editor de texto.
Descarga del repositorio de rack VCV y compilación de la aplicación principal
Configurando archivos y carpetas
Construyendo tu primer módulo completo
Tutorial 02: Construya y pruebe los módulos básicos de VCV clásicos >> Lea el tutorial
Descarga los archivos del paquete
Construye y prueba los módulos en VCV Rack
Tutorial 03: Usa la nueva plantilla de tutoriales >> Lee el tutorial
Establecer los archivos y carpetas de configuración básica del módulo
Construye y almacena nuevos módulos.
Pruebe su módulo en VCV Rack
Organizando tu trabajo y planificando tareas.
Tutorial 04: Consolidando y validando su proyecto >> Lea el tutorial
Compruebe si existen complementos similares
Dibuja algunas maquetas y define características.
Tutorial 05: ¿Estás listo? Si es así, es hora de trabajar >> Leer el tutorial
Configurando tu SLUG, ModuleName y archivos
Definiendo tamaño y estilo para tu módulo.
Comentando tus bloques de código
Construyendo tu primer módulo creado
Tutorial 06: Construyendo componentes básicos> TODO
Objetivo, crear un circuito de audio simple, también conocido como "EL MEZCLADOR"
Creación de puertos de entrada y salida
Creando un mando que controla un parámetro num.
Creando un botón de cambio para cambiar un parámetro booleano.
Creando un vu meter para visualizar un param param
Creando una pantalla para visualizar cualquier param.
Creando un botón momentáneo
Creando un menú con infos estáticos.
Creando una información dinámica del usuario en el panel.
Tutorial 07: Personalizando tus componentes> TODO
Creando tu capa de fondo
Creando nuevos controles
Creando un panel de pantalla
Añadiendo algunas informaciones condicionales en el menú.
Añadiendo algunas carpetas para presets
Construyendo un módulo avanzado
Tutorial 08: Creando una fuente de audio> TODO
Objetivo, crear un nuevo circuito de audio, también conocido como "EL SAMPLER".
...
Tutorial 09: Creando un generador de ondas> TODO
Objetivo, crear un nuevo circuito de audio, también conocido como "EL SINTETIZADOR"
...
Tutorial 10: Creando una sección de filtro> TODO
Objetivo, crear un nuevo circuito de audio, también conocido como "EL EQUALIZADOR".
...
...

Estoy buscando personas que puedan ayudar a ampliar esta documentación sobre la creación de módulos en MacOS y Linux;)
