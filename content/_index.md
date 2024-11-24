---
# Deja el título vacío para usar el título del sitio configurado en params.yaml
title: ""
date: 2022-10-24
type: landing

design:
  # Espaciado predeterminado entre secciones
  spacing: "6rem"

sections:
  # Sección de biografía
  - block: resume-biography-3
    content:
      # Usuario del perfil a mostrar (carpeta dentro de `content/authors/`)
      username: admin
      text:
   <p style="font-size: 18px; line-height: 1.8; margin-bottom: 20px;">
        Me considero una persona curiosa que no puede quedarse con la duda. Siempre estoy muy interesado en los fenómenos sociales, el comportamiento humano y el funcionamiento de nuestras sociedades. Estas inquietudes las he plasmado en mi especialidad en comunicación política y en el diseño de campañas electorales.
      </p>
      <p style="font-size: 18px; line-height: 1.8; margin-bottom: 20px;">
        En los últimos años, he complementado esta preparación con el análisis de datos y técnicas de investigación cuantitativas, lo que me ha permitido ampliar mi espectro de estudio y trabajo. Por ejemplo, he aplicado estos conocimientos al analizar la evolución de la pandemia de la COVID-19 en la Comunidad Valenciana.
      </p>
      <p style="font-size: 18px; line-height: 1.8; margin-bottom: 20px;">
        Además, he podido aplicar mi conocimiento en Ciencia Política trabajando y coordinando varias campañas electorales a nivel local. También he desempeñado roles como asesor de grupo municipal y actualmente como concejal.
      </p>
      # Botón de acción debajo de la biografía
      button:
        text: "Descargar CV"
        url: uploads/mi-cv.pdf
    design:
      css_class: dark
      background:
        color: black
        image:
          # Imagen de fondo (sube el archivo a `assets/media/`)
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false

  # Sección de introducción
  - block: markdown
    content:
      title: "📚 Mi Investigación"
      subtitle: ""
      text: |-
        Este es un espacio para compartir mi misión. Soy un investigador dedicado a explorar las aplicaciones de la inteligencia artificial en diversos campos.

        Me encanta colaborar en proyectos innovadores. ¡Contáctame si deseas trabajar juntos! 😃
    design:
      columns: "1"

  # Sección de publicaciones destacadas
  - block: collection
    id: papers
    content:
      title: "Publicaciones Destacadas"
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  # Sección de publicaciones recientes
  - block: collection
    content:
      title: "Publicaciones Recientes"
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation

  # Sección de charlas recientes
  - block: collection
    id: talks
    content:
      title: "Charlas Recientes y Futuras"
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1

  # Sección de noticias
  - block: collection
    id: news
    content:
      title: "Noticias Recientes"
      subtitle: ""
      text: ""
      page_type: post
      count: 5
      filters:
        exclude_featured: false
      order: desc
    design:
      view: date-title-summary
      spacing:
        padding: [0, 0, 0, 0]

  # Sección de llamada a la acción
  - block: cta-card
    content:
      title: "👉 Construye tu propio sitio web académico"
      text: |-
        Este sitio está generado por Hugo Blox Builder, una herramienta gratuita y de código abierto.

        <a class="github-button" href="https://github.com/HugoBlox/hugo-blox-builder" data-color-scheme="no-preference: light; light: light; dark: dark;" data-icon="octicon-star" data-size="large" data-show-count="true" aria-label="Star HugoBlox/hugo-blox-builder on GitHub">Star</a>
      button:
        text: "Comienza Aquí"
        url: https://hugoblox.com/templates/
    design:
      card:
        css_class: "bg-primary-700"
---
