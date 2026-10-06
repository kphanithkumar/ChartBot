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
chartbot-og5t8mhnq-phanith1.vercel.app

## Structure
```
client/   React (Vite) UI
server/   Express + Socket.IO
```
Set `VITE_SOCKET_URL` in `client/.env` to point at a deployed server.


<img width="1037" height="667" alt="Image" src="https://github.com/user-attachments/assets/158fc5ea-2661-486b-a929-0e8c108917c0" />
<img width="1091" height="517" alt="Image" src="https://github.com/user-attachments/assets/59f584b0-a14d-4bc0-bc10-772a743c97ba" />

