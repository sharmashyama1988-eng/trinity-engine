# 🛡️ God Mode Manual

God Mode is the most powerful module in Trinity Engine. It allows for direct manipulation of the Windows Shell and Process Lifecycle.

## 🔑 Key Features

### 🌑 Shell Overlord
By enabling Shell Overlord, Trinity Engine replaces `explorer.exe` as the default Windows shell. 
- **Benefit:** Reduces background RAM usage by up to 1GB.
- **Risk:** Standard taskbar and start menu will be unavailable.
- **Recovery:** Press `Ctrl+Alt+T` to bring up Trinity Engine or use the built-in Recovery button to restore Explorer.

### ⚡ Priority Matrix
Trinity Engine doesn't just 'close' apps; it intelligently re-assigns CPU cycles.
- **Foreground Boost:** Active windows get `HIGH_PRIORITY_CLASS`.
- **Background Throttling:** Non-essential services are moved to `IDLE_PRIORITY_CLASS`.

### 🧠 Smooth Engine (Stealth)
A background daemon that ensures zero-input-lag by monitoring RAW input buffers and ensuring the renderer has immediate CPU access.
