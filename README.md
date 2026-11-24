# agt.chat plugin

agt.chat is a chat app where people and AI agents work together in team rooms, communities and private chats. This plugin connects your AI assistant to your agt.chat rooms, so you can use the AI plan you already pay for inside agt.chat, with no extra credits.

## What it does

- **Catch up:** ask "what did I miss in #release?" and get what was decided, what is still open, and what is waiting on you.
- **Reply in a room:** ask your assistant to answer someone or post an update. It reads the room first, shows you the draft, and posts only when you say so.
- **Keep the board moving:** turn a discussion into tasks, or move a task to in progress, review or done.

## How to use it

1. Add the plugin, then connect agt.chat when asked. You sign in on agt.chat's own page.
2. Pick the space and the rooms the assistant may use. You can change this later in agt.chat, on the Budget page under Connected apps.
3. Ask in plain words, for example "summarize today in #general" or "create tasks from the planning thread".

## What data it sends and where

- The assistant reads only the rooms you picked, through the agt.chat connector at `https://agt.chat/v1/mcp`. It never sees other rooms. End-to-end encrypted rooms cannot be picked, because the server cannot read them.
- Messages it posts appear in the room as your connected app, labeled as such, so others know an AI wrote them.
- Text written by other people reaches the assistant marked as untrusted, and the skills tell it never to follow instructions found there.
- You can disconnect at any time in agt.chat. Its access stops at once.

Privacy policy: https://agt.chat/privacy. Connector guide: https://agt.chat/docs/connector.

## Contents

- `.mcp.json`: the agt.chat connector.
- `skills/catch-up`, `skills/reply-in-room`, `skills/room-tasks`: how to work well in agt.chat rooms.

## License

MIT. See `LICENSE`.
