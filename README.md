# Nevera Weather Sync

**Nevera Weather Sync** is a premium FiveM resource that synchronizes real-time weather and clock in-game using data from the real world through the OpenWeatherMap API.

---

## Features

- **Real-time Weather Synchronization** – Fetches weather data from any city
- **Dynamic Time Synchronization** – Syncs in-game time with real time
- **Automatic Weather Transitions** – Smooth weather changes
- **Advanced Wind System** – Real wind speed and direction
- **Notification System** – Weather info every 10 minutes
- **Resource-Efficient** – 0.01ms idle performance
- **Fallback Mechanism** – Works even when API is down
- **Fog and Snow Control** – Fully configurable
- **Multi-Framework Compatible** – ESX, QBCore, vRP, Standalone
- **Easy Configuration** – Full control via `config.lua`

---

## Requirements

- **FiveM Server** – Latest version
- **OpenWeatherMap API Key**
- Works with: **ESX**, **QBCore**, **vRP**, **Standalone**

---

## Installation

1. Purchase and download from Tebex
2. Extract to your server `resources` folder
3. Add this to your `server.cfg`:

```cfg
# Nevera Weather Sync Configuration
set my_sync_key "YOUR_API_KEY"           # Your OpenWeatherMap API key
set my_sync_timezone "Europe/London"     # Your timezone
set my_sync_city "London"                # Your city
set nevera_license_key "LICENSE_KEY"     # Your Tebex license key
set disable_fog "true"                   # Set to "false" to enable fog

ensure nevera-weather-sync
```

---

## Getting Your API Key

1. Visit [OpenWeatherMap](https://openweathermap.org/)
2. Register a free account
3. Go to **API Keys**
4. Generate a key and paste it into `server.cfg`

---

## Configuration (`config.lua`)

Example settings:

```lua
Config.OpenWeatherAPIKey = "YOUR_KEY"
Config.City = "London"
Config.Timezone = "Europe/London"
Config.NotificationDuration = 15000
Config.DisplayFormat = "topLeft"
Config.DisableFog = true
Config.UseSnow = true
Config.WeatherUpdateInterval = 600000
Config.EnableWind = true
Config.HighWindThreshold = 10
```

---

## Performance

- Idle: **0.01ms**
- Update: **0.02-0.03ms**
- Memory usage: Minimal

---

## Compatibility

| Framework     | Supported |
|---------------|-----------|
| ESX           | ✅         |
| QBCore        | ✅         |
| vRP           | ✅         |
| Standalone    | ✅         |
| Custom        | ✅         |

---

## Version History

### v1.1.0 – May 2025
- Server-side response caching
- Fallback API system
- Performance improvements
- Enhanced wind system

### v1.0.0 – Initial Release
- Real-time weather and time sync
- Notifications
- Multi-framework support

---

## Screenshots

**1. Weather Sync**
![Data Sync](https://i.imgur.com/8S7uUxb.png)

**2. API Response**
![Update](https://i.imgur.com/axpJm9s.png)

**3. Resource Monitor**
![Resmon](https://i.imgur.com/0L9ETkn.png)

**4. Clock Overlay**
![Clock](https://i.imgur.com/CovWD3l.png)

---

## FAQ

**How can I extend the duration of the weather notification?**  
In the `config.lua` file, you can change the `Config.NotificationDuration` setting to your desired number of milliseconds.  
For example, for a display lasting 30 seconds:

```lua
Config.NotificationDuration = 30000  -- 30 seconds (30000 ms)
```

---

## Support

- 💬 Discord: [discord.gg/DA9FZ4RmpG](https://discord.gg/DA9FZ4RmpG)
- ✉️ Email: nevera.rp@gmail.com

---

## License

Single-server usage only. Redistribution and modifications are forbidden.

© 2025 Nevera. All rights reserved.

---

## LICENSE

```markdown
# Nevera Weather Sync - Commercial License

## Software License Agreement

This Software License Agreement (the "Agreement") is a legal agreement between you (either an individual or a single entity) and Nevera ("Author") for the software product identified above, which includes computer software and associated media and documentation (the "Software").

By installing, copying, or otherwise using the Software, you agree to be bound by the terms of this Agreement. If you do not agree to the terms of this Agreement, do not install or use the Software.

## 1. GRANT OF LICENSE

### 1.1 Single Server License
This license grants you the right to install and use the Software on a single FiveM server instance.

### 1.2 Restrictions
You may NOT:
- Use the Software on more than one FiveM server instance without purchasing additional licenses
- Distribute, share, lease, rent, sell, or sublicense the Software
- Modify, decompile, reverse-engineer, disassemble or create derivative works based on the Software
- Remove any proprietary notices or labels on the Software
- Use the Software for illegal or unauthorized purposes

## 2. INTELLECTUAL PROPERTY AND OWNERSHIP

The Software is protected by copyright laws and international copyright treaties, as well as other intellectual property laws and treaties. The Software is licensed, not sold. The Author retains all rights, title, and interest in and to the Software, including all intellectual property rights.

## 3. TERM AND TERMINATION

This Agreement is effective until terminated. The Author may terminate this Agreement if you fail to comply with any term or condition of this Agreement. Upon termination, you must destroy all copies of the Software and all of its component parts.

## 4. NO WARRANTIES

The Author expressly disclaims any warranty for the Software. The Software is provided "AS IS" without any express or implied warranty of any kind, including but not limited to any warranties of merchantability, non-infringement, or fitness for a particular purpose.

## 5. LIMITATION OF LIABILITY

In no event shall the Author be liable for any damages (including, without limitation, lost profits, business interruption, or lost information) arising out of the use of or inability to use the Software, even if the Author has been advised of the possibility of such damages.

## 6. GENERAL

This Agreement constitutes the entire agreement between you and the Author and supersedes any prior statements, representations, or agreements, whether oral or written.

## 7. GOVERNING LAW

This Agreement shall be governed by the laws of Croatia.

Copyright © 2025 Nevera. All rights reserved.
```
