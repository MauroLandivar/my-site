# 🌐 Mi Portfolio Personal — Mauro Landivar

Este repositorio contiene el sitio web de mi portfolio profesional, accesible en:

**👉 [www.landivarparada.com/profile](https://www.landivarparada.com/profile)**

---

## ¿Qué es esto?

Es mi sitio web personal como **Product Manager**. Muestra mi experiencia, proyectos, educación y cómo contactarme. El sitio fue diseñado originalmente en **Webflow** y ahora está hosteado aquí en **GitHub Pages** para poder editarlo directamente.

---

## ¿Cómo funciona?

Cuando hago un cambio en el código y lo subo a GitHub (`git push`), el sitio se actualiza automáticamente en minutos. No necesito hacer nada más.

El proceso es:
```
Edito el código → git push → GitHub lo despliega solo → el sitio se actualiza
```

---

## Estructura de carpetas

```
my-site/
│
├── profile/
│   └── index.html        ← El sitio web completo (todo está aquí)
│
├── index.html            ← Redirige automáticamente a /profile
│
├── CNAME                 ← Le dice a GitHub que use el dominio www.landivarparada.com
│
├── webflow               ← Copia del HTML original exportado de Webflow (respaldo)
│
├── .github/
│   └── workflows/
│       └── pages.yml     ← Instrucciones automáticas para publicar el sitio
│
└── README.md             ← Este archivo
```

---

## ¿Dónde están las imágenes?

Las imágenes **no están guardadas en este repositorio**. Se cargan directamente desde el servidor de Webflow (su CDN). Esto significa:

- Las imágenes están en internet, en una URL que empieza con:
  `https://cdn.prod.website-files.com/6717cb0608ec7a59c57ac7a5/`
- No ocupan espacio en este repositorio
- Se cargan rápido porque vienen de un servidor optimizado

Si en algún momento quiero cambiar una imagen, tengo que reemplazar la URL de esa imagen en el archivo `profile/index.html`.

---

## ¿Cómo edito el sitio?

Todo el contenido está dentro del archivo `profile/index.html`. Para hacer cambios:

1. Abro el archivo `profile/index.html`
2. Busco el texto o sección que quiero cambiar
3. Hago el cambio
4. Hago commit y push

Puedo hacer esto directamente desde este editor con Claude.

### Ejemplos de cosas fáciles de cambiar:
- **Mi nombre o título** → buscar "Mauro Landivar" en el HTML
- **Mi email o WhatsApp** → buscar "mauro@landivarparada.com" o "wa.me"
- **Texto de una sección** → buscar el texto exacto y editarlo
- **Un proyecto nuevo** → copiar el bloque HTML de un proyecto existente y cambiar la imagen y el texto

---

## Dominio personalizado

El sitio usa el dominio `www.landivarparada.com`, comprado en **Google Domains** (ahora Squarespace). El archivo `CNAME` conecta ese dominio con GitHub Pages.

---

## Tecnologías usadas

| Tecnología | Para qué sirve |
|---|---|
| HTML | La estructura de la página |
| CSS (Webflow) | Los estilos y diseño visual |
| JavaScript (Webflow) | Las animaciones e interacciones |
| GitHub Pages | Donde está hosteado el sitio (gratis) |
| GitHub Actions | Publica el sitio automáticamente en cada push |
