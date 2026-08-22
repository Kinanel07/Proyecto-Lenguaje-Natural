# Análisis de Sentimiento en Reseñas de E-commerce

**Equipo Cienciahub**

Modelo de análisis de sentimiento sobre reseñas de productos de comercio electrónico, construido a partir del corpus *Amazon Fine Food Reviews*.

![Python](https://img.shields.io/badge/Python-3.10+-blue)
![Licencia de datos](https://img.shields.io/badge/datos-CC0-lightgrey)

---

## Descripción

Este repositorio contiene el desarrollo completo de un *pipeline* de procesamiento de lenguaje natural para clasificar la polaridad del sentimiento expresado en reseñas de productos publicadas por usuarios de Amazon.

El proyecto responde a una necesidad concreta del sector importador: una compañía que decide qué productos traer al mercado dispone en las reseñas públicas de un volumen de opinión imposible de procesar manualmente. Automatizar su lectura permite identificar las características más valoradas por los consumidores, detectar inconformidades recurrentes y reconocer los factores que inciden en la decisión de compra.

El impacto esperado es doble: **reducir el riesgo** de importar artículos con problemas sistemáticos y **orientar la construcción del portafolio** conforme a las necesidades reales del mercado, transformando opiniones dispersas de clientes en información accionable para la inversión.

---

## Ficha del proyecto

| Campo | Valor |
|---|---|
| **Nombre del equipo** | Cienciahub |
| **Área temática** | Empresarial |
| **Dominio específico** | E-commerce |
| **Pregunta NLP central** | Implementar un modelo de análisis de sentimiento basado en reseñas de productos de e-commerce |
| **Tarea NLP principal** | Pipeline de limpieza, preparación y modelado para clasificación de sentimiento |
| **Fuente de datos** | Amazon Fine Food Reviews (SNAP / Kaggle) |
| **Volumen** | ~568 000 registros (~280 MB) |
| **Herramientas** | Pandas, NumPy, Scikit-learn, NLTK |

---

## Datos

**Origen.** Corpus recopilado por McAuley y Leskovec (Universidad de Stanford) y publicado en el Stanford Network Analysis Project. Republicado en Kaggle bajo licencia CC0 (dominio público).

**Fuente:** https://www.kaggle.com/datasets/snap/amazon-fine-food-reviews

### Características generales

| Característica | Valor |
|---|---|
| Reseñas | 568 454 |
| Usuarios | 256 059 |
| Productos | 74 258 |
| Período | Octubre 1999 – Octubre 2012 |
| Mediana de palabras por reseña | 56 |
| Idioma | Inglés |

### Esquema

| Columna | Descripción | Tipo |
|---|---|---|
| `Id` | Identificador único de cada fila/reseña | entero |
| `ProductId` | Identificador único del producto reseñado | texto |
| `UserId` | Identificador único del usuario que escribió la reseña | texto |
| `ProfileName` | Nombre de perfil del usuario (26 valores faltantes) | texto |
| `HelpfulnessNumerator` | Cuántos usuarios marcaron la reseña como útil | entero |
| `HelpfulnessDenominator` | Cuántos usuarios en total votaron si la reseña era útil o no | entero |
| `Score` | Calificación otorgada por el usuario, de 1 a 5 estrellas | entero |
| `Time` | Marca de tiempo de cuándo se hizo la reseña | entero (Unix timestamp) |
| `Summary` | Resumen breve de la reseña (27 valores faltantes) | texto |
| `Text` | Contenido completo del texto de la reseña | texto |


---

## Referencias

McAuley, J. y Leskovec, J. (2013). *From amateurs to connoisseurs: modeling the evolution of user expertise through online reviews*. En *Proceedings of the 22nd International Conference on World Wide Web (WWW '13)*.

Stanford Network Analysis Project. *Web data: Amazon Fine Foods reviews*. https://snap.stanford.edu/data/web-FineFoods.html

---

## Licencia

El código de este repositorio se distribuye bajo licencia MIT.

El conjunto de datos utilizado está publicado bajo CC0 (dominio público). Si publica trabajos derivados del corpus, cite el artículo de McAuley y Leskovec (2013) conforme solicita la ficha original de los datos.
