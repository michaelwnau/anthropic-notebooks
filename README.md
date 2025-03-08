# Anthropic Notebooks
A comprehensive collection of Jupyter notebooks for working with Anthropic's Claude AI models. This repository provides examples, tutorials, and utilities
for leveraging Claude's capabilities across various use cases.

  ## Purpose

  This repository serves as a practical resource for developers, researchers, and data scientists working with Anthropic's Claude AI models. It includes
  examples and tutorials for:

  - Interacting with Claude through the Anthropic API
  - Implementing RAG (Retrieval Augmented Generation) systems
  - Working with multimodal capabilities (images, charts, graphs)
  - Building practical applications with Claude's computer use capabilities

  ## Repository Structure

```
  anthropic-notebooks/
  ├── computer-use/              # Notebooks for Claude's computer use capabilities
  │   ├── Lesson_2.ipynb
  │   ├── Lesson_3.ipynb
  │   ├── Lesson_4.ipynb
  │   ├── Lesson_5.ipynb
  │   └── Lesson_6.ipynb
  ├── context-retrieval/         # RAG implementation examples
  │   └── context_rag.ipynb
  ├── examples/                  # General usage examples
  │   └── multimodal/
  │       └── multimodal_contextual_retrieval_rag.ipynb
  ├── images-graphs/             # Working with visual content
  │   ├── image_caption_anthropic.ipynb
  │   └── reading_charts_graphs_powerpoints.ipynb
  ├── CLAUDE.md                  # Development guidelines
  ├── LICENSE
  ├── pyproject.toml            # Project configuration
  └── README.md
```
  ## Prerequisites

  - Python 3.10 or higher
  - Anthropic API key

  ## Installation

  1. Clone the repository:
     ```bash
     git clone https://github.com/yourusername/anthropic-notebooks.git
     cd anthropic-notebooks

  2. Set up the environment using uv:
  uv pip install -e ".[dev]"
  uv venv
  3. Activate the virtual environment:
    - Linux/Mac: source .venv/bin/activate
    - Windows: .venv\Scripts\activate

  Usage

  1. Set up your Anthropic API key as an environment variable:
  export ANTHROPIC_API_KEY=your_api_key_here
  2. Launch Jupyter:
  jupyter notebook
  3. Navigate to the notebook of interest and run the cells.

  Alternatively, you can run a specific notebook:
  jupyter nbconvert --execute [notebook_path] --to notebook --output [output_path]

  Available Examples and Capabilities

  Computer Use

  Tutorials for leveraging Claude's computer use capabilities, covering topics from basic interaction to advanced usage patterns.

  Context Retrieval

  Implementation of Retrieval Augmented Generation (RAG) systems with Claude, including contextual embeddings for enhanced performance.

  Multimodal

  Examples of working with Claude's multimodal capabilities, combining text and visual inputs for rich interactions.

  Images and Graphs

  Notebooks demonstrating how to:
  - Process and caption images using Claude
  - Extract information from charts, graphs, and PowerPoint presentations

  Dependencies

  Main dependencies:
  - anthropic
  - jupyter
  - notebook
  - ipykernel
  - matplotlib
  - pillow

  Development dependencies:
  - ruff (for linting and formatting)

  Contributing Guidelines

  When contributing to this repository, please follow these guidelines:

  Code Style & Linting

  - Run linter: ruff check .
  - Apply automatic fixes: ruff check --fix .
  - Format imports: ruff format .
  - Use descriptive variable names (e.g., response over resp)
  - Follow import structure: standard libs → third-party → local modules
  - Include type hints for function parameters and return values
  - Use Python f-strings for string formatting
  - Handle API errors explicitly with try/except blocks

  Notebook Best Practices

  - Document code with markdown cells explaining purpose and approach
  - Include output cells when committing notebooks
  - Keep notebook cells focused and atomic (single responsibility)
  - Use standard Claude API patterns from Anthropic documentation
  - Group new notebooks by topic/functionality
  - Maintain backward compatibility with Claude API versions

  Repository Organization

  - Store media assets in appropriate subdirectories
  - Follow existing patterns when generating new examples

  License

  [License information]

  Acknowledgements

  This repository contains examples based on Anthropic's official cookbooks and documentation.
  ```
