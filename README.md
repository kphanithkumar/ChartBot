# Harbor Chat

A single-page React chat app with likes, emoji, @mentions and optional real-time sync through a Socket.IO + Express server.

## Features
- Type a message and press **Send** (or Enter): it appears in the thread above the box
- Each message gets a random user from `["Alan", "Bob", "Carol", "Dean", "Elin"]`
- Like button at the right end of every message with a live count
- **Stretch goals (all done)**
  - Emoji picker
  - `@` mentions: typing `@` lists the users, keep typing to filter, click or press Enter/Tab to pick
  - Socket.IO server (Express): messages and likes are broadcast to every open tab/browser. If the server is off, the app still works locally.

## Run
```bash
npm run install:all
npm run dev
```
- Client: http://localhost:5173
- Server: http://localhost:4000

Client only (no sockets): `cd client && npm install && npm run dev`

Open two browser tabs to see messages and likes sync.

## Structure
```
client/   React (Vite) UI
server/   Express + Socket.IO
```
Set `VITE_SOCKET_URL` in `client/.env` to point at a deployed server.

