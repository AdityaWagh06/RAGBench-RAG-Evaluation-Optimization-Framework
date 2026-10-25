# RAGBench

**A framework for benchmarking, evaluating, and optimizing Retrieval-Augmented Generation (RAG) pipelines.**

RAGBench is an open-source project designed to help developers understand, measure, and improve the performance of RAG systems through reproducible experiments and evaluation metrics.

Instead of relying on intuition, RAGBench aims to make it easier to compare retrieval strategies, embedding models, chunking configurations, and reranking approaches using consistent datasets and measurable results.

> **Project status:** Early development — the initial framework is being designed.

## Why RAGBench?

Building a RAG pipeline involves more than retrieving documents and passing them to a language model. Retrieval quality, chunking strategy, embedding selection, and context relevance can all affect the final answer.

RAGBench aims to provide a practical environment for evaluating these components independently and understanding their impact on overall pipeline performance.

## Planned Features

- **Retrieval Evaluation** — Measure retrieval precision, recall, and ranking quality.
- **Chunking Experiments** — Compare chunk sizes, overlap settings, and splitting strategies.
- **Embedding Evaluation** — Benchmark embedding models using consistent datasets.
- **Reranking Support** — Evaluate reranking strategies and their impact on retrieval quality.
- **RAG Quality Evaluation** — Assess context relevance, answer correctness, and faithfulness where suitable evaluation methods are available.
- **Reproducible Benchmarks** — Run comparable experiments against fixed datasets and configurations.
- **Evaluation Reports** — Generate structured reports to compare pipeline configurations.
- **Local-First Design** — Support offline evaluation where possible, without requiring paid model APIs for core functionality.

## How It Will Work

The intended workflow is:

1. Load a document collection and evaluation dataset.
2. Configure chunking, embedding, retrieval, and optional reranking strategies.
3. Run experiments against the same dataset.
4. Calculate relevant retrieval and answer-quality metrics.
5. Compare results and identify opportunities for improvement.

## Technology Stack

The initial implementation is planned around:

| Technology | Purpose |
|---|---|
| Python | Core evaluation framework |
| Sentence Transformers | Local embedding models |
| FAISS or ChromaDB | Vector search and retrieval experiments |
| FastAPI | Optional API for running experiments |
| pytest | Automated testing and regression checks |

The final stack may evolve as implementation decisions are validated.

## Evaluation Areas

RAGBench aims to cover multiple stages of a RAG pipeline:

- **Data ingestion:** Document loading, parsing, and preprocessing.
- **Retrieval:** Semantic search, top-k retrieval, and hybrid search.
- **Ranking:** Candidate ranking and reranking comparisons.
- **Generation:** Answer quality and groundedness evaluation.
- **Performance:** Execution time and experiment-level comparisons.

Metrics will be selected according to the component being evaluated rather than combining unrelated measurements into a single score.

## Getting Started

Installation instructions and runnable examples will be added as the initial implementation becomes available.

The project is not yet ready for production use.

## Roadmap

- [ ] Establish the core project structure and configuration format.
- [ ] Implement document ingestion and a baseline retrieval pipeline.
- [ ] Add configurable chunking strategies.
- [ ] Implement retrieval evaluation metrics.
- [ ] Add embedding and reranking comparisons.
- [ ] Introduce RAG answer-quality evaluation.
- [ ] Generate reproducible benchmark reports.
- [ ] Add automated tests and continuous integration.
- [ ] Document examples and supported integrations.

## Contributing

RAGBench is intended to be developed in the open. Contributions may include evaluation metrics, retrieval strategies, embedding integrations, datasets, testing, documentation, and performance improvements.

Before opening a pull request, check the repository's contribution guidelines and existing issues.

## Project Goals

RAGBench aims to make RAG evaluation more reproducible, transparent, and accessible to developers experimenting with retrieval-based AI applications.

The long-term goal is to help developers make evidence-based decisions about their RAG architectures instead of relying solely on anecdotal results.

## License

The project license will be specified in the repository before the first public release.