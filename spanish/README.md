# Demostraciones de embeddings vectoriales

Un embedding vectorial codifica una entrada como una lista de números de punto flotante.

"dog" → [0.017198, -0.007493, -0.057982, 0.054051, -0.028336, 0.019245,…]

Diferentes modelos producen diferentes embeddings, con longitudes variadas.

| Modelo | Codifica | Longitud del vector |
| --- | --- | --- |
| word2vec | palabras | 300 |
| Sbert (Sentence-Transformers) | texto (hasta ~400 palabras) | 768 |
| OpenAI text-embedding-ada-002 | texto (hasta 8191 tokens) | 1536 |
| OpenAI text-embedding-3-small | texto (hasta 8191 tokens) | 256-1536 |
| OpenAI text-embedding-3-large | texto (hasta 8191 tokens) | 256-3072 |
| Azure AI Vision | imagen o texto | 1024 |

Los embeddings vectoriales se usan comúnmente para búsqueda por similitud, detección de fraude, sistemas de recomendación y RAG (Generación Aumentada por Recuperación).

Este repositorio contiene una exploración visual de vectores, utilizando varios modelos de embedding.

Notebooks disponibles aquí:

* [Generamos embeddings de OpenAI para conjuntos de datos](prep_openai.ipynb)
* [Generamos embeddings de Word2Vec para conjuntos de datos](../prep_word2vec_gnews.ipynb)
* [Generamos nuevos embeddings de texto de OpenAI](generate_embedding.ipynb)
* [Comparamos embeddings de OpenAI y Word2Vec](comparison.ipynb)
* [Similitud vectorial](similarity.ipynb)
* [Búsqueda vectorial](search.ipynb)
* [Generamos vectores multimodales para conjunto de datos](prep_multimodal.ipynb)
* [Exploramos vectores multimodales](multimodal_vectors.ipynb)
* [Métricas de distancia vectorial](distance_metrics.ipynb)
* [Cuantización vectorial](quantization.ipynb)
* [Reducción de dimensiones vectoriales (MRL)](dimension_reduction.ipynb)
