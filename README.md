INFORME DEL PROYECTO

PROYECTO:

SISTEMA DE GESTION DE LIBROS ELECTRONICOS

DESARROLLADOR: Carlos Maruri Mediavilla

RESUMEN:
Se está desarrollando un sistema modular en el lenguaje Go para gestionar libros electrónicos mediante una interfaz de consola. Esta versión permite listar, agregar, editar y eliminar libros, usando una estructura en capas que incluye modelado, persistencia en MySQL y una interfaz básica por terminal.

OBJETIVOS:
- Diseñar un sistema funcional en consola.
- Conectar con base de datos MySQL.
- Implementar operaciones CRUD completas.
- Preparar la arquitectura para una futura versión web.

LENGUAJE:

Go (Golang)
El lenguaje utilizado en este proyecto es Go (también conocido como Golang), un lenguaje de programación desarrollado por Google. Go es conocido por su simplicidad, eficiencia y excelente soporte para la concurrencia, lo cual lo convierte en una excelente opción para aplicaciones de servidor y sistemas distribuidos. En este sistema, Go facilita una arquitectura clara y mantenible, manejando la lógica de negocio, enrutamiento HTTP y conexión a bases de datos de manera eficiente. Su tipado estático, compilación rápida y librerías estándar robustas permiten desarrollar aplicaciones seguras y de alto rendimiento.

DESCRIPCIONES y CAMBIOS REALIZADOS
1. Modelado de datos
Se definió la estructura `models.Libro` con campos privados y métodos públicos de acceso, encapsulando los datos del libro: Título, Autor, Categoría y Año.


2. Base de Datos
Se creó una tabla `libros` en MySQL. La conexión se gestiona desde el paquete `bd` con uso de variables de entorno.
3. Interfaz administrativa
Se desarrolló un menú en consola para operar las funciones básicas: listar, agregar, editar y eliminar libros.
4. Funcionalidades del Sistema
- Listar libros
- Agregar nuevo libro
- Editar libro existente
- Eliminar libro
- Guardar y recuperar desde MySQL
5. Problemas encontrados
Inicialmente se presentaron errores de conexión y manejo de tipos de datos. También se depuró el manejo de índices al modificar libros.
6. Migración Web
Integrar interfaz web con templates HTML, migrar el flujo de consola a navegador, mantener lógica modular y mejorar validaciones.
7. Diagramas del Sistema
Se elaboró un diagrama de arquitectura en capas: modelo, controlador, base de datos, interfaz.
8. Documentación adicional
- Archivo `.env`
- Comentarios en el código fuente
9. Rutas de Interés (links git)
  
https://github.com/oldwolf68/Golang-programing



CONCLUSIONES:

El desarrollo del sistema de gestión de libros electrónicos en su versión de consola ha permitido sentar las bases funcionales del proyecto, asegurando que los principales procesos como el modelado de datos, la interacción con la base de datos y las operaciones CRUD básicas estén correctamente implementados. El uso del lenguaje de programación Go ha demostrado ser una elección acertada para este tipo de sistemas debido a su simplicidad, rapidez de ejecución, manejo eficiente de concurrencia y su enfoque en la claridad y mantenibilidad del código. 
Además, la modularidad implementada a través de interfaces y paquetes ha facilitado la escalabilidad del sistema hacia futuras versiones web. Durante este avance se han abordado retos importantes como el diseño inicial del modelo de datos, la conexión y operaciones con MySQL, así como la implementación de una lógica de servicios que abstrae las operaciones de almacenamiento. Estos componentes se han integrado con éxito para permitir la gestión básica de los libros desde la terminal.


Incorporar paquetes estándar y externos documentados:
Se deben utilizar paquetes como html/template, net/http, y otros externos como gorilla/mux, documentando su propósito y aplicación en el sistema.

Construir una interfaz web básica con vistas HTML renderizadas dinámicamente:
Se deben generar páginas dinámicas que muestren los datos del sistema utilizando el motor de plantillas de Go.
