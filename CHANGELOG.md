# Changelog

All notable changes to the Meduseld services hub.

## Recent Updates

### Services
- Added Jellyfin media server integration with status monitoring
- Enabled real-time status checks for game server panel
- Enabled SSH terminal access with availability monitoring
- Integrated Steam news feed for current game

### UI/UX Improvements
- Fixed game server panel title to display "{Game Name} Server" format
- Made tooltips clickable on mobile devices for better accessibility
- Added Bootstrap tooltip support with click and hover triggers
- Improved mobile experience for info icons and status badges

### Features
- Automatic service status checks every 30 seconds
- Collapsible game news panel with Steam API integration
- Server specifications display
- Games queue showing upcoming titles
- Discord integration widget

### Technical
- Status monitoring using fetch with timeout controls
- No-CORS mode for cross-origin status checks
- Responsive design with Bootstrap 5.3.2
- Dynamic content updates based on configuration
