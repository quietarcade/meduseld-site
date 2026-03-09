# Meduseld Services

A service hub for managing game servers, media streaming, and other services hosted on meduseld.io.

## Features

- Game server control panel with real-time status monitoring
- Jellyfin media server access
- SSH terminal access
- Game news feed from Steam
- Server specifications display
- Upcoming games queue

## Services

### Game Server Panel
Control and monitor the current game server (Icarus). Start, stop, restart, and check server status in real-time.

### Jellyfin Media Server
Stream movies, TV shows, and other media content through the Jellyfin server.

### SSH Access
Secure shell access to the server via web-based terminal.

### Game Wiki
Community wiki with guides, tips, and information for the current game (coming soon).

## Configuration

The site uses a configuration object in `menu/index.html` to manage service URLs and game information:

```javascript
const CONFIG = {
  gameName: 'Icarus',
  gameAppId: '1149460',
  panelUrl: 'https://panel.meduseld.io',
  sshUrl: 'https://ssh.meduseld.io',
  terminalUrl: 'https://terminal.meduseld.io',
  wikiUrl: 'https://wiki.meduseld.io',
  jellyfinUrl: 'https://jellyfin.meduseld.io'
};
```

## Status Monitoring

All active services perform automatic status checks every 30 seconds to ensure real-time availability information.
