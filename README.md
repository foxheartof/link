# FoxHeart · Micrositio Meet & Greet

Micrositio **responsive** para GitHub Pages, con **exactamente dos enlaces de acción**:

1. **Más información** → https://foxheartof.github.io/
2. **Comprar boleto $800** → https://mpago.la/1xB6cLS

## Publicación en GitHub Pages

1. Crea un repositorio nuevo en GitHub, por ejemplo `foxheart-boletos` (no sobrescribas el repositorio original `foxheartof.github.io`).
2. Extrae este ZIP y sube **todos los archivos de la carpeta** a la raíz del nuevo repositorio. Debe quedar `index.html` en la raíz.
3. En **Settings → Pages**, selecciona **Deploy from a branch**, rama **main** y directorio **/(root)**. Guarda los cambios.
4. Abre la dirección que indique GitHub Pages (por ejemplo, `https://TU-USUARIO.github.io/foxheart-boletos/`).

No es necesario instalar Node, paquetes, frameworks ni servicios adicionales. También puedes abrir `index.html` directamente en el navegador para revisar el diseño.

## Estructura

```text
.
├── index.html         # Contenido y los dos enlaces
├── styles.css         # Diseño responsive
├── assets/
│   └── favicon.svg    # Ícono local, sin dependencias
├── .nojekyll           # GitHub Pages sirve los archivos tal cual
└── README.md          # Instrucciones de publicación
```

## Estilo y fotografía

Se reutiliza la paleta del sitio actual de FoxHeart (rosa `#ff7ca9`, dorado `#f0c541`, fondo oscuro `#120c11`). Para mantener la identidad original sin redistribuir archivos de terceros, la fotografía de fondo se carga desde `https://foxheartof.github.io/assets/hero-main.jpg`. Si el recurso no está disponible, el diseño muestra un fondo degradado local de respaldo. El resto del micrositio es completamente estático.

Para volverlo totalmente autónomo, copia una fotografía que tengas autorización de usar a `assets/hero-main.jpg` y sustituye la URL de la regla `.poster__visual` en `styles.css` por `url('assets/hero-main.jpg')`.

## Editar botones

En `index.html`, cambia las URL `href` de las dos etiquetas `<a>` dentro del bloque `nav.actions`. Los enlaces se abren en una pestaña nueva con `rel="noopener noreferrer"`.
