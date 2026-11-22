# Documentación del proceso con IA — El Progreso

Proyecto final · Electiva 1: Herramientas de IA para la Transformación Digital

## A. Prompts de desarrollo (ingeniería de prompts)

Cada prompt sigue la estructura **Rol → Contexto → Tarea → Formato → Restricciones**.

| # | Propósito | Prompt |
|---|-----------|--------|
| 1 | Conceptualizar el emprendimiento y entrevistar al usuario | "Actúa como consultor de emprendimiento y desarrollador web. Quiero crear la página del Minimercado y Distribuidora El Progreso (Bogotá). Hazme una entrevista corta, una pregunta a la vez, para definir: enfoque del negocio (venta al detal), público, productos, funcionalidades de la página, tono de marca y datos de contacto. Al final resume todo en una estructura de página." |
| 2 | Definir identidad y funcionalidades | "Quiero un diseño llamativo pero organizado con verde y negro para títulos y naranja para resaltar. Tono tradicional de barrio con un toque de clase. Lema: 'Todo lo que necesitas está a la vuelta de tu casa'. Secciones: pasillo virtual por categoría, favoritos con precios (x1, x2, x3), promociones con código de descuento, horarios, dirección, teléfono y footer con Instagram, WhatsApp y Términos." |
| 3 | Generar el código de la página (Canvas activo) | "Generame el código de la página en un solo archivo HTML autocontenido (HTML, CSS y JavaScript puro) con LocalStorage para carrito, código PROGRESO10 (10%) y registro de pedidos, que genere el mensaje de la lista de mercado para WhatsApp (3023596524). Prepara la estructura para conectarla luego a Firebase. Entrégalo como archivo descargable." |
| 4 | Plan de trabajo en Notion según la rúbrica | "Con esta rúbrica del profesor (Kanban de 4 columnas con 8+ tareas, CRM con 10+ clientes ficticios, calendario con 6+ eventos, página principal con navegación), adapta mi workspace de Notion del Minimercado El Progreso con datos realistas y coherentes con el negocio." |
| 5 | Crear imágenes y moodboard (ver sección B) | Ver prompts B1–B8. |
| 6 | Preparar el repositorio y el historial de commits | "Dame los comandos de Git para subir el proyecto a GitHub con commits pequeños y descriptivos (Conventional Commits) y publicarlo con GitHub Pages." |
| 7 | Revisar y mejorar la página | "Revisa este index.html: valida el flujo de compra (carrito, cupón, mensaje de WhatsApp), accesibilidad y vista móvil, y dime qué corregir." |

## B. Prompts para imágenes con IA

Usa la herramienta de generación de imágenes vista en clase. Guarda cada resultado con el **nombre de archivo indicado** dentro de la carpeta `img/` y la página los mostrará automáticamente. Para la entrega, captura pantalla de cada generación junto con su prompt.

Estilo común a todas: *fotografía cálida y natural, luz de mañana, paleta verde profundo, negro y naranja cálido, ambiente de tienda de barrio colombiana con toque de clase*.

| # | Archivo | Prompt |
|---|---------|--------|
| B1 | `logo.png` | "Logotipo para 'El Progreso', minimercado y distribuidora de barrio en Bogotá. Monograma 'EP' con una canasta de frutas simplificada, estilo plano moderno con aire tradicional, colores verde profundo (#166534), negro y un acento naranja, fondo blanco, sin degradados, vectorial, legible en tamaño pequeño." |
| B2 | `hero.jpg` | "Fachada de un minimercado de barrio colombiano al amanecer, cajones de frutas frescas en la entrada, letrero verde con el nombre 'El Progreso', gente saludando con amabilidad, fotografía cálida, luz natural, composición horizontal 16:9." |
| B3 | `canasta-frutas.jpg` | "Canasta de mimbre con frutas campesinas colombianas frescas (mango, banano, mandarina, guayaba, tomate de árbol) sobre mesa de madera, luz natural suave, fondo verde difuminado, fotografía de producto, formato 4:3." |
| B4 | `huevos.jpg` | "Cubeta de 30 huevos criollos de granja sobre una mesa de madera rústica con paja, luz de mañana, fotografía de producto, formato 4:3." |
| B5 | `leche.jpg` | "Jarra y vaso de leche entera fresca sobre mesa de cocina de barrio, luz natural, estilo fotográfico limpio, formato 4:3." |
| B6 | `arroz.jpg` | "Bolsa de arroz blanco y granos de arroz en un cuenco de barro sobre madera, luz cálida, fotografía de producto, formato 4:3." |
| B7 | `aguardiente.jpg` | "Botella de aguardiente transparente y un vaso pequeño sobre una mesa de madera oscura, fondo oscuro con destellos naranja, fotografía de producto elegante, formato 4:3. Sin marcas reales." |
| B8 | `cerveza.jpg` | "Tres botellas de cerveza heladas con gotas de agua sobre hielo, fondo oscuro con luz naranja, fotografía de producto, formato 4:3. Sin marcas reales." |

> Consejo: pide "sin texto ni marcas reales" para evitar logos ajenos y letras deformadas.

## C. Prompt del moodboard

| Archivo | Prompt |
|---------|--------|
| `moodboard.jpg` | "Moodboard para la marca 'El Progreso', minimercado y distribuidora de barrio en Bogotá. Collage ordenado en cuadrícula con: frutas campesinas frescas, canasta de mimbre, fachada de tienda de barrio, tendero sonriendo, estantes con abarrotes, madera cálida, tipografía serif elegante en negro, paleta verde profundo (#166534), negro (#111111), naranja (#F2800F) y crema (#FBF6EA). Sensación: tradicional, cercano, fresco, con un toque de clase. Formato horizontal 16:9." |

**Paleta y tipografía de la marca**

| Elemento | Valor |
|----------|-------|
| Verde | #166534 |
| Negro | #111111 |
| Naranja (resaltes) | #F2800F |
| Crema (fondo) | #FBF6EA |
| Títulos | Fraunces (serif) |
| Texto | Nunito (sans) |
