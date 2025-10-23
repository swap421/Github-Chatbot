# GitHub Chatbot CLI

A powerful CLI tool for interacting with GitHub using AI. Get insights about your pull requests, issues, and repository status through natural language queries.

## Features

- 🤖 **AI-powered GitHub interactions** using DeepSeek API
- 📋 **Pull request management** - view PRs, review comments
- 🐛 **Issue tracking** - track assigned issues and their status
- 🔍 **Repository monitoring** - check CI/CD status and repository info
- 🔐 **Secure session management** with encrypted storage
- 🎨 **Rich CLI interface** with beautiful formatting
- 🌍 **Cross-platform support** - Windows, macOS, Linux

## Installation

```bash
pip install github-chatbot
```

## Quick Start

1. **Install the package:**
   ```bash
   pip install github-chatbot
   ```

2. **Set up your API key:**
   ```bash
   export DEEPSEEK_API_KEY="your-deepseek-api-key"
   ```

3. **Start the chatbot:**
   ```bash
   gchat start
   ```

4. **Follow the prompts:**
   - Enter your GitHub Personal Access Token (PAT)
   - Enter your GitHub organization name
   - Enter your GitHub username

## Usage

### Basic Commands

```bash
# Start the chatbot
gchat start

# Clear saved session
gchat logout
```

### Example Queries

Once started, you can ask questions like:

- **"Show me my pull requests in the frontend repo"**
- **"What issues are assigned to me in the backend project?"**
- **"Get review comments for PR #123"**
- **"Check the CI status of the latest commit"**

## Configuration

### Required Setup

1. **GitHub Personal Access Token (PAT)**
   - Go to GitHub Settings → Developer settings → Personal access tokens
   - Create a token with `repo` and `read:org` scopes
   - Use this token when prompted by the chatbot

2. **DeepSeek API Key**
   - Get your API key from [DeepSeek](https://platform.deepseek.com/)
   - Set it as an environment variable: `DEEPSEEK_API_KEY`

### Session Management

The chatbot securely stores your:
- GitHub PAT (encrypted)
- Organization name
- Username

Data is stored in `~/.github-chatbot-secrets` with encryption.

## Requirements

- Python 3.8+
- GitHub Personal Access Token
- DeepSeek API Key
- Internet connection

## Dependencies

- `click` - CLI framework
- `requests` - HTTP requests
- `rich` - Beautiful terminal output
- `openai` - AI API client
- `cryptography` - Secure data storage
- `python-dotenv` - Environment variable management

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License.

## Support

If you encounter any issues or have questions:

1. Check the [Issues](https://github.com/yourusername/github-chatbot/issues) page
2. Create a new issue with detailed information
3. Include error messages and steps to reproduce

---

Made with ❤️ for the GitHub community
