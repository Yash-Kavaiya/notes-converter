# Notes Converter Agent

A helpful AI assistant powered by NVIDIA NIM and Google ADK that answers user questions using the Llama 3.1 Nemotron Nano 8B model.

## Features

- 🤖 AI-powered agent using Google ADK framework
- ⚡ Fast inference with NVIDIA NIM API
- 🦙 Powered by Llama 3.1 Nemotron Nano 8B model
- 📝 Simple and easy to use

## Prerequisites

- Python 3.8 or higher
- NVIDIA NIM API key ([Get one here](https://build.nvidia.com/))

## Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/Yash-Kavaiya/notes-converter.git
   cd notes-converter
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up environment variables**
   
   Copy the sample environment file:
   ```bash
   cp .env.sample .env
   ```
   
   Edit `.env` and add your NVIDIA NIM API key:
   ```properties
   NVIDIA_NIM_API_KEY=your_actual_api_key_here
   NVIDIA_NIM_API_BASE="https://integrate.api.nvidia.com/v1/"
   ```

## Usage

```python
from my_agent.agent import root_agent

# The agent is ready to use
# Add your implementation here to interact with the agent
```

## Project Structure

```
notes-converter/
├── my_agent/
│   ├── __init__.py
│   ├── agent.py          # Main agent configuration
│   └── __pycache__/
├── requirements.txt       # Python dependencies
├── .env                   # Environment variables (not tracked in git)
├── .env.sample           # Sample environment file
└── README.md             # This file
```

## Configuration

The agent is configured with the following settings:

- **Model**: `nvidia/llama-3.1-nemotron-nano-8b-v1`
- **Name**: `root_agent`
- **Description**: A helpful assistant for user questions
- **Instruction**: Answer user questions to the best of your knowledge

## Dependencies

- `google-adk`: Google Agent Development Kit for building AI agents

## Getting Your API Key

1. Visit [NVIDIA Build](https://build.nvidia.com/)
2. Sign in or create an account
3. Navigate to the API section
4. Generate your API key
5. Copy it to your `.env` file

## Security Notes

⚠️ **Important**: Never commit your `.env` file with actual API keys to version control. The `.env` file is already included in `.gitignore` to prevent accidental commits.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is open source and available under the [MIT License](LICENSE).

## Author

**Yash Kavaiya**
- GitHub: [@Yash-Kavaiya](https://github.com/Yash-Kavaiya)

## Support

If you encounter any issues or have questions, please open an issue on GitHub.

---

Made with ❤️ using Google ADK and NVIDIA NIM
