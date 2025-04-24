# MCP Chat Application

This is an interactive chat application that uses the Model Control Protocol (MCP) with Groq's language models. The application provides a command-line interface for having conversations with an AI assistant while maintaining conversation memory.

## Features

- Interactive command-line chat interface
- Integration with Groq's language models (using qwen-qwq-32b)
- Conversation memory management
- Simple commands for clearing history and exiting
- Browser automation capabilities through MCP

## Prerequisites

- Python 3.x
- Required API keys:
  - GROQ_API_KEY

## Installation

1. Clone this repository:
```bash
git clone <https://github.com/rohith372/MCP>
cd <https://github.com/rohith372/MCP>
```

2. Install the required dependencies:
```bash
pip install -r requirements.txt
uv add langchain-groq
uv add langchain-openai
uv add mcp-use
```

3. Create a `.env` file in the project root and add your API keys:
```
GROQ_API_KEY=your_groq_api_key_here
```

## Usage

1. Run the chat application:
```bash
python app.py
```

2. Available commands during chat:
- Type your message and press Enter to chat with the assistant
- Type `clear` to clear the conversation history
- Type `exit` or `quit` to end the conversation

## Configuration

The application uses a configuration file `browser_mcp.json` for MCP client settings. Make sure this file is present in your project directory with the appropriate configuration.

## Dependencies

- langchain-groq
- python-dotenv
- mcp-use
- asyncio

## Error Handling

The application includes basic error handling for:
- API communication issues
- Invalid inputs
- Session management
