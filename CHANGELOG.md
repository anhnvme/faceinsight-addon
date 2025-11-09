# Changelog

All notable changes to this add-on will be documented in this file.
## [1.0.5] - 2025-11-09
- Fix MQTT
- Fix test folder

## [1.0.0] - 2025-10-25

### Added
- Initial release of FaceInsight Home Assistant Add-on
- Face recognition using InsightFace (buffalo_s, buffalo_l, antelopev2 models)
- Web interface for person management
- MQTT integration for Home Assistant automations
- Automatic training from inbox folder
- Recognition history with bounding boxes
- Storage management and cleanup
- Settings page for configuration
- Test page for verification
- Support for nicknames and display names
- Auto-slug name generation from Vietnamese text
- Shared JavaScript utilities
- Image preview modal with ESC key support
- Click-to-view original images

### Features
- Real-time face detection and recognition
- Multi-person support with configurable limits
- Automatic cleanup of old history (30 days retention)
- Model switching (buffalo_s/buffalo_l/antelopev2)
- MQTT notifications with person details
- Docker-based deployment
- Persistent storage in `/config/faceinsight/`
- Health check endpoint
- Responsive web UI

### Configuration Options
- MQTT host, port, credentials, topic

### Known Limitations
- First run takes 2-3 minutes to download models
- Requires at least 5 images per person for good accuracy
- MQTT broker required for notifications
- ARM support limited to ARMv7 and ARM64

### Dependencies
- Python 3.11
- InsightFace
- OpenCV
- Flask
- SQLite
- Paho MQTT
- Watchdog

