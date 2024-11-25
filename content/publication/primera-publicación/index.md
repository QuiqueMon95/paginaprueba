---
title: "Mi Primera Publicación"
date: 2024-11-25
authors:
  - Quique Montero
summary: "Una breve descripción de mi primera publicación."
tags:
  - Ciencia Política
  - Análisis de Datos
categories:
  - Investigación
featured: true  # Establece en true si quieres que esta publicación sea destacada.

---
Aquí va el contenido principal de tu publicación. Puedes usar **Markdown** para agregar formato.
Estoy muy emocionado de compartir un nuevo proyecto en el que he estado trabajando. Este proyecto se enfoca en el análisis de datos espaciales y el comportamiento humano, aplicando lo aprendido en mis estudios de geografía física y ciencia política.

¡Espero que les guste!

<div style="text-align: center;">
  <img src="/assets/images/Rplot.png" alt="Mapa de orihuela" width="600" />
</div>

```r
ggplot() +
  geom_sf(data = c_ori_limp, aes(fill = categoria), col = NA) +
  scale_fill_manual(values = c(
    "1" = "#2b83ba",   
    "2" = "#abdda4" ,    
    "3" = "#fdae61" ,  
    "4" = "#d7191c" ),
    
    labels = c("1" = "Antes de 1960", 
               "2" = "1960-1979", 
               "3" = "1980-1999",
               "4" = "2000-actualidad"),
    name = "",
    na.translate = FALSE) +
  
  theme_minimal() +
  theme(     
    panel.background = element_rect(fill = "transparent",
                                    colour = NA_character_), 
    panel.grid.major = element_blank(), 
    panel.grid.minor = element_blank(), 
    plot.background = element_rect(fill = "transparent",
                                   colour = NA_character_), 
    legend.background = element_rect(fill = "transparent"),
    legend.box.background = element_rect(fill = "transparent"),
    legend.key = element_rect(fill = "transparent"),
    axis.text.x = element_blank(),
    axis.text.y = element_blank(),
    plot.title = element_blank(),
    plot.subtitle = element_blank(),
    plot.caption = element_blank(),
    axis.ticks.y = element_blank(),
 ```
