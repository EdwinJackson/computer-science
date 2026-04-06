# Gemini Context: Computer Science Knowledge Base

This repository is a comprehensive personal knowledge base and study guide for Computer Science, System Architecture, and Site Reliability Engineering (SRE). It is primarily used for technical interview preparation and as a "digital garden" for continuous learning.

## Directory Overview

The project is structured as an **Obsidian Vault**, organized into thematic folders covering various domains of computer science and software engineering.

- **`algorithms/`**: Detailed explanations, complexity analysis, and implementations (often in TypeScript) of core algorithms (e.g., Binary Search, Merge Sort, Quick Sort).
- **`architecture/`**: System design concepts, patterns, and tradeoffs (e.g., Load Balancing, Backpressure, Outbox Pattern, Recovery Point Objective).
- **`data structures/`**: Fundamental building blocks of data organization (e.g., Arrays, B-Trees, Hash Tables, Stacks, Queues).
- **`data-engineering/`**: Ecosystems, loaders, replicators, and patterns related to data processing and storage.
- **`machine-learning/`**: Core ML concepts, including Attention mechanisms, Transformers, Embeddings, and Vectors.
- **`problems/`**: Solutions and notes for specific technical interview problems (e.g., Two Sum, Group Anagrams), following a standard template (Difficulty, Requirements, Test Cases, Solution).
- **`site-reliability-engineering/`**: Concepts related to DevOps and SRE, including SLAs, SLIs, SLOs, and Observability. This folder appears to be a nested Git repository.
- **`Tutorials/`**: Practical guides (e.g., RAG with LLaMa 3).
- **`assets/`**: Images, diagrams, and Excalidraw files used throughout the notes.
- **`.obsidian/`**: Configuration for the Obsidian editor, including plugins like `obsidian-excalidraw-plugin` and `table-editor-obsidian`.

## Key Files

- **`Readme.md`**: Contains a structured **12-week Study Plan** for technical interview preparation, mapping topics to specific weeks and LeetCode problems.
- **`Algorithm Analysis.md`**: General overview of Big O notation and complexity analysis.
- **`.agent/workflows/conceptual-summary.md`**: A template for summarizing concepts, encouraging the use of Mermaid diagrams and analogies.

## Usage & Conventions

### Note Structure
Most concept notes follow a consistent pattern:
1.  **Explanation**: High-level definition and "how it works."
2.  **Specifications**: Complexity analysis (Time/Space) for algorithms or key features for architectural patterns.
3.  **Implementation/Examples**: Code snippets (TypeScript, JavaScript) or diagrams (Mermaid, Excalidraw).
4.  **Inter-linking**: Notes heavily use Obsidian **WikiLinks** (`[[Note Name]]`) to connect related concepts.

### Coding Style
Code examples are primarily in **TypeScript** or **JavaScript**. They are typically written for clarity and education rather than production use.

### Interaction Guidelines
When asked to summarize a new concept or update an existing one:
- Refer to the template in `.agent/workflows/conceptual-summary.md`.
- Use **WikiLinks** to link to existing notes in the vault.
- Include **Complexity Analysis** for any algorithmic content.
- Use **Mermaid** for architectural diagrams when appropriate.
- Prioritize **"Understanding over Memorization"** as per the `Readme.md` philosophy.
