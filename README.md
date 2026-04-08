# ChatBot

A Python chatbot powered by the Anthropic Claude API, demonstrating single-turn and multi-turn conversations.

## Prerequisites

- Python 3.11+
- An [Anthropic API key](https://console.anthropic.com/)

## Setup

1. **Clone the repository**

   ```bash
   git clone <repo-url>
   cd ChatBot
   ```

2. **Install dependencies**

   ```bash
   pip install -e .
   ```

   This installs the required packages:
   - `anthropic` — Anthropic Python SDK
   - `python-dotenv` — loads environment variables from a `.env` file

3. **Configure your API key**

   Create a `.env` file in the project root:

   ```
   ANTHROPIC_API_KEY=your-api-key-here
   ```

## Usage

### Notebook

Open [01_Requests.ipynb](01_Requests.ipynb) to explore interactive examples:

- Loading the API key from `.env`
- Sending a single message to Claude
- Building a multi-turn conversation with helper functions (`add_user_message`, `add_assistant_message`, `chat_with_claude`)

### CLI

```bash
python main.py
```

## Project Structure

```
├── 01_Requests.ipynb   # Jupyter notebook with API usage examples
├── main.py             # Application entry point
├── pyproject.toml      # Project metadata and dependencies
└── README.md
```