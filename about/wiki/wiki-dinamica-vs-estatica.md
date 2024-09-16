---
dg-publish: false
---

# Wiki dinámica vs Wiki estática

Comparar una wiki dinámica hecha con MediaWiki versus una wiki estática escrita y generada desde Obsidian.md implica evaluar varios factores, como la facilidad de uso, la administración, las características, el rendimiento y los costos. Aquí te dejo un desglose de los pros y contras de cada opción:

### Wiki dinámica escrita desde MediaWiki

**Pros:**
1. **Funcionalidad rica:** MediaWiki ofrece una amplia gama de funcionalidades integradas, como historial de revisiones, control de acceso, extensiones y plugins, plantillas, y más.
2. **Colaboración en tiempo real:** Permite a múltiples usuarios editar y colaborar en tiempo real, lo que es ideal para proyectos comunitarios o empresariales.
3. **Historial de cambios:** Proporciona un historial detallado de cambios con la capacidad de revertir a versiones anteriores, lo cual es útil para seguimiento y auditoría.
4. **Control de acceso y permisos:** Ofrece herramientas avanzadas para gestionar permisos y roles de usuario, garantizando la seguridad y el control sobre el contenido.
5. **Extensibilidad:** Hay una gran cantidad de extensiones disponibles que pueden añadir funcionalidad adicional según las necesidades específicas.

**Contras:**
1. **Complejidad en la instalación y administración:** Requiere conocimientos técnicos para instalar, configurar y mantener el servidor, incluyendo la gestión de bases de datos, actualizaciones y seguridad.
2. **Costo del servidor:** Puede implicar costos adicionales por el hosting del servidor, especialmente si se requiere un servidor de alto rendimiento para manejar un gran volumen de tráfico.
3. **Curva de aprendizaje:** Puede ser complicado para usuarios no técnicos aprender a utilizar y administrar MediaWiki de manera efectiva.
4. Diseñado para ser editado a través de su interfaz web

### Wiki estática escrita desde Obsidian.md + plugin Obsidian Digital Garden

**Pros:**
1. **Facilidad de uso:** Obsidian.md es fácil de usar con una interfaz intuitiva y amigable, ideal para usuarios individuales o pequeños equipos.
2. **Despliegue sencillo:** Desplegar la wiki en GitHub Pages es relativamente sencillo y gratuito, lo que elimina la necesidad de gestionar un servidor.
3. **Rendimiento:** Las páginas estáticas suelen ser más rápidas de cargar y menos susceptibles a problemas de rendimiento bajo alta carga.
4. **Seguridad:** Al ser estática, hay menos vectores de ataque comparado con aplicaciones web dinámicas, lo que mejora la seguridad.
5. **Portabilidad:** Los archivos markdown son fácilmente portables y pueden ser editados con cualquier editor de texto.

**Contras:**
1. **Funcionalidad limitada:** Las wikis estáticas tienen funcionalidades limitadas en comparación con MediaWiki, como la falta de edición colaborativa en tiempo real y control avanzado de acceso.
2. **Actualizaciones manuales:** Cada vez que se realiza un cambio, es necesario regenerar y desplegar el sitio estático, lo que puede ser un proceso manual si no está automatizado correctamente.
3. **Falta de historial de cambios:** A menos que se utilice control de versiones (como Git), no hay un historial detallado de cambios ni la capacidad de revertir a versiones anteriores fácilmente.
4. **Limitaciones de contenido dinámico:** Implementar funcionalidades dinámicas (como formularios o búsquedas avanzadas) es más complicado y puede requerir soluciones adicionales.

### Conclusión
La elección entre MediaWiki y una wiki estática en Obsidian.md depende de las necesidades específicas del proyecto. Si se requiere colaboración en tiempo real, funcionalidades avanzadas y control detallado de acceso, MediaWiki es la mejor opción. Sin embargo, si se busca una solución simple, fácil de desplegar y mantener, con menos necesidades de funcionalidades avanzadas, una wiki estática con Obsidian.md y Obsidian Digital Garden puede ser más adecuada.