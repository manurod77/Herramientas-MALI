# Sitio de herramientas bioclimáticas · MALI Módulo 3

Sitio estático: una portada y cuatro herramientas, todas en un solo archivo HTML cada una. No necesita compilación ni dependencias.

| Archivo | Qué es |
|---|---|
| `index.html` | Portada con el índice de las herramientas |
| `paquete-climatico.html` | Convierte un archivo EPW en el paquete climático de texto, con descarga en .md |
| `visualizador-solar.html` | Visualizador solar de vanos en tres dimensiones |
| `predimensionamiento-solar.html` | Paneles y terma solar, versión breve |
| `calculadora-solar.html` | Paneles y terma solar, versión completa, hora por hora |
| `generador-craft.html` | Generador de prompts CRAFT-PRO del Módulo 3 |
| `generador-craft-imagen.html` | Generador de prompts de visualización arquitectónica para ComfyUI |
| `plantilla-craft-herramientas.html` | El prompt con el que se construyó el visualizador, y su plantilla en blanco |
| `manual-visualizador.html` | Manual de uso del visualizador solar |
| `manual-sketchup.html` | Guía para conectar la IA con SketchUp |
| `guia-crear-herramientas.html` | Guía de método: cómo crear herramientas con asistencia de IA |

## Publicarlo en Vercel desde esta carpeta

Con la interfaz de línea de comandos de Vercel, parado en esta carpeta:

```
npx vercel --prod
```

La primera vez pide iniciar sesión en el navegador y confirmar el nombre del proyecto. Las siguientes veces, el mismo comando actualiza el sitio.

## Publicarlo con GitHub

1. Crea un repositorio vacío en GitHub, sin README.
2. Desde esta carpeta:

```
git init
git add .
git commit -m "Herramientas bioclimaticas MALI M3"
git branch -M main
git remote add origin https://github.com/<usuario>/<repositorio>.git
git push -u origin main
```

3. En Vercel, nuevo proyecto desde ese repositorio. Sin framework, sin comando de compilación: es un sitio estático.

Desde entonces, cada cambio que subas al repositorio se publica solo.

## Agregar una herramienta nueva

Copia su archivo HTML a esta carpeta y añade una tarjeta en `index.html`, duplicando un bloque `<a class="card">`. En la sección «En preparación» está la tarjeta de las herramientas de partículas de viento y lluvia, para reemplazarla cuando existan.

## Autoría

Ver `LICENCIA.md`. Las herramientas se entregan por enlace al sitio, no repartiendo los archivos.
