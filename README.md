# SpatialNVR Plugin Catalog

Official catalog of plugins for [SpatialNVR](https://github.com/Spatial-NVR/SpatialNVR).

## How It Works

SpatialNVR fetches this catalog to display available plugins in the Plugins page. The catalog is refreshed periodically and can be manually refreshed from the UI.

## Plugin Structure

```yaml
plugins:
  - id: plugin-id           # Unique identifier
    name: Plugin Name       # Display name
    description: ...        # Short description
    category: camera        # One of: camera, detection, integration, storage, notification
    repository: https://... # GitHub repository URL
    author: Author Name     # Plugin author
    official: true          # Maintained by Spatial-NVR team
    verified: true          # Tested and verified to work
    status: available       # available, coming-soon, deprecated
    icon: https://...       # URL to plugin icon (optional)
    features:               # List of features
      - Feature 1
      - Feature 2
    requirements:           # System requirements (optional)
      - Requirement 1
    supported_devices:      # For camera plugins (optional)
      - Device 1
```

## Adding Your Plugin

Want your plugin listed in the catalog?

1. Ensure your plugin follows the [Plugin Development Guide](https://github.com/Spatial-NVR/SpatialNVR/blob/main/docs/plugins/DEVELOPMENT.md)
2. Create a GitHub release with pre-built binaries
3. Open a Pull Request adding your plugin to `catalog.yaml` under `community_plugins`
4. Once reviewed and verified, we'll merge it into the catalog

## Official Plugins

| Plugin | Category | Status |
|--------|----------|--------|
| [Reolink](https://github.com/Spatial-NVR/reolink-plugin) | Camera | ✅ Available |
| [Wyze](https://github.com/Spatial-NVR/wyze-plugin) | Camera | ✅ Available |
| [Frigate](https://github.com/Spatial-NVR/frigate-plugin) | Detection | ✅ Available |
| [Home Assistant](https://github.com/Spatial-NVR/homeassistant-plugin) | Integration | ✅ Available |
| [HomeKit](https://github.com/Spatial-NVR/homekit-plugin) | Integration | 🔜 Coming Soon |
| [MQTT Publisher](https://github.com/Spatial-NVR/mqtt-plugin) | Integration | ✅ Available |
| [Telegram](https://github.com/Spatial-NVR/telegram-plugin) | Notification | 🔜 Coming Soon |
| [Pushover](https://github.com/Spatial-NVR/pushover-plugin) | Notification | 🔜 Coming Soon |

## License

MIT License
