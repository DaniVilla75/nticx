# 🚀 NTICX 4° Año — Lanzador de Módulos

Sitio web interactivo desarrollado para la materia **NTICX (Nuevas Tecnologías de la Información y la Conectividad)**, 4° año de Educación Secundaria. Funciona como portal de acceso centralizado a los distintos módulos de la materia, con una interfaz moderna estilo "dashboard tecnológico".

🔗 **[Ver sitio en vivo](https://danivilla75.github.io/NOMBRE-DEL-REPO/)** *(actualizar con la URL real de GitHub Pages)*

---

## 📋 Descripción

El **Lanzador de Módulos** es la página de inicio (`index.html`) desde la cual los estudiantes acceden a cada unidad temática de la materia. Cada módulo se presenta como una tarjeta interactiva con ícono, título, descripción breve y un botón de acceso animado.

Incluye además una **sección destacada** (Portal ProfeDani) con un diseño diferenciado (paleta cálida naranja) que enlaza a recursos educativos adicionales externos.

---

## 🗂️ Estructura de módulos

| # | Módulo | Estado | Archivo |
|---|--------|--------|---------|
| 1 | Alfabetización informática-computacional | 🔜 Próximamente | `#modulo1` |
| 2 | Alfabetización en redes digitales de información | ✅ Disponible | `modulo2.html` |
| 3 | Alfabetización en manejo de la información | ✅ Disponible | `modulo3.html` |
| 4 | Alfabetización en manejo de componentes de imagen visual | 🔜 Próximamente | `#modulo4` |
| 5 | Alfabetización en medios digitales de comunicación y colaboración | 🔜 Próximamente | `#modulo5` |
| 6 | Alfabetización multimedia | 🔜 Próximamente | `#modulo6` |
| 7 | Ciudadanía digital | 🔜 Próximamente | `#modulo7` |

> Los módulos marcados como "Próximamente" muestran un mensaje informativo al hacer clic, hasta que se suban sus respectivos archivos HTML.

### Material complementario
- `wifi_conectividad_argentina.html` — Material sobre WiFi, routers, seguridad, ancho de banda y servicios de Internet en Argentina (enlazado desde el Módulo 3, pestaña "WIFI").

---

## ✨ Características técnicas

- **100% HTML/CSS/JS estático** — no requiere backend ni instalación, ideal para GitHub Pages.
- **Diseño responsivo** (mobile-first) con grid adaptable de tarjetas.
- **Generación dinámica de tarjetas** desde un array de datos en JavaScript (`modulesData`), lo que facilita agregar o editar módulos sin tocar el HTML.
- **Modal de carga animado** al acceder a cada módulo, con mensajes personalizados por módulo.
- **Efectos visuales**: fondo con textura de ruido sutil, grilla tecnológica, animaciones de entrada (`fadeUp`), efectos hover con brillo y barra de progreso por tarjeta.
- Tipografías: [Inter](https://fonts.google.com/specimen/Inter) y [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) (Google Fonts).
- Iconografía: [Font Awesome 6](https://fontawesome.com/).

---

## 🛠️ Cómo agregar un nuevo módulo

Para activar un módulo que esté "Próximamente", basta con editar el array `modulesData` dentro de `index.html`:

```javascript
{
  id: 1,
  title: "Módulo 1 · Alfabetización informática-computacional",
  shortDesc: "Hardware, software, sistemas operativos y pensamiento computacional.",
  icon: "fas fa-laptop-code",
  color: "#2a6f9c",
  link: "modulo1.html"   // ← cambiar de "#modulo1" al archivo real
}
```

1. Subí el archivo `moduloX.html` a la raíz del repositorio (misma carpeta que `index.html`).
2. Cambiá el campo `link` del módulo correspondiente, apuntando al nombre exacto del archivo.
3. (Opcional) Personalizá el mensaje de carga en `customMessages` dentro de la función `launchModule()`.

---

## 📂 Estructura de archivos sugerida

```
/
├── index.html                          # Lanzador principal (este archivo)
├── modulo2.html                        # Módulo 2 - Redes digitales
├── modulo3.html                        # Módulo 3 - Manejo de la información
├── wifi_conectividad_argentina.html    # Material complementario WiFi
└── README.md                           # Este documento
```

---

## 🚀 Publicar en GitHub Pages

1. Subí todos los archivos `.html` a la rama `main` del repositorio.
2. En **Settings → Pages**, seleccioná la rama `main` y la carpeta `/ (root)`.
3. GitHub generará una URL del tipo `https://usuario.github.io/repositorio/`.
4. Esa URL abrirá automáticamente `index.html` como página de inicio.

---

## 👨‍🏫 Autor

**Prof. Daniel Villarruel**
NTICX · 4° Año · Educación Secundaria

Portal de recursos adicionales: [ProfeDani](https://danivilla75.github.io/ProfeDani/)

---

## 📄 Licencia

© 2026 — Todos los derechos reservados. Material educativo de uso áulico.
