# Práctica: Creación y Publicación de Ontología (LOT4KG – Tarea 3)

En esta práctica vais a realizar la Tarea 3 (Ontology Modelling & Publishing) de la metodología \[LOT\]4KG. El objetivo es diseñar una ontología a partir de vuestro dominio/dataset y publicarla de forma accesible, con documentación, diagramas y artefactos reutilizables.

Herramientas obligatorias:
- Creación/modelado: Chowlk (https://chowlk.linkeddata.es/)
- Documentación + publicación: OnToology (https://ontoology.linkeddata.es/)  ￼



## Objetivo

A partir de vuestro dominio y del dataset ya preparado (o en paralelo), debéis:
1. Modelar la ontología con Chowlk (clases, propiedades y restricciones básicas).
2.	Exportar la ontología a RDF/OWL (recomendado: Turtle .ttl).
3.	Publicar y documentar la ontología con OnToology, de forma que:
	- se generen docs HTML, diagramas y un informe de evaluación,
	- quede disponible una forma de acceso web (p. ej., GitHub Pages / publicación con URL persistente si aplica).

⸻

## Requisitos y entrega

Debéis entregar en vuestra carpeta del repositorio (estructura recomendada):
- ontology/
	- modelo.png (export del diagrama)
	- ontology.ttl (obligatorio)
	- README.md
		- IRI base / namespace
		- alcance + preguntas de competencia
	 	- enlace(s) a la publicación/documentación resultante

## Flujo de trabajo

### 1) (OPCIONAL) Definición de alcance y preguntas de competencia

Antes de dibujar, dejad claro:
- Alcance: qué cubre y qué NO cubre vuestra ontología. Es decir:
- 5–10 preguntas de competencia (qué queréis poder responder con datos conformes a vuestra ontología).

📌 Podéis añadirlo en ontology/README.md.

⸻

### 2) Modelado con Chowlk (diagrama)

Usad Chowlk para crear el diagrama conceptual:
- Clases principales del dominio.
- Propiedades de objeto (relaciones entre entidades).
- Propiedades de datos (atributos literales).
- Dominios y rangos cuando tenga sentido.


Recomendación docente:
- Empezad por un “core” pequeño (3–6 clases) y ampliad.
- Nombres consistentes (p. ej., CamelCase para clases y camelCase para propiedades).

📌 Entregables: ontology/modelo.png

⸻

###  3) Exportación a RDF/OWL desde Chowlk


Checklist mínimo del TTL:
- Namespace/prefijos consistentes.
- Declaración owl:Ontology con metadatos:
	- dcterms:title
	- dcterms:description
	- dcterms:license
	- owl:versionInfo (o versión/IRI de versión si lo hacéis así)
- Etiquetas/descripciones en clases y propiedades (rdfs:label, rdfs:comment), al menos en los elementos principales.

📌 Entregable: ontology/ontology.ttl

⸻

### 4) Documentación y evaluación automática con OnToology

OnToology trabaja conectándose a vuestro repositorio de GitHub: monitoriza cambios, y cuando detecta cambios en ontologías, genera documentación/diagramas/evaluación y abre un Pull Request con los resultados.  ￼

1. Preparar el repositorio
- Subid al repo vuestro ontology/ontology.ttl (y el diagrama si corresponde).
- Aseguraos de que el fichero de ontología está en una ruta estable (para que OnToology lo detecte bien).

2. Registrar el repositorio en OnToology
	1.	Entrad en OnToology y registrad vuestro repositorio en formato usuario/repositorio.  ￼
	2.	Autorizad el acceso a GitHub cuando lo solicite (redirección a GitHub).  ￼
	3.	Seguid las indicaciones de la presentación de clase para generar la documentación.

3. Ontoology, genera, típicamente:
- Documentación HTML (basada en Widoco),
- diagramas (p. ej., AR2DTool: diagrama de clases / taxonomía),
- informe de evaluación (p. ej., OOPS!),
- otros artefactos (p. ej., contexto JSON-LD), según configuración.  ￼

4. Pull Request y carpeta de salida
- OnToology creará un Pull Request en vuestro repo con una carpeta OnToology/ que contiene los resultados.  ￼
- Debéis revisar los outputs y hacer merge del PR.

📌 Entregables:
- El PR con la carpeta OnToology/, muévelo a la carpeta de tu equipo (ontology/documentacion/).

⸻

### 5) Publicación web 

El objetivo es que la documentación se pueda visitar en un navegador. Vamos a activar GitHub Pages para crear un servidor de web estáticas en tu repositorio. Sigue las instrucciones descritas en la presentación de clase. 
 ￼

📌 Entregable: en ontology/README.md, poned:
	- URL pública donde se ve la documentación,



