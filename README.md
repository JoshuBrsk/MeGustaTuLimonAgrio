# Caso 3: LibroNet – Sistema de biblioteca
Cliente: Biblioteca Escolar San Martín · Prototipo: `index.html`

## Paso 1. Objetivo principal (5 min)
**Nombre del proyecto:** LibroNet

**Problema:** La biblioteca anota los préstamos en un cuaderno. Se pierden libros, no se sabe quién tiene cuál y las devoluciones atrasadas pasan sin control.

**Objetivo principal:** Desarrollar un sistema que administre el catálogo de libros, los socios y los préstamos y devoluciones.

**Objetivos específicos:**
1. Registrar libros con autor y ejemplares disponibles.
2. Registrar socios (estudiantes y docentes).
3. Registrar préstamos con fecha de devolución.
4. Registrar devoluciones y marcar atrasos.
5. Consultar libros disponibles.

**Alcance inicial:** Prototipo con 3 módulos (Libros, Socios, Préstamos). No incluye multas con pago, carnet con código QR ni biblioteca digital.

## Paso 2. Análisis funcional (10 min)
**Usuarios:** Bibliotecario (registra préstamos); Socio (estudiante o docente que consulta); Administrador (gestiona el catálogo).

**Necesidades principales:** Saber qué libros hay, quién tiene cada uno y cuándo debe devolverlo.

**Requisitos funcionales**
|Código|Requisito|
|---|---|
|RF-01|Registrar y listar libros con autor y ejemplares.|
|RF-02|Registrar y listar socios.|
|RF-03|Registrar un préstamo con fecha de devolución.|
|RF-04|Descontar un ejemplar disponible al prestar.|
|RF-05|Registrar la devolución de un libro.|
|RF-06|Marcar los préstamos atrasados.|
|RF-07|Buscar un libro por título o autor.|

**Requisitos no funcionales**
|Código|Requisito|
|---|---|
|RNF-01|Diseño responsive (celular, tablet y PC).|
|RNF-02|Rendimiento: cada pantalla carga en menos de 2 segundos.|
|RNF-03|Compatibilidad con Chrome, Edge y Firefox actuales.|
|RNF-04|Mantenibilidad: código separado en HTML, CSS y JavaScript.|
|RNF-05|Seguridad (versión real): acceso con usuario y contraseña.|
|RNF-06|Usabilidad: lenguaje simple para estudiantes y docentes.|

## Paso 3. Planificación (5 min)
|Integrante|Responsabilidad|
|---|---|
|1|Líder / coordinación|
|2|Análisis funcional|
|3|Requisitos y documentación|
|4|Diseño UI|
|5|Desarrollo|
|6|GitHub / integración y publicación|

*(Sustituir el número por el nombre real de cada integrante.)*

Calendario: **Análisis → Diseño → Desarrollo → Pruebas → Publicación**
|Etapa|Tiempo|Responsable|
|---|---|---|
|Análisis|15 min|Integrantes 2 y 3|
|Diseño|10 min|Integrantes 1 y 4|
|Desarrollo|15 min|Integrante 5|
|Pruebas|5 min|Integrantes 3 y 6|
|Publicación|5 min|Integrante 6|

## Paso 4. Diseño detallado (10 min)
**Arquitectura propuesta (sistema real):** cliente–servidor en 3 capas.
```
Navegador (HTML/CSS/JS)  →  API Web (C#)  →  Base de datos
```
**Tecnologías:** prototipo con HTML5, CSS3, JavaScript, Git y GitHub Pages; versión real con ASP.NET Core, Entity Framework Core, SQL Server.

**Módulos:** Libros, Socios, Préstamos.

**Navegación:** `[Inicio] [Libros] [Socios] [Préstamos]`

**Pantallas principales:**
- **Inicio:** banner, contadores por módulo y tabla reciente.
- **Libros:** tabla de datos y formulario para agregar registros.
- **Socios:** tabla de datos y formulario para agregar registros.
- **Préstamos:** tabla de datos y formulario para agregar registros.

## Paso 5. Ejecución (15 min)
Prototipo en `index.html`. Cumple el mínimo: página de inicio, menú, 3 módulos, datos ficticios, tablas, formularios y navegación. Hecho solo con HTML y CSS, una página por módulo, sin JavaScript ni base de datos.
Probar en Visual Studio Code con la extensión **Live Server** (clic derecho en `index.html` → *Open with Live Server*).

## Paso 6. Seguimiento y pruebas (5 min)
|Prueba|Resultado esperado|Estado|
|---|---|---|
|Navegar por todo el menú|Cada vista carga sin errores|☐|
|Abrir el formulario de cada módulo|El formulario se muestra completo|☐|
|Revisar los datos ficticios de cada módulo|Tablas con datos coherentes|☐|
|Abrir en celular|Se adapta a la pantalla|☐|
|Abrir la URL publicada|El prototipo carga desde GitHub Pages|☐|

## Paso 7. Aceptación (3 min)
**¿El prototipo demuestra la solución planteada?** Sí: muestra los módulos y el flujo principal del sistema con datos de ejemplo.

**Requisitos demostrables con el prototipo:**
1. RF-01: Registrar y listar libros con autor y ejemplares.
2. RF-02: Registrar y listar socios.
3. RF-03: Registrar un préstamo con fecha de devolución.
4. RF-06: Marcar los préstamos atrasados.
5. RNF-01: Diseño responsive (celular, tablet y PC).

## Paso 8. Cierre (2 min)
1. Subir el proyecto a GitHub.
2. Verificar que el repositorio esté actualizado.
3. Activar GitHub Pages (*Settings → Pages → Deploy from a branch → main / root*).
4. Presentar la URL: `https://TU-USUARIO.github.io/NOMBRE-REPO/`

## Paso 9. Mantenimiento (futuro)
Conectar base de datos real, agregar inicio de sesión por roles, reportes en PDF y notificaciones.
# MeGustaTuLimonAgrio
