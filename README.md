# Sherpa Alzheimer's Chatbot

An AI-powered conversational chatbot developed collaboratively during the **OPIT Hackathon 2026** as part of **Team StackBreakers**.

Sherpa explores how conversational AI, multilingual support, and alternative interfaces can make Alzheimer's-related information more accessible.

> **Disclaimer:** This project is an educational hackathon prototype. It is not a substitute for professional medical advice, diagnosis, or treatment.

## Project Overview

Sherpa is a chatbot project combining a web-based frontend with a Python backend and AI model integration.

The project brings together conversational AI, multilingual functionality, and alternative interaction channels to explore more accessible ways of engaging with Alzheimer's-related information.

## Technology Stack

### Frontend
- Next.js 15+
- React
- TypeScript
- Tailwind CSS
- Lucide React

### Backend
- Django
- Django REST Framework
- SQLite
- Gradio Client
- Deep Translator
- LangDetect

### Integrations
- Telegram Bot API
- Amazon Alexa voice interface
- ngrok for development and testing of externally accessible services

## Key Project Areas

- **Conversational AI:** Integration with an AI model through the Gradio Client.
- **Multilingual support:** Language detection and translation functionality.
- **Web interface:** A frontend built with Next.js, React, and TypeScript.
- **Backend API:** Django REST Framework for backend functionality.
- **Alternative interfaces:** Telegram and an experimental Alexa integration.

The availability and completeness of individual features depend on the current implementation and configuration.

## Project Structure

The repository contains the following main components:

- `src/` — Frontend source code.
- `public/` — Public frontend assets.
- `accessibot_backend/` — Django backend.
- `chat_api/` — Chat API component.
- `manage.py` — Django management entry point.
- `package.json` — Frontend package configuration.

## Getting Started

### Prerequisites

- Node.js 18 or later.
- Python compatible with the backend dependencies.
- npm or pnpm.
- A Hugging Face read token if required by the configured AI model.

### Frontend Setup

Install the frontend dependencies:

```bash
npm install
```

Start the development server using the script defined in `package.json`:

```bash
npm run dev
```

Open the local development address printed in your terminal.

### Backend Setup

Create and activate a virtual environment from the project root.

**Windows:**

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

**Linux/macOS:**

```bash
python -m venv .venv
source .venv/bin/activate
```

Install the backend dependencies using the project's dependency file, if available.

If no dependency file exists, create one based on the packages and versions actually required by the backend before attempting installation.

Apply database migrations from the directory containing `manage.py`:

```bash
python manage.py migrate
```

Create an administrator account if required:

```bash
python manage.py createsuperuser
```

Run the Django development server:

```bash
python manage.py runserver
```

### Environment Configuration

Configure any required API credentials through environment variables or a local `.env` file.

Never commit real API tokens, passwords, or other secrets to version control.

Consult the relevant integration documentation to determine which environment variables are required.

## Team and Acknowledgements

Developed collaboratively during the **OPIT Hackathon 2026** as part of **Team StackBreakers**.

Special thanks to my teammate, **[EtahJo](https://github.com/EtahJo)**, for their collaboration and contributions to the project.

This repository showcases the project while acknowledging the collaborative effort behind its development.

### Original Project

The original repository is available at:

[EtahJo/sherpa-alzheimer](https://github.com/EtahJo/sherpa-alzheimer)

## Project Status

This repository documents a hackathon project. Setup instructions, integrations, and feature descriptions should be verified against the current source code.

## Disclaimer

Sherpa is an educational project and should not be relied upon for medical decisions or as a replacement for professional healthcare services.