# SPEC-000 — Foundation

## Propósito

Establecer la base técnica y las convenciones iniciales de **TaskFlow Lite**, definiendo su estructura, restricciones y reglas de trabajo para permitir un desarrollo incremental, simple y consistente.

## Estructura inicial del proyecto

El código fuente del proyecto se organizará dentro de `src/`.

```text
TaskFlow-Lite/
├── src/
│   ├── index.html
│   ├── css/
│   └── js/
├── .gitignore
└── README.md
```

La estructura inicial únicamente establece la organización del proyecto. No se implementarán todavía funcionalidades relacionadas con la gestión de tareas.

## Restricciones técnicas

* Utilizar **HTML5** para la estructura de las páginas.
* Utilizar **CSS3** para los estilos de la interfaz.
* Utilizar **JavaScript ES Modules** para la lógica del lado del cliente.
* No utilizar frameworks o librerías de frontend.
* No utilizar backend, APIs propias ni bases de datos externas.
* La persistencia de datos se realizará posteriormente mediante **localStorage**.
* El proyecto deberá poder ejecutarse localmente desde **VSCode**.
* El código fuente deberá mantenerse dentro de `src/`.
* En esta etapa no se implementarán historias funcionales.

## Convenciones de nombres

* Carpetas: `kebab-case`.
* Archivos HTML, CSS y JavaScript: `kebab-case`.
* Variables y funciones de JavaScript: `camelCase`.
* Constantes: `UPPER_SNAKE_CASE` únicamente cuando represente un valor constante global.
* Clases CSS: `kebab-case`.
* Los nombres deberán describir claramente la responsabilidad del elemento.

## Convenciones de Git

* Utilizar Git para el control de versiones.
* Cada commit deberá representar un cambio pequeño y relacionado con una sola intención.
* Utilizar mensajes de commit en formato:

```text
tipo: descripción breve
```

* Tipos permitidos inicialmente:

  * `feat`: nueva funcionalidad.
  * `fix`: corrección de errores.
  * `docs`: documentación.
  * `refactor`: reorganización interna sin cambio funcional.
  * `chore`: mantenimiento o configuración.

* No incluir archivos generados, temporales o dependencias innecesarias en el repositorio.

## Definition of Done técnica inicial

La foundation se considera terminada cuando:

* La estructura inicial del proyecto existe dentro de `src/`.
* Las tecnologías definidas para el proyecto están establecidas y no se utilizan frameworks.
* Las convenciones de nombres y Git están documentadas.
* El proyecto puede abrirse y ejecutarse localmente desde VSCode.
* No existen historias ni funcionalidades de negocio implementadas en esta etapa.

## Fuera de alcance

Quedan fuera del alcance de esta SPEC:

* Registro de tareas.
* Visualización de tareas.
* Actualización de estados.
* Edición o eliminación de tareas.
* Búsqueda, filtros u ordenamiento.
* Persistencia funcional mediante `localStorage`.
* Backend o API.
* Autenticación y gestión de usuarios.
* Diseño funcional de las pantallas.
* Implementación de historias de usuario.
