# MCP Demo Project

A Python-based demo service built using the model Control Protocol (MCP) framework. This project provides a collection of mathematical operations and utilities through an MCP server. s

## Features

- Basic arithmetic operations (addition, subtraction, multiplication, division)
- Advanced mathematical functions (power, square root, cube root)
- Trigonometric functions (sin, cos, tan)
- Special operations (factorial, logarithm, remainder)
- List operations (sum of list, exponential sum)
- Image processing capabilities (thumbnail creation)
- String operations (ASCII value conversion)
- Fibonacci sequence generation

## Prerequisites

- Python 3.8 or higher
- pip (Python package installer)

## Installation

1. Clone the repository:
```bash
git clone <your-repository-url>
cd mcp-assignment
```

2. Create and activate a virtual environment:
```bash
python3 -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

### Running the Server

To run the MCP server:

```bash
python src/server.py dev  # For development server
# or
python src/server.py      # For stdio transport
```

### Available Tools

The server provides the following tools:

#### Basic Arithmetic
- `add(a: int, b: int) -> int`: Add two numbers
- `subtract(a: int, b: int) -> int`: Subtract two numbers
- `multiply(a: int, b: int) -> int`: Multiply two numbers
- `divide(a: int, b: int) -> float`: Divide two numbers

#### Advanced Mathematics
- `power(a: int, b: int) -> int`: Calculate power of two numbers
- `sqrt(a: int) -> float`: Calculate square root
- `cbrt(a: int) -> float`: Calculate cube root
- `factorial(a: int) -> int`: Calculate factorial
- `log(a: int) -> float`: Calculate natural logarithm
- `remainder(a: int, b: int) -> int`: Calculate remainder of division

#### Trigonometric Functions
- `sin(a: int) -> float`: Calculate sine
- `cos(a: int) -> float`: Calculate cosine
- `tan(a: int) -> float`: Calculate tangent

#### List Operations
- `add_list(l: list) -> int`: Sum all numbers in a list
- `int_list_to_exponential_sum(int_list: list) -> float`: Calculate sum of exponentials

#### Special Functions
- `mine(a: int, b: int) -> int`: Special mining operation
- `fibonacci_numbers(n: int) -> list`: Generate Fibonacci sequence
- `strings_to_chars_to_int(string: str) -> list[int]`: Convert string to ASCII values
- `create_thumbnail(image_path: str) -> Image`: Create image thumbnail
- `open_notes() -> dict`: Open Notes app in macos
- `create_note_table_and_add_text(serial_number: int, query: str, response_text: str) -> dict`: Create a new note and add a table with llm query and response.

## Project Structure

```
mcp-assignment/
├── src/
│   ├── server.py      # Main server implementation
│   └── talk2mcp.py    # Client implementation
├── requirements.txt   # Project dependencies
├── .gitignore        # Git ignore rules
├── LICENSE           # MIT License
└── README.md         # This file
```

## Development

The project uses the Mission Control Protocol (MCP) framework for communication between the client and server. The server implements various mathematical and utility functions as MCP tools that can be called by the client.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

