# Todo CLI

A command-line todo app built with Python, SQLite, Typer, and Rich.

## Setup

```bash
# Clone the repo
git clone <your-repo-url>
cd todocli-python

# Create a virtual environment
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

## Usage

```bash
# Add a todo
python todocli.py add "Finish homework" "Study"

# Show all todos
python todocli.py show

# Complete a todo (by position number)
python todocli.py complete 1

# Update a todo
python todocli.py update 1 --task "New task name" --category "Learn"

# Delete a todo
python todocli.py delete 1
```

## Project Structure

```
todocli-python/
├── model.py       # Todo data model
├── database.py    # SQLite database operations
├── todocli.py     # CLI commands and display
└── todo.db        # Local database (auto-generated, not on GitHub)
```

## Dependencies

- [Typer](https://typer.tiangolo.com/) — CLI framework
- [Rich](https://rich.readthedocs.io/) — terminal formatting and tables
- SQLite — built into Python, no install needed
