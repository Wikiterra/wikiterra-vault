---
dg-publish: false
---

# Markdown
Markdown es un lenguaje de marcado simple que permite formatear texto fácilmente en un editor de texto plano, utilizando una sintaxis mínima y fácil de leer.

El renderizado de Markdown se realiza con un motor de JavaScript que lo convierte en formato web, HTML para la estructura y CSS para los estilos. Y este formato web se muestra gracias a un navegador web.

> Obsidian es un Google Chrome "disfrazado", ya que utiliza electronJS un framework que combina chromium + nodeJS, para crear crear aplicaciones multiplataforma.

Algunos temas de Obsidian integran estilos especiales para formatos de Markdown, como infoboxes, grids, tarjetas. Un ejemplo es [ITS Theme Documentación](https://publish.obsidian.md/slrvb-docs/ITS+Theme/ITS+Theme) usado para esta wiki.

A continuación se cita la sintaxis básica de Markdown.

## Sintaxis de markdown

### Cabeceras
```
# Cabecera 1
## Cabecera 2
### Cabecera 3
#### Cabecera 4
##### Cabecera 5
###### Cabecera 6
```
# Cabecera 1
## Cabecera 2
### Cabecera 3
#### Cabecera 4
##### Cabecera 5
###### Cabecera 6

### Émfasis
*Este texto irá en cursiva*
Este texto también estará en cursiva

**Este texto estará en negrita
Este texto también estará en negrita.

==Este texto está subrayado==

```
*Este texto estará en cursiva*

Este texto también estará en cursiva

**Este texto estará en negrita

Este texto también estará en negrita.

==Este texto está subrayado==
```

### Listas
```
#### Desordenadas
* Item 1
* Item 2
  * Item 2a
  * Item 2b
#### Ordenadas
1. Item 1
2. Item 2
3. Item 3
   1. Item 3a
   2. Item 3b
```

#### Desordenadas
* Item 1
* Item 2
  * Item 2a
  * Item 2b
#### Ordenadas
1. Item 1
2. Item 2
3. Item 3
   1. Item 3a
   2. Item 3b

### Casillas de selección
```markdown
- [ ] Uncheckd
- [x] Checked
```

- [ ]  Uncheckd
- [x]  Checked

### Etiquetas / tags
Haz click en la etiqueta de abajo para ver el contenido en otras páginas con la misma etiqueta.
#etiqueta

### Notas de pie de página
```markdown
Este es un ejemplo de cómo agregar una nota al pie de página[^1].

[^1]: Aquí hay información extra en el pie de página
```

Este es un ejemplo de cómo agregar una nota al pie de página[^1].

[^1]: Este es el texto de la nota al pie.

---

### Archivos:

> [!warning] Para evitar sobrecargar la web, se recomienda utilizar archivos livianos y alojarlos en un servidor externo especializado para imágenes, como CDNs (Amazon CloudFront, Cloudflare CDN, Akamai), servicios en la nube con CDN integrado (Amazon S3, Google Cloud), o plataformas de alojamiento de imágenes (Imgur, Flickr).
>  El generador estático 11Ty se sobrecarga cuando tiene decenas de imágenes o archivos pesados, y además puede dar problemas con el servidor de sitios estático como GitHub Pages.

#### Documentos (.md, .html, .excalidraw, .pdf)
```markdown
![[formula]]  - Insertar documento completo

![[formula#Explanation]]  - Insertar cabecera del documento

![[formula#^eq]] - Insertar frase del documento
```

![[katex-formula]]

![[katex-formula#Explanation]]


![[katex-formula#^eq]]


#### Imágenes (.jpg, .png, .svg)
> [!warning] No es recomendable insertar imágenes directamente, para eso usar un CDN o servidor externo.
```markdown
 ![GitHub Logo|300](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

![[github-logo.png]]
```

![GitHub Logo|300](https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png)

#### Audios (mp3, .wav, .ogg)
> [!warning] No es recomendable insertar audio directamente, mejor usar fuentes externas.
```html
<audio controls>  
  <source src="../recursos/audio/flute.mp3" type="audio/mp3">
  audio not supported
</audio>

![[flute.mp3]]

<iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/1860933699"></iframe>
```

<iframe width="100%" height="166" scrolling="no" frameborder="no" allow="autoplay" src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/tracks/1860933699"></iframe>

#### Videos (.mp4, .webm)
> [!warning] No es recomendable insertar videos localmente, mejor enlazar a un video externo.
>
> Usando el generador estático HUGO, no se puede en MD es necesario usar HTML. 

> [!NOTE] 
> - **YouTube**: Para incrustar videos de YouTube, utiliza un `<iframe>` o una imagen de miniatura que enlace al video.
> - **Imgur**: Para videos alojados en Imgur, usa la etiqueta `<video>` con el enlace directo al archivo `.mp4`.
> - **Vimeo**: Para videos de Vimeo, utiliza un `<iframe>` con los parámetros adecuados en la URL para personalizar la visualización y controlar la reproducción.


```html
<!-- No recomendado para hacer una web estática -->
![[Bunny.mp4]]
<video src="../zen/audiovisual/Bunny.mp4" controls></video>

<!-- Se pueden usar estilos como: style="width:100%; aspect-ratio:16 / 9;" -->

<iframe width="500" height="315" src="https://www.youtube-nocookie.com/embed/1AeihtlrAkU?si=ZmtKlUeIU_LYpgSr"></iframe>

<a href="https://www.youtube.com/watch?v=1AeihtlrAkU" target="_blank">
  <img src="https://img.youtube.com/vi/1AeihtlrAkU/maxresdefault.jpg" alt="Ver video en YouTube" style="width:100%; max-width:560px;">
</a>

<iframe style="width:100%; aspect-ratio:16 / 10;" frameborder="0" allowfullscreen src="https://i.imgur.com/RLiDqCP.mp4" allowfullscreen></iframe>

<video style="width:100%; aspect-ratio:16 / 10;" controls>
  <source src="https://i.imgur.com/RLiDqCP.mp4" type="video/mp4">
  Tu navegador no soporta el formato de video.
</video>

<iframe src="https://player.vimeo.com/video/980152026" style="width:100%; aspect-ratio:16 / 10;"  allow="autoplay; fullscreen; picture-in-picture; clipboard-write" title="How to embed a video"></iframe>
```


<iframe width="500" height="315" src="https://www.youtube-nocookie.com/embed/1AeihtlrAkU?si=ZmtKlUeIU_LYpgSr"></iframe>

<a href="https://www.youtube.com/watch?v=1AeihtlrAkU" target="_blank">
  <img src="https://img.youtube.com/vi/1AeihtlrAkU/maxresdefault.jpg" alt="Ver video en YouTube" style="width:100%; max-width:560px;">
</a>

<video style="width:100%; aspect-ratio:16 / 10;" controls>
  <source src="https://i.imgur.com/RLiDqCP.mp4" type="video/mp4">
  Tu navegador no soporta el formato de video.
</video>

<iframe src="https://player.vimeo.com/video/980152026" style="width:100%; aspect-ratio:16 / 10;"  allow="autoplay; fullscreen; picture-in-picture; clipboard-write" title="How to embed a video"></iframe>

### Enlaces o links
```markdown
[[wikiterra]]
[[wikiterra#Objetivo]]
[[wikiterra#^intro1]]
[[wikiterra|WikiTerra - Una wiki de nuestro cosmos]]
[Hugo](https://gohugo.io)
```

[[index]]
[[index#Objetivo]]
[[index#^intro1]]
[[index|WikiTerra - Una wiki de nuestro cosmos]]
[Hugo](https://gohugo.io)

### Bloques de referencia
```markdown
> Si he visto más lejos es por estar de pie sobre hombros de Gigantes.
```

> Si he visto más allá es porque me he subido a hombros de gigantes.

### Código en línea
```markdown
El `código` en línea tiene `marcas de retroceso` a su alrededor.
```

El `código` en línea tiene `marcas de retroceso` a su alrededor.

### Bloques de código

\`\`\`go
func main() {
    fmt.Println("Hello World")
}
\`\`\`

```go
func main() {
    fmt.Println("Hello World")
}
```

### Tablas
```markdown
| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |
```

| Syntax    | Description |
| --------- | ----------- |
| Header    | Title       |
| Paragraph | Text        |

---

### Callouts
```
> [!NOTE] Título de la nota
> Información

> [!WARNING] Una advertencia
> Esto es una advertencia

> [!NOTE]+ Abrir por defecto
> Llamada plegable/colapsable

> [!FAQ]- Cerrado por defecto
> Llamada plegable/colapsable

> [!TIP] Llamadas anidadas
> Texto dentro del aviso
> > [!EXAMPLE] Llamada interna
> > Múltiples capas anidadas
> > [!TODO] Texto dentro del aviso
```
> [!NOTE] Título de la nota
> Información

> [!WARNING] Una advertencia
> Esto es una advertencia

> [!NOTE]+ Abrir por defecto
> Llamada plegable/colapsable

> [!FAQ]- Cerrado por defecto
> Llamada plegable/colapsable

> [!TIP] Llamadas anidadas
> Texto dentro del aviso
> > [!EXAMPLE] Llamada interna
> > Múltiples capas anidadas
> > [!TODO] Texto dentro del aviso

---

## Lenguajes de marcado soportados
Obsidian soporta de forma nativa la integración con Canvas (formato JSON), Excalidraw (formato JSON), KaTeX, Mermaid y PlantUML mediante convertidores en JavaScript y plugins especializados. Además con plugins se pueden usar otros como Graphviz, AsciiMath, Timeline, Chess, Dita.

### Canvas
> No está soportado, solo funciona visualizándolo desde Obsidian.
```md
![[mindmap-luz.canvas|mindmap-luz]]
```

### Excalidraw
```md
![[squares.excalidraw]]
```

### KaTEX (formulas matemáticas)
```latex
$$ E = mc^2 $$
```

$$ E = mc^2 $$

### Mermaid (diagramas)
```txt
``mermaid
	graph LR;
		A--> B
``

``mermaid
	gantt
		title Diagrama de Gannt
		dateFormat YYYY-MM-DD
		section Section
		A task           :a1, 2014.01-01, 30d
		Another task     :after a1, 20d
		section Another
		Task in sec      :2014.01-12, 12d
		another task     : 24d
``
```

```mermaid
	graph LR;
		A--> B
```

```mermaid
	gantt
		title A Gannt Diagram
		dateFormat YYYY-MM-DD
		section Section
		A task           :a1, 2014.01-01, 30d
		Another task     :after a1, 20d
		section Another
		Task in sec      :2014.01-12, 12d
		another task     : 24d
```
---

### PlantUML  (diagramas UML)
> Para renderizar PlantUML en Obsidian.md es necesario instalar el plugin PlantUML, sin embargo Digital garden si lo renderiza.
```plantuml
@startuml
Bob -> Alice : hello
@enduml
```


## References
- [Markdown Syntax](https://www.markdownguide.org/basic-syntax/)
- [Hugo Markdown](https://gohugo.io/content-management/formats/#markdown)
