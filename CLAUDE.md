# CLAUDE.md - Guidelines for working with anthropic-notebooks

## Environment Setup
- Install dependencies: `uv pip install -e ".[dev]"`
- Create virtual environment: `uv venv`
- Activate virtual environment: `source .venv/bin/activate` (Linux/Mac) or `.venv\Scripts\activate` (Windows)

## Notebook Execution
- Run notebooks: `jupyter notebook` (opens web interface)
- Run specific notebook: `jupyter nbconvert --execute [notebook_path] --to notebook --output [output_path]`

## Code Style & Linting
- Run linter: `ruff check .`
- Fix linting issues: `ruff check --fix .`
- Format imports: `ruff format .`
- Prefer descriptive variable names (e.g., `response` over `resp`)
- Import structure: standard libs → third-party → local modules
- Type hints encouraged for function parameters and return values
- Use Python f-strings for string formatting
- Handle API errors explicitly with try/except blocks
- Document code with markdown cells explaining purpose/approach
- Include output cells when committing notebooks
- Keep notebook cells focused and atomic (single responsibility)
- Use standard Claude API patterns from Anthropic documentation

## Repository Organization
- Group notebooks by topic/functionality
- Store media assets in appropriate subdirectories
- Maintain backward compatibility with Claude API versions

When generating new examples, follow existing patterns in similar notebooks.