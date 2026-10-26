# Mini AI Coding Agent

A Python-based AI coding agent powered by the OpenAI API that can interact with a local development environment through tool calling. The agent can inspect files, read code, create or modify files, and execute shell commands with user approval.

## Features

- **File Explorer:** Lists files and directories in the working directory.
- **File Reader:** Reads text files to provide the agent with context.
- **File Writer:** Creates and updates files based on user instructions.
- **Command Execution:** Runs shell commands after requesting user permission.
- **Tool Calling:** Uses the OpenAI API to decide which tools are needed to complete a task.
- **Interactive Terminal:** Supports ongoing conversations with the agent.

## Tech Stack

- Python
- OpenAI API
- JSON
- Git and GitHub

## How It Works

1. The user submits a task through the terminal.
2. The OpenAI model determines whether a tool is needed.
3. The agent executes the requested tool and returns its result to the model.
4. The model uses the result to decide the next step or provide a final response.

## Getting Started

### Prerequisites

- Python 3.10 or newer
- An OpenAI API key
- Git

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/christianlafaille1-spec/mini-ai-coding-agent.git
   cd mini-ai-coding-agent
   ```

2. Create and activate a virtual environment:

   ```bash
   python -m venv .venv
   ```

   Windows PowerShell:

   ```powershell
   .venv\Scripts\Activate.ps1
   ```

3. Install the OpenAI Python SDK:

   ```bash
   pip install openai
   ```

4. Set your API key as an environment variable in PowerShell:

   ```powershell
   $env:OPENAI_API_KEY="your-api-key"
   ```

5. Run the agent using the appropriate Python entry-point file in the project.

## Security

- API keys should be stored in environment variables, never committed to source code.
- Shell commands require user approval before execution.
- Only run commands and modify files you understand and trust.

## Future Improvements

- Improved file and directory access controls
- Better error handling and logging
- Conversation history management
- More robust command execution safeguards
- Unit tests and automated testing

## Author

Christian Lafaille

Built as a hands-on project to explore AI agents, Python development, and tool calling.
