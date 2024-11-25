---
# Deja el título vacío para usar el título del sitio configurado en params.yaml
title: ""
date: 2022-10-24
type: landing

sections:
  # Bloque de publicaciones
  - block: collection
    id: papers  # Identificador único para publicaciones
    content:
      title: "Publicaciones Destacadas"
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2

  # Bloque de biografía
  - block: resume-biography-3
    id: bio  # Identificador único para biografía
    content:
      username: admin
      text: "Me considero una persona curiosa que no puede quedarse con la duda. Siempre estoy muy interesado en los fenómenos sociales, el comportamiento humano y el funcionamiento de nuestras sociedades. Estas inquietudes las he plasmado en mi especialidad en comunicación política y en el diseño de campañas electorales.<br/><br/>
      
      En los últimos años, he complementado esta preparación con el análisis de datos y técnicas de investigación cuantitativas, lo que me ha permitido ampliar mi espectro de estudio y trabajo. Por ejemplo, he aplicado estos conocimientos al analizar la evolución de la pandemia de la COVID-19 en la Comunidad Valenciana.<br/><br/>
      
      Además, he podido aplicar mi conocimiento en Ciencia Política trabajando y coordinando varias campañas electorales a nivel local. También he desempeñado roles como asesor de grupo municipal y actualmente como concejal.<br/><br/>"
      button:
        text: "Descargar CV"
        url: uploads/mi-cv.pdf
    design:
      css_class: biography-section
---
