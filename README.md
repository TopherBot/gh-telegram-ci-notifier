# GH Telegram CI Notifier

A tiny Python project that demonstrates a fast‑track repository with a complete CI pipeline.
On every push, GitHub Actions runs linting, tests and sends a Telegram message indicating success or failure.

## Features
- Single `main.py` script (Hello World)
- Pytest test suite
- Flake8 linting
- GitHub Actions workflow with best‑practice settings:
  - Pinning actions to immutable SHAs
  - Concurrency cancellation
  - Least‑privilege token permissions
  - Optional Telegram alerts via `curl`

## Setup

1. Clone the repo.
2. Create a Telegram Bot via @BotFather and obtain `BOT_TOKEN` and a chat ID.
3. Add the following secrets in your repository settings:
   - `TELEGRAM_BOT_TOKEN`
   - `TELEGRAM_CHAT_ID`
4. Push changes; the CI will run automatically.

## Usage

```bash
python main.py
```

## License

MIT
