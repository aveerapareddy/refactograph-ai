# Refactograph AI

GPT-powered codebase knowledge graph & intelligent refactoring assistant

## Overview

Refactograph AI is a tool that helps developers understand and improve their codebase by:

1. Building a knowledge graph of code dependencies
2. Analyzing code structure and relationships
3. Generating intelligent refactoring suggestions using GPT
4. Providing impact analysis for potential changes

## Features

- **Code Parsing**: AST-based analysis of Python code
- **Dependency Graph**: Visualization and analysis of code relationships
- **GPT Integration**: AI-powered refactoring suggestions
- **Impact Analysis**: Understanding the effects of code changes
- **REST API**: Easy integration with existing tools

## Project Structure

```
refactograph-ai/
├── parser/          # Code parsing and analysis
├── graph/           # Dependency graph management
├── llm/             # GPT integration and suggestions
├── api/             # FastAPI backend
├── data/            # Sample code and test data
├── requirements.txt # Project dependencies
```

## Setup

1. Clone the repository:

   ```bash
   git clone https://github.com/aveerapareddy/refactograph-ai.git
   cd refactograph-ai
   ```

2. Create a virtual environment:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

4. Set up environment variables:
   ```bash
   cp .env.example .env
   # Edit .env and add your OpenAI API key
   ```

## Usage

1. Start the API server:

   ```bash
   cd api
   uvicorn main:app --reload
   ```

2. Access the API documentation at `http://localhost:8000/docs`

3. Use the API to:
   - Upload and analyze code
   - Get refactoring suggestions
   - View dependency graphs
   - Perform impact analysis

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
