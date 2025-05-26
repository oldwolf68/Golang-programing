Sistema de Gestión de Libros Electrónicos

Objetivo General

Diseñar y desarrollar un sistema web funcional y modular en Go que permita gestionar libros electrónicos mediante la incorporación de técnicas de programación funcional, estructuras de datos organizadas y un enfoque escalable, reutilizable y mantenible.

Objetivos Específicos

Permitir el registro de nuevos libros electrónicos:
El sistema debe brindar una interfaz para que el usuario ingrese información como título, autor, categoría, año y un identificador único.

Visualizar y listar todos los libros registrados:
Se debe renderizar una vista dinámica que muestre todos los libros almacenados, de forma ordenada y clara.

Implementar búsqueda y filtrado funcional:
Los usuarios deben poder buscar libros por criterios como autor o título, utilizando funciones puras para procesar los datos.

Actualizar la información de libros existentes:
El sistema debe permitir modificar los datos de un libro de forma controlada y validada.

Eliminar libros del sistema de forma segura:
Se debe ofrecer una opción para eliminar registros, con verificación para evitar eliminaciones accidentales.

Separar claramente la lógica funcional de la lógica de entrada/salida:
Todas las funciones de procesamiento (filtrar, validar, calcular) deben estar desacopladas de la capa que maneja las peticiones HTTP o la base de datos.

Utilizar programación funcional como base de desarrollo lógico:
El sistema debe estructurarse para aprovechar funciones puras, evitar el uso de estado global y fomentar código inmutable y reutilizable.

Incorporar paquetes estándar y externos documentados:
Se deben utilizar paquetes como html/template, net/http, y otros externos como gorilla/mux, documentando su propósito y aplicación en el sistema.

Construir una interfaz web básica con vistas HTML renderizadas dinámicamente:
Se deben generar páginas dinámicas que muestren los datos del sistema utilizando el motor de plantillas de Go.
