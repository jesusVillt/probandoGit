# Desarrollo de Servicios Web con Node.js

## Datos académicos

| Campo | Detalle |
|---|---|
| **Universidad** | Universidad Autónoma de Chihuahua |
| **Facultad** | Facultad de Ingeniería |
| **Carrera** | Ingeniería en Computación |
| **Materia** | Desarrollo De Aplicaciones Web |
| **Docente** | Ramirez Martinez Luis Antonio |
| **Actividad** | Desarrollo de Servicios Web con Node.js |
| **Alumno** | Jesús Manuel Villegas Terrazas |
| **Matrícula** | 385743 |
| **Fecha de entrega** | 04/09/2026 |

## Descripción
Esta practica consiste en la creación de un todo-list. Este todo-list nos permite
crear nuevas tareas, actualizar las tareas ya creadas, ver tareas y eliminar tareas.
Todo esto a traves de los metodos del protocolo http.

## Objetivo
El objetivo de esta actividad es aplicar los conocimientos teoricos que llevamos hasta el momento del curso para crear una api rest mock. Con esta se busca demostrar la forma en la que podemos usar el protocolo http para lograr procesar peticiones y enviar
respuestas.

## Tecnologías utilizadas
- Node.js: Entorno de ejecución para JavaScript en el servidor.
- JavaScript: Lenguaje de programación principal del proyecto.
- Express.js (v5.2.1): Framework web
- log4js: Librería utilizada para el registro de logs
- soap: Librería utilizada para la integración y consumo de servicios web basados en el protocolo SOAP.
- Jest: Herramienta y framework de pruebas unitarias (Desarrollo).
- ESLint: Herramienta de análisis estático para identificar errores y mantener un estilo de código limpio (Desarrollo).

## Requisitos previos
- Node.js (v18.0.0 o superior)
- npm (v9.0.0 o superior)


## Instalación
Clonar el repositorio del proyecto
*git clone <URL_DEL_REPOSITORIO>*

Navegar al directorio del proyecto
*cd <NOMBRE_DEL_REPOSITORIO>*

Instalar todas las dependencias 
*npm install*


## Ejecución
Para correr el servidor web y empezar a hacer realizar peticiones:
*npm run dev*

## Scripts / comandos disponibles
| Comando | Descripción |
|---|---|
| `npm run dev`  | incia el servidor en modo de desarrollo |
| `npm run test` | Ejecuta el set de pruebas unitarias     |
| `npm run lint` | Analiza todo el proyecto desde la raiz  |

## Funcionalidades / uso
*Crear una tarea con el metodo POST:* para crear una tarea por medio de este metodo
es necesario acceder a la ruta api/tasks/ y enviar un objeto JSON como el
siguiente: {"title": "Aqui el nombre de la tarea"}.

*Obtener todas las tareas con el método GET:* para obtener el listado completo de tareas registradas por medio de este método es necesario acceder a la ruta api/tasks/.

*Obtener una tarea específica con el método GET:* para consultar una tarea en particular por medio de este método es necesario acceder a la ruta api/tasks/:id (id es el identificador de la tarea que desea buscar).

*Actualizar una tarea con el método PUT:* para modificar una tarea existente por medio de este método es necesario acceder a la ruta api/tasks/:id enviando el identificador de la tarea a actualizar y un objeto JSON en el cuerpo con los datos a modificar.
Ejemplo: 
{
    "title": "Nuevo titulo de la tarea",
    "completed": "true"
}

*Eliminar una tarea con el método DELETE:* para remover una tarea del sistema por medio de este método es necesario acceder a la ruta api/tasks/:id especificando el identificador de la tarea que se desea borrar.

## Pruebas
Para realizar pruebas unitarias en esta practica se utilizo Jest.
Para correr estas pruebas ejecute:
*npm run test*
Las pruebas se aseguran de que lo siguiente se ejecute de manera correcta:
- Creación de una tarea
- Consulta de una tarea
- Modificación de una tarea
- Eliminación de una tarea


## Análisis de calidad de código
Para analizar la calidad del codigo en esta practica se utilzo EsLint.
Este analisis se realizará al ejecutar el siguente comando
*npm run lint*


## Estructura general del proyecto
```text
proyecto/
├── src/                  # Codigo fuente de la aplicación
├── tests/                # En esta carpeta se encuentran las pruebas
├── eslint.config.js      # En este archivo se encuentra la configuración del linter
├── package.json          # Dependencias y scripts del proyecto
├── package-lock.json     # Versiones exactas de dependencias
└── README.md             # Documentación del proyecto
```

## Autor
Jesus Manuel Villegas Terrazas — 385743
