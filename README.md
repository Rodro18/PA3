# Portal del Estudiante

## Descripción del proyecto

El proyecto Portal del Estudiante es una aplicación web desarrollada con React que funciona como una SPA, es decir, una aplicación de una sola página. Su objetivo es permitir que un estudiante pueda revisar un catálogo de cursos, consultar el detalle de cada curso y gestionar una preinscripción académica agregando o quitando cursos seleccionados.

La aplicación fue desarrollada aplicando los contenidos relacionados con JSX, componentes funcionales, Hooks, React Router y Context API.

## Utilizamos:

* React
* JavaScript
* JSX
* React Router DOM
* Hooks: useState y useEffect
* Context API
* CSS
* Vite

## Funcionalidades principales

* Visualizar un catálogo de cursos.
* Consultar el detalle de cada curso.
* Navegar entre vistas sin recargar la página.
* Agregar cursos a una preinscripción.
* Evitar que se agreguen cursos duplicados.
* Quitar cursos seleccionados.
* Limpiar toda la preinscripción.
* Mostrar la cantidad de cursos seleccionados en el menú de navegación.
* Calcular el total de créditos de los cursos seleccionados.
* Mostrar una vista informativa sobre el proyecto.
* Simular la carga de cursos mediante useEffect.

Descripción de carpetas
* components

Contiene componentes reutilizables de la interfaz, como el menú de navegación, tarjetas de cursos, footer y elementos de cursos seleccionados.

* pages

Contiene las vistas principales de la aplicación: inicio, catálogo, detalle del curso, preinscripción y acerca del proyecto.

* routes

Contiene la configuración de rutas de la aplicación mediante React Router. Esto permite separar la navegación del archivo principal App.jsx.

* context

Contiene el contexto global del proyecto. En este caso, se utiliza CourseContext.jsx para manejar los cursos seleccionados por el estudiante.

* hooks

Contiene el hook personalizado useCourses, que permite consumir el contexto de cursos desde diferentes componentes de forma más ordenada.

* data

Contiene los datos mock locales de los cursos. Estos datos simulan la información académica sin necesidad de usar una base de datos o backend.

## Instalación del proyecto

Para instalar las dependencias del proyecto, ejecutar:

npm install

## Ejecución del proyecto

Para iniciar la aplicación en modo desarrollo, ejecutar:

npm run dev

Luego abrir en el navegador la URL que indique la terminal. Por ejemplo:

http://localhost:5173/

## Manejo de estado global

El proyecto utiliza **Context API** para manejar el estado global de la preinscripción. Esto permite que los cursos seleccionados puedan compartirse entre diferentes componentes, como el detalle del curso, la página de preinscripción y el menú de navegación.

El estado global permite:

* Agregar cursos.
* Evitar cursos duplicados.
* Quitar cursos seleccionados.
* Limpiar toda la preinscripción.
* Mostrar la cantidad de cursos seleccionados en el Navbar.

## Uso de Hooks

En el proyecto se utilizaron Hooks de React:

* `useState`: para manejar estados locales y el estado global de cursos seleccionados.
* `useEffect`: para simular la carga inicial del catálogo de cursos.
* `useParams`: para obtener el identificador del curso desde la URL dinámica.
* `useContext`: para consumir el contexto global mediante el hook personalizado useCourses

## Datos mock

La aplicación trabaja con datos mock locales almacenados en el archivo:

```txt
src/data/courses.js
```

Estos datos simulan la información de los cursos disponibles, incluyendo nombre, docente, categoría, modalidad, duración, créditos, horario y descripción.

## Componentes principales

* Navbar.jsx

Muestra el menú principal de navegación y la cantidad de cursos seleccionados.

* CourseCard.jsx

Muestra la información resumida de cada curso dentro del catálogo.

* SelectedCourseItem.jsx

Representa cada curso agregado a la preinscripción y permite quitarlo.

* Footer.jsx

Muestra información general del proyecto en la parte inferior de la aplicación.

## Vistas principales

* Inicio

Presenta el portal y permite acceder al catálogo de cursos.

* Catálogo de cursos

Muestra los cursos disponibles en forma de tarjetas.

* Detalle del curso

Muestra información completa de un curso seleccionado y permite agregarlo a la preinscripción.

* Mi preinscripción

Muestra los cursos seleccionados, la cantidad total de cursos y el total de créditos. También permite quitar cursos o limpiar toda la selección.

* Acerca del proyecto

Explica brevemente el objetivo, tecnologías y flujo principal de la aplicación.

## Capturas de pantalla

Las capturas principales del proyecto corresponden a:

* Página de inicio.
* Catálogo de cursos.
* Detalle de curso.
* Mi preinscripción.
* Acerca del proyecto.
* Prueba de errores

## Link de exposición en YouTube

```txt
https://youtu.be/mF_zdXTH1fA
```

## Conclusión

El Portal del Estudiante cumple con los requerimientos planteados para la PA3, ya que implementa una aplicación SPA en React con navegación entre vistas, componentes funcionales reutilizables, Hooks, React Router y manejo de estado global mediante Context API. Además, permite al estudiante consultar cursos, revisar detalles y gestionar su preinscripción de forma clara y funcional.
