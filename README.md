# Conecta TI 2026 · Kit de inicio U2S05

Sitio de un evento ficticio de tecnología. El HTML ya está completo y la hoja de estilos ya tiene colores, tipografía y bordes. **Lo que falta es la maquetación responsiva**, y eso es lo que vas a construir en esta sesión.

## Estructura

```
conecta-ti/
├── index.html          <- NO necesitas modificarlo (salvo el paso 1 del tutorial)
├── css/
│   └── estilos.css     <- aquí trabajas, en el bloque 6 al final del archivo
├── capturas/           <- aquí guardas tus 3 capturas de evidencia
└── README.md           <- aquí respondes la bitácora (al final de este archivo)
```

## Cómo abrirlo

- **En Codespaces:** sube la carpeta a un repositorio nuevo llamado `u2s05-conecta-ti`, abre el Codespace y ejecuta en la terminal `php -S localhost:8000`. Abre el puerto 8000 en el navegador.
- **Sin Codespaces:** abre `index.html` directamente en Chrome o Edge. Funciona igual porque es HTML y CSS puro.

## Anchos de prueba (DevTools, modo dispositivo)

| Vista | Ancho | Nombre de la captura |
|---|---|---|
| Celular | 375 px | `capturas/movil-375.png` |
| Tableta | 768 px | `capturas/tableta-768.png` |
| Escritorio | 1280 px | `capturas/escritorio-1280.png` |

Para tomar captura de página completa en DevTools: `Ctrl + Shift + P` (en Mac `Cmd + Shift + P`), escribe `screenshot` y elige **Capture full size screenshot**.

## Bitácora (responde aquí, 2 a 4 líneas por pregunta)

1. **¿Por qué el sitio original se veía diminuto o con barra horizontal en el celular? Menciona las dos causas que corregiste.**

   El sitio se veía diminuto porque no estaba configurado correctamente para adaptarse al ancho de la pantalla del celular. Esto se corrigió agregando la etiqueta meta viewport en el HTML, para que el navegador utilizara el ancho real del dispositivo. La segunda causa era que algunos elementos tenían una distribución que no se adaptaba a pantallas pequeñas. Para solucionarlo, utilicé Flexbox, Grid y media queries, haciendo que los elementos cambiaran su distribución según el tamaño de la pantalla.

2. **¿En qué parte del sitio elegiste Flexbox y en cuál Grid? Explica el criterio que usaste (una dimensión vs. dos dimensiones).**

   Utilicé Flexbox en los bloques de horario, el menú principal y la lista de patrocinadores, porque necesitaba acomodar los elementos principalmente en una sola dirección, ya fuera en filas o columnas. En cambio, utilicé Grid en la agenda, la cuadrícula de ponentes y el pie de página, porque necesitaba organizar los elementos en filas y columnas. Mi criterio fue usar Flexbox para distribuir elementos en una dimensión y Grid para controlar su distribución en dos dimensiones.

3. **¿Qué hace exactamente `repeat(auto-fit, minmax(240px, 1fr))`? Explícalo como si se lo contaras a un compañero que faltó.**

   Esta instrucción de CSS permite crear columnas que se adaptan automáticamente al espacio disponible. repeat() repite las columnas; auto-fit intenta colocar tantas como quepan en el contenedor; minmax(240px, 1fr) indica que cada columna debe medir al menos 240 píxeles y que puede crecer para ocupar el espacio disponible. De esta manera, las tarjetas se acomodan automáticamente según el ancho de la pantalla, sin tener que definir manualmente el número de columnas para cada tamaño

4. **¿Qué fue lo que más te costó y cómo lo resolviste? (qué recurso usaste: tutorial, hoja de referencia, checklist de errores, laboratorio, un compañero)**

  Lo que más me costó fue comprender cómo distribuir los elementos para que la página se adaptara correctamente a los diferentes tamaños de pantalla. Lo resolví revisando el tutorial, utilizando las indicaciones de CSS y probando el diseño en distintos anchos de pantalla. También recibí apoyo para comprender cómo organizar los elementos con Flexbox y Grid y cómo utilizar las media queries para cambiar la distribución en celulares, tabletas y computadoras.

---
*Conecta TI 2026 es un evento ficticio creado con fines didácticos. Prof. Alonso · Tecnologías de Información*
