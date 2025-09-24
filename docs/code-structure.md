# Code Structure Documentation 🏗️

This document provides a comprehensive overview of the GitHub Copilot Hands-on Labs repository structure, making it easy for contributors and users to understand how the codebase is organized.

## Repository Overview

The repository is organized into several main directories, each serving a specific purpose in delivering GitHub Copilot learning experiences:

```
github-copilot-hands-on/
├── docs/                    # MkDocs documentation site
├── labs/                    # Hands-on lab exercises
├── images/                  # Shared images and QR codes
├── .github/                 # GitHub configuration and workflows
├── .devcontainer/           # Development container configuration
├── README.md               # Main repository documentation
├── CONTRIBUTING.md         # Contribution guidelines
├── LICENSE.md              # Project license
├── CHANGELOG.md           # Version history
└── mkdocs.yml             # MkDocs configuration
```

## Documentation Structure (`docs/`)

The `docs/` directory contains the complete documentation site built with MkDocs Material:

### Core Documentation
- `index.md` - Main documentation landing page
- `workshop-overview.md` - Complete workshop overview and structure
- `train-the-trainer.md` - Guidelines for workshop facilitators
- `model-comparison.md` - Comparison of different AI models
- `future-roadmap.md` - Planned features and improvements
- `rag-extension-lab.md` - RAG (Retrieval Augmented Generation) extension lab

### Hands-on Labs (`docs/hands-on/`)
Detailed step-by-step guides for each lab exercise:

#### Fundamentals
- `html-gallery.md` - HTML Image Gallery with animations
- `rock_paper_scissors.md` - Rock Paper Scissors game in Python

#### APIs
- `starwars-api.md` - Star Wars API client in Java
- `starwars-api-python.md` - Star Wars API client in Python

#### MCP (Model Context Protocol)
- `gh-gallery-mcp.md` - Image Gallery using MCP
- `mcp-server-starter.md` - Building custom MCP servers

#### Additional Resources
- `index.md` - Labs overview and navigation
- `other-labs.md` - Additional lab exercises

### Assets (`docs/assets/`)
- `images/` - Documentation images organized by topic
  - `custom/` - Custom branding and logos
  - `gallery/` - HTML gallery screenshots
  - `mcp/` - MCP-related images
  - `python/` - Python lab screenshots
  - `starwarsapi/` - API lab screenshots
  - `workshop/` - Workshop overview images

### JavaScript (`docs/javascripts/`)
- `tablesort.js` - Table sorting functionality for documentation

## Labs Structure (`labs/`)

The `labs/` directory contains all hands-on exercise implementations organized by programming language and technology:

### HTML/JavaScript (`labs/html/`)
- `calculator/` - Basic calculator implementation
  - `README.md` - Exercise instructions
  - `calculator.html` - Calculator implementation
- `gallery/` - Image gallery with animations
  - `instructions.md` - Detailed step-by-step guide
  - `index.html` - Basic gallery implementation
  - `index-vision_agent.html` - Advanced vision agent version
  - `images/` - Gallery sample images
  - `solution/` - Complete solution files

### Java (`labs/java/`)
- `README.md` - Java labs overview
- `starwarsapi/` - Star Wars API client
  - `instructions.md` - Step-by-step implementation guide
  - `pom.xml` - Maven configuration
  - `src/` - Source code structure
  - `images/` - Supporting screenshots
- `crudapp/` - CRUD application example
  - `instructions.md` - Implementation guide
  - `demo/` - Demonstration files

### Python (`labs/python/`)
- `README.md` - Python labs overview
- `rock_paper_scissors/` - Game implementation
  - `README.md` - Quick start guide
  - `game.py` - Main game logic
  - `tests/` - Unit tests
- `starwarsapi/` - API client implementation
  - `README.md` - Project overview
  - `requirements.txt` - Python dependencies
  - `src/` - Source code
  - `tests/` - Test suite

### GitHub Copilot Extensions (`labs/ghcp-extensions/`)
- `README.md` - Guide for GitHub Copilot extensions

### Infrastructure as Code (`labs/terraform-iac/`)
- `README.md` - Terraform/IaC exercises

## GitHub Configuration (`.github/`)

### Templates
- `ISSUE_TEMPLATE.md` - Issue reporting template
- `PULL_REQUEST_TEMPLATE.md` - Pull request template
- `CODE_OF_CONDUCT.md` - Community guidelines

### Workflows (`workflows/`)
- `deploy-mkdocs.yml` - Automated documentation deployment

## Development Environment

### Container Configuration (`.devcontainer/`)
- `devcontainer.json` - VS Code development container setup with all necessary tools and extensions

### Documentation Configuration
- `mkdocs.yml` - MkDocs Material configuration including:
  - Theme customization
  - Navigation structure
  - Plugin configuration
  - Markdown extensions

## Lab Structure Standards

Each lab follows a consistent structure:

1. **README.md** - Quick overview and getting started
2. **instructions.md** (where applicable) - Detailed step-by-step guide
3. **Source files** - Implementation code
4. **Tests** - Unit tests and validation
5. **Images/Screenshots** - Visual aids and examples
6. **Solution files** - Complete working examples

## Adding New Labs

When contributing new labs, follow this structure:

1. Create a new directory in the appropriate language folder under `labs/`
2. Add a comprehensive `README.md` with overview and quick start
3. Include detailed `instructions.md` with step-by-step guidance
4. Provide complete source code with comments
5. Add unit tests where applicable
6. Include supporting images in an `images/` subdirectory
7. Create corresponding documentation in `docs/hands-on/`
8. Update navigation in `mkdocs.yml`

## Documentation Standards

- Use clear, descriptive headings
- Include code snippets with syntax highlighting
- Add screenshots for UI components
- Provide both beginner and advanced sections
- Include GitHub Copilot tips and suggestions
- Use consistent emoji icons for visual appeal
- Cross-reference related materials

## Build and Deployment

The repository uses MkDocs Material for documentation:

- **Local development**: `mkdocs serve`
- **Build**: `mkdocs build`
- **Deployment**: Automated via GitHub Actions to GitHub Pages

## Contributing Guidelines

See the [repository CONTRIBUTING.md](https://github.com/Azure-Samples/github-copilot-hands-on/blob/main/CONTRIBUTING.md) for detailed contribution guidelines including:
- Code standards
- Pull request process
- Issue reporting
- Community guidelines

---

For questions about the repository structure or to suggest improvements, please open an issue or start a discussion.