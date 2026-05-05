# Port Forwarding Tester

A lightweight Node.js HTTP server for testing local port forwarding and connectivity.

## What it does

- Prompts the user to enter a port number.
- Starts an HTTP server bound to `0.0.0.0` on the entered port.
- Returns a simple HTML response confirming the server is running and showing the port.

## Requirements

- Node.js installed (recommended Node 14+).

## Usage

1. Open a terminal in the project folder.
2. Run:

```bash
node server.js
```

3. When prompted, enter the port number you want the server to use. Example:

```text
Enter port: 3000
```

4. Open a browser and visit:

```text
http://0.0.0.0:3000
```

## Notes

- If no valid port is entered, the server defaults to port `3000`.
- Binding to `0.0.0.0` makes the server accessible from other devices on the same network, which is helpful for port forwarding and external access testing.

## Example response

The page will display:

- `It works ✅`
- `Port: <your port>`

## File

- `server.js` — main script for starting the test server.

