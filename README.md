# AgroAlertas ASPANU

Prototipo web de AgroAlertas, una aplicación para avisar a los productores agrícolas sobre alertas climáticas como lluvias fuertes, vientos y sequías.

Evidencia GA7-220501096-AA3-EV01. Codificación de módulos del software.

## Tecnologías

- React con Vite
- Bootstrap y React Bootstrap
- React Router para la navegación entre páginas
- Git y GitHub para el control de versiones

## Cómo ejecutar el proyecto

1. Instalar las librerías con el comando: npm install
2. Ejecutar el proyecto con el comando: npm run dev
3. Abrir en el navegador la dirección que aparece en la terminal, normalmente http://localhost:5173

Usuario de prueba: productor
Contraseña: 1234

## Estructura del proyecto

- assets: imágenes de la aplicación
- src/main.jsx: arranque de la app
- src/App.jsx: rutas de la app
- src/pages: una página por cada pantalla
- src/styles: estilos de la app
- index.html: página base donde se dibuja React

## Flujo de la aplicación

Inicio, luego Login, luego Selección de rol. Desde ahí cada rol va a su página:

- Agrónomo: crear alerta
- Gerencia: notificaciones por WhatsApp o SMS
- Productor: ver la alerta y el calendario

## Estándar de codificación

Estas son las reglas que se siguieron en todo el código.

### Nombres

- Componentes de React con la primera letra en mayúscula, por ejemplo Login, Registro, CrearAlerta.
- Variables y funciones en camelCase y en español, por ejemplo manejarEnvio, verPassword, mostrarError.
- Constantes con datos fijos en mayúscula, por ejemplo USUARIOS.
- Archivos de las páginas en minúscula con el mismo nombre del html original, por ejemplo login.jsx, crear-alerta.jsx.
- Clases de CSS en minúscula y separadas con guion, por ejemplo login-form-section, btn-submit.

### Formato

- Indentación de 2 espacios en los archivos jsx y de 4 espacios en el css.
- Comillas simples en JavaScript y comillas dobles en los atributos de JSX.
- Cada archivo termina con export default del componente.
- Las importaciones van al inicio del archivo: primero React, luego librerías y al final archivos propios.

### Organización

- Una página por archivo dentro de src/pages.
- Las rutas de todas las páginas están en App.jsx.
- Los estilos están en un solo archivo, src/styles/style.css, separados por secciones.
- Las imágenes están en la carpeta assets.

### Comentarios

- Cada página tiene un comentario arriba con el título en mayúscula y una línea que explica qué hace.
- Cada función tiene un comentario que explica para qué sirve.
- En el JSX se usan comentarios para separar las partes de la pantalla, como la barra de arriba, el formulario o las tarjetas.
- En el CSS cada sección empieza con un comentario con su nombre en mayúscula.

### Control de versiones

- El proyecto se maneja con Git y se sube a GitHub.
- La carpeta node_modules no se sube, está en el archivo .gitignore.
- Cada commit tiene un mensaje corto que dice qué se cambió.