# AI-Air-Assistant-Agent (Ollama & Gradio)

AirAssistant Agent is an intelligent, automated airline assistant designed to help users retrieve flight information, check prices, and get status updates dynamically using AI.

## Key Features
- **Intelligent Tool Calling:** Uses LLMs to autonomously determine when to query databases for flight information.
- **Dynamic Interaction:** Provides real-time answers based on custom database tools.
- **User-Friendly Interface:** Built with Gradio to provide a clean, chat-based experience for end-users.
- **Secure Architecture:** Implements environment variable management to keep API keys secure.

## Prerequisites
To run this project, ensure you have the following installed:
- Python 3.9+
- `pip install gradio langchain openai python-dotenv`

## Getting Started
- Clone the repository.
- Create a .env file in the root directory of the project and configure the following environment variables:

```bash
OLLAMA_BASE_URL=http://localhost:11434/v1
OLLAMA_MODEL=llama3
```
## Setup
- Using Python + venv

bash:
```BASH
pyenv local 3.11.3
python -m venv .venv
source .venv/Scripts/activate
python -m pip install --upgrade pip
pip install -r requirements.txt
```
Install Dependensies

- Using UV (recommended)

After selecting the Python version, create a virtual environment with uv:

````
uv venv
````
Then install the dependencies:

````
uv pip install -r requirements.txt --refresh
````