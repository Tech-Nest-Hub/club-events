# OpenClaw: Prerequisites & Getting Started

> [!NOTE]
> OpenClaw is an open-source AI agent that runs on your own machine and can
> take real actions (browse, run code, send messages). This is a setup
> checklist, not the full manual.

## prerequisites

- 8 GB RAM minimum for better performance (16 GB+ for local models)
- Node.js 22, 24, or 25.9+ (check with `node --version` in you terminal or cmd). Node 26 is recommended according to the official [docs](https://docs.openclaw.ai/install).
- An API key for your chosen model provider. You can get one freely from **[Google AI Studio](https://aistudio.google.com/api-keys)**.

> [!WARNING]
> OpenClaw can run commands and send messages on your behalf. So, use it with caution.

## installation

#### using Scripts(Recommended)

#### For macOS / Linux / WSL

```bash
curl -fsSL https://openclaw.ai/install.sh | bash
```

#### For Windows

```bash
iwr -useb https://openclaw.ai/install.ps1 | iex
```

#### using npm(Recommended)

```bash
npm i -g openclaw
```

```bash
openclaw onboard
```

Here is the official installation guide [link](https://docs.openclaw.ai/install) for more information.

## after install

1. Run the onboarding wizard, pick a model provider, paste in your API key
2. It opens a Control UI in your browser (default port 18789)
3. Send a test message, confirm you get a reply
4. Optional: connect a messaging app

> [!TIP]
> Everything else (skills, plugins, schedules) can wait until you actually need it.
