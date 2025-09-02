# TravesIA — Public overview

Este repositorio es una **presentación** del proyecto (capturas, resumen y contacto).  
El **código fuente completo** está en un repositorio **privado** y se comparte **bajo solicitud**.

---

## Índice
1. [Qué es](#qué-es)
2. [Tecnologías y arquitectura (alto nivel)](#tecnologías-y-arquitectura-alto-nivel)
3. [Login](#login)
4. [Crear mi ruta](#crear-mi-ruta)
5. [Subir mis rutas](#subir-mis-rutas)
6. [Todos mis proyectos](#todos-mis-proyectos)
7. [Ver Mapa](#ver-mapa)
8. [Demo en vídeo](#demo-en-vídeo)
9. [Capturas](#capturas)
10. [Solicitar acceso al código](#solicitar-acceso-al-código)
11. [Autor y contacto](#autor-y-contacto)
12. [Aviso](#aviso)

---

## Qué es
**TravesIA** es un asistente para planificar travesías de montaña.  
Combina mapa interactivo, gestión de tracks y puntos de interés, y un planificador asistido por IA para proponer itinerarios según días, dificultad y preferencias.

---

## Tecnologías y arquitectura (alto nivel)
- **Frontend**: aplicación SPA con React, diseño responsive.
- **Backend**: API en Python (framework moderno para APIs REST).
- **Autenticación**: JWT.
- **Mapas / Geo**: librerías de visualización y datos abiertos.
- **Base de datos**: relacional.
- **Integraciones**: proveedor LLM para asistencia en la planificación.

> Se mantiene el detalle a alto nivel para no exponer decisiones internas. La implementación completa reside en un repositorio privado.

---

## Login
**Objetivo:** acceso seguro a las funciones personales (rutas, proyectos, opiniones).

**Qué muestra**
- Formulario con campos **Email o usuario** y **Contraseña**.
- Enlace **“Crear una nueva cuenta”** que abre el formulario de alta.
- Mensajes claros de validación/errores.

**Acciones clave**
- Iniciar sesión y crear sesión segura.
- Crear cuenta nueva desde el enlace de registro.
- Redirección a la pantalla principal con el menú lateral tras autenticar.

**Notas**
- Datos minimizados y protegidos (HTTPS, tokens de corta vida y refresco).
- En este repo público no se exponen endpoints ni credenciales.

**Capturas**

<p align="center">
  <img src="assets/login_1.png" alt="Figura 1 — Pantalla de inicio de sesión (Login) — TravesIA" width="840"><br/>
  <sub><b>Figura 1.</b> Pantalla de inicio de sesión</sub>
</p>

<p align="center">
  <img src="assets/login_2.png" alt="Figura 2 — Formulario de alta de nueva cuenta — TravesIA" width="840"><br/>
  <sub><b>Figura 2.</b> Formulario de alta de nueva cuenta</sub>
</p>


---

## Crear mi ruta
**Objetivo:** asistente para definir una travesía con parámetros de usuario.

**Qué muestra**
- Formulario guiado: días, tipo de ruta (lineal/circular), destino, puntos intermedios, nivel de dificultad, pernocta prevista.
- Vista previa de resultados y estimaciones.

**Acciones clave**
- Generar una propuesta inicial asistida por IA.
- Ajustar parámetros y volver a calcular.
- Guardar borrador como proyecto.

**Resultados**
- Resumen de la propuesta (distancia, desnivel, puntos clave).
- En versiones avanzadas: exportación a GPX/PDF (opción prevista en roadmap).

**Captura sugerida**
- `assets/crear-mi-ruta.png`

---

## Subir mis rutas
**Objetivo:** subir y gestionar archivos GPX del usuario.

**Qué muestra**
- Selector de archivos con validaciones básicas (extensión GPX, tamaño).
- Lista de rutas subidas con fecha y estado de procesado.

**Acciones clave**
- Subir, renombrar y eliminar rutas.
- Ver detalles de cada ruta: distancia y puntos clave detectados.

**Notas**
- Se evita exponer metadatos sensibles en el repo público.
- Procesado del GPX para obtener estadísticas básicas y puntos de interés.

**Captura sugerida**
- `assets/subir-mis-rutas.png`

---

## Todos mis proyectos
**Objetivo:** gestión de proyectos de planificación guardados por el usuario.

**Qué muestra**
- Listado con estado (borrador, en revisión, confirmado).
- Filtros por fecha, zona, días y dificultad.

**Acciones clave**
- Abrir un proyecto para editarlo.
- Duplicar como base para una nueva propuesta.
- Eliminar un proyecto.

**Resultados**
- Registro de decisiones y parámetros usados.
- Historial mínimo para trazabilidad.

**Captura sugerida**
- `assets/todos-mis-proyectos.png`

---

## Ver Mapa
**Objetivo:** explorar el mapa con tracks, waypoints y capas temáticas.

**Qué muestra**
- Mapa interactivo con capas de:
  - Tracks del usuario.
  - Waypoints (refugios, picos, puntos de agua, posibles zonas de vivac).
- Panel lateral con información del elemento seleccionado.

**Acciones clave**
- Activar/desactivar capas.
- Seleccionar elementos para ver detalles.
- Enlazar un elemento del mapa como punto de la planificación.

**Notas**
- Se usan datos abiertos y fuentes cartográficas compatibles.
- En futuras versiones: soporte offline y caché de teselas (PWA).

**Captura sugerida**
- `assets/ver-mapa.png`

---

## Demo en vídeo
Enlace (no listado): añade aquí tu URL de YouTube o Drive.

---

## Capturas
Coloca las imágenes en `assets/` y referencia los nombres anteriores:
- `assets/login.png`
- `assets/crear-mi-ruta.png`
- `assets/subir-mis-rutas.png`
- `assets/todos-mis-proyectos.png`
- `assets/ver-mapa.png`

Ejemplo de inserción en el README:
```markdown
![Login](assets/login.png)

## Demo en vídeo
Enlace (no listado): _añade aquí tu URL de YouTube/Drive_

## Solicitar acceso al código
El repositorio con el **código** es **privado**.  
Si te interesa revisarlo (recruiters, profesorado o colaboradores), escribe a **gescoi.san@gmail.com** indicando el motivo.  
También puedes abrir una *issue* titulada “Access request”.

## Autor
**Guillem Sánchez**  
Email: **gescoi.san@gmail.com** · GitHub: **guisantes1**

## Aviso
Este repositorio público contiene material informativo (texto, capturas).  
El **código fuente** no se publica aquí.  
© 2025 Guillem Sánchez. Todos los derechos reservados.
