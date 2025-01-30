# Browser Hot-Reloading in FastAPI using arel

[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
[![Python Versions](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/downloads/)

## 🌟 Overview

Browser hot-reloading is a crucial development technique that automatically refreshes your web application when source files change, providing a seamless and efficient development experience for Python ASGI web frameworks like FastAPI.

## 📖 What is arel?

`arel` is a lightweight library designed to implement development-only hot-reloading for non-Python files that are not dynamically read from disk on each request. This includes:

- HTML templates
- GraphQL schemas
- Cached rendered Markdown content
- Static assets

### Key Features

- Real-time file change detection
- WebSocket-based browser notifications
- Customizable reload hooks
- Minimal performance overhead

## 🔧 How Does arel Work?

1. **File Watching**: arel monitors specified files for changes
2. **WebSocket Notification**: When a file is modified, it sends a signal to the browser
3. **Automatic Reload**: An injected client script triggers a page refresh
4. **Custom Hooks**: Developers can register additional server-side reload operations

## 🚀 Quick Start

### Prerequisites

- Python 3.8+
- FastAPI
- uvicorn

### Installation

```bash
# Clone the repository
git clone https://github.com/ashleymavericks/browser-hot-reloading.git

# Install dependencies
pipenv install  # or pip install -r requirements.txt
```

### Running the Application

```bash
# Start the FastAPI application with hot-reloading
DEBUG=true uvicorn main:app --reload
```

## 🧠 Deep Dive: How It Works

For an in-depth explanation of browser hot-reloading and the implementation details, check out the comprehensive blog post:

[Supercharge Your FastAPI Development with Browser Hot Reloading Using Arel](https://dev.to/ashleymavericks/browser-hot-reloading-for-python-asgi-web-apps-using-arel-1l19)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
