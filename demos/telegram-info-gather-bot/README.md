# Telegram Info Gather Bot

This folder is for a Telegram message gathering and digest bot.

## Environment Rule

Use this folder's virtual environment.

Do not use global Python for this project.

Project Python:

```powershell
.\.venv\Scripts\python.exe
```

Activate the virtual environment:

```powershell
.\.venv\Scripts\Activate.ps1
```

After activation, install dependencies if needed:

```powershell
pip install -r requirements.txt
```

## Installed Packages

The current project environment includes:

- `telethon`
- `python-dotenv`

They are listed in `requirements.txt`.

## Sensitive Files

Do not commit or upload these files:

- `.env`
- `*.session`
- `*.session-journal`
- `data/`
- `output/`
- `logs/`

These are already covered by `.gitignore`.

## Config

Copy `.env.example` to `.env` when setting up real credentials.

Required values:

```env
TELEGRAM_API_ID=
TELEGRAM_API_HASH=
TELEGRAM_PHONE=
TARGET_CHAT=
```

Meaning:

- `TELEGRAM_API_ID`: Telegram developer API ID from `https://my.telegram.org`
- `TELEGRAM_API_HASH`: Telegram developer API hash
- `TELEGRAM_PHONE`: your Telegram phone number
- `TARGET_CHAT`: group username, invite link, or chat id to read from

## Next Step

The first script should only do this:

1. Log in with Telethon.
2. List available chats.
3. Fetch a small sample of messages.
4. Save the sample locally.

Do not add AI summary or auto-forwarding until message access is confirmed.

## Note For Future Codex Chats

Before working on this project, read this README first.

Use:

```powershell
.\.venv\Scripts\python.exe
```

Do not use:

```powershell
python
```

unless the virtual environment has already been activated.
