# Snippetbox

[![Go](https://img.shields.io/badge/Go-1.21+-00ADD8?style=flat&logo=go&logoColor=white)](https://golang.org)
[![License](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)

A modern, lightweight snippet sharing service built purely in Go. Think of it as your own self-hosted version of Pastebin or GitHub Gist, where users can easily upload, share, and manage code snippets.

## 🚀 Features

- **Snippet Upload & Sharing**: Upload text/code snippets with syntax highlighting
- **Clean Web Interface**: Simple, intuitive user interface for browsing and creating snippets
- **Snippet Management**: View, edit, and organize your code snippets
- **Multiple Language Support**: Syntax highlighting for various programming languages
- **Lightweight & Fast**: Built with Go for optimal performance
- **Self-Hosted**: Run your own snippet sharing service
- **No Dependencies**: Pure Go implementation with minimal external dependencies

## 🛠️ Tech Stack

- **Backend**: Pure Go (Golang)
- **Web Framework**: Go's standard `net/http` package or lightweight Go web framework
- **Database**: SQLite/PostgreSQL/MySQL (configurable)
- **Frontend**: HTML/CSS/JavaScript with Go templates
- **Deployment**: Standalone binary or Docker container

## 📋 Prerequisites

- Go 1.21 or higher
- Database (SQLite for development, PostgreSQL/MySQL for production)

## 🔧 Installation

### From Source

```bash
# Clone the repository
git clone https://github.com/lokicodess/snippetbox.git
cd snippetbox

# Build the application
go build -o snippetbox ./cmd/web

# Run the application
./snippetbox
```

### Using Go Install

```bash
go install github.com/lokicodess/snippetbox/cmd/web@latest
```

### Docker

```bash
# Build Docker image
docker build -t snippetbox .

# Run with Docker
docker run -p 8080:8080 snippetbox
```

## 🚀 Usage

1. Start the application:
   ```bash
   ./snippetbox
   ```

2. Open your browser and navigate to `http://localhost:8080`

3. Create a new snippet:
   - Click on "Create Snippet"
   - Paste your code or text
   - Add a title and select the language
   - Save and share the generated URL

4. Share snippets with others using the generated URLs

## 📁 Project Structure

```
snippetbox/
├── cmd/
│   └── web/            # Web application entry point
├── internal/
│   ├── handlers/       # HTTP handlers
│   ├── models/         # Data models and database logic
│   ├── validator/      # Input validation
│   └── config/         # Configuration management
├── ui/
│   ├── html/           # HTML templates
│   ├── static/         # CSS, JS, and other static files
│   └── assets/         # Images and other assets
├── migrations/         # Database migration files
├── docker/             # Docker configuration
├── docs/              # Documentation
└── README.md
```

## ⚙️ Configuration

The application can be configured using environment variables or a configuration file:

```bash
export SNIPPETBOX_PORT=8080
export SNIPPETBOX_DB_DSN="user:pass@tcp(localhost:3306)/snippetbox"
export SNIPPETBOX_SECRET_KEY="your-secret-key"
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by services like Pastebin and GitHub Gist
- Built with the power and simplicity of Go
- Thanks to the Go community for excellent libraries and tools

## 📞 Support

If you have any questions or need help, please:
- Open an issue on GitHub
- Check the [documentation](docs/)
- Join our community discussions

---

**Made with ❤️ and Go**