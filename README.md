<p align="center">
  <img src="assets/icon.png" alt="MaxAtoms" width="120" height="120" style="border-radius: 20px;">
</p>

<h1 align="center">MaxAtoms</h1>

<p align="center">
  <strong>Free, open-source Windows gaming optimizer.</strong><br>
  Strip the bloat. Tune your system. Unlock every frame.
</p>

<p align="center">
  <a href="https://github.com/adamsmacker/maxatoms/releases/latest"><img src="https://img.shields.io/github/v/release/adamsmacker/maxatoms?style=flat-square&color=00e5ff&label=Download" alt="Download"></a>
  <a href="LICENSE"><img src="https://img.shields.io/badge/License-MIT-c850c0?style=flat-square" alt="License"></a>
  <a href="https://github.com/adamsmacker/maxatoms/stargazers"><img src="https://img.shields.io/github/stars/adamsmacker/maxatoms?style=flat-square&color=00e5ff" alt="Stars"></a>
  <img src="https://img.shields.io/badge/Platform-Windows%2010%2F11-0078D6?style=flat-square&logo=windows" alt="Platform">
</p>

---

## What is MaxAtoms?

MaxAtoms is a **one-click Windows optimizer** designed specifically for gaming. It disables unnecessary services, tunes power settings, optimizes network configs, and clears system overhead — so your hardware can focus on what matters: your game.

No ads. No upsells. No telemetry. Just performance.

---

## Features

**⚡ Power Plan Tuning** — Activates high-performance power plans and adjusts CPU scheduling to eliminate micro-stutters and keep clocks boosted.

**🧹 Bloat Removal** — Disables unnecessary background services, startup apps, and Windows telemetry that steal CPU cycles.

**🌐 Network Optimization** — Tunes TCP/IP settings and disables Nagle's algorithm to reduce latency in online games.

**🎮 GPU Priority** — Configures Windows to prioritize GPU resources for your game, reducing render queue delays and input lag.

**💾 Memory Management** — Clears standby memory, optimizes page file settings, and reduces fragmentation for sustained performance.

**🛡️ Safe & Reversible** — Every optimization creates a system restore point first. One click to apply, one click to undo.

---

## Quick Start

### 1. Download

Grab the latest release from the [Releases page](https://github.com/adamsmacker/maxatoms/releases/latest).

### 2. Extract & Run

Unzip the archive and run `MaxAtoms.exe`. No installation required.

> **Note:** Windows may show a SmartScreen warning since the app isn't code-signed. Click **"More info" → "Run anyway"** to proceed. The app is fully open-source — you can inspect every line of code.

### 3. Optimize

Click the optimize button. MaxAtoms will:
1. Create a system restore point
2. Apply all selected optimizations
3. Show you exactly what changed

That's it. Game on.

---

## System Requirements

| Requirement | Details |
|---|---|
| **OS** | Windows 10 or Windows 11 |
| **Permissions** | Run as Administrator (required for system-level tweaks) |
| **Runtime** | None — fully self-contained |
| **Disk Space** | ~50 MB |

---

## How It Works

MaxAtoms applies a curated set of Windows optimizations using PowerShell scripts under the hood. Every tweak targets a specific performance bottleneck:

| Category | What It Does | Why It Helps |
|---|---|---|
| Power Plan | Switches to Ultimate Performance plan, disables core parking | Prevents CPU throttling during gameplay |
| Services | Disables non-essential background services | Frees CPU and memory for your game |
| Network | Disables Nagle's, optimizes TCP settings | Reduces network latency (lower ping) |
| GPU | Sets hardware-accelerated GPU scheduling, adjusts priority | Reduces input lag and render queues |
| Memory | Clears standby list, optimizes page file | Prevents stutters from memory pressure |
| Visual Effects | Disables unnecessary Windows animations | Frees GPU and CPU resources |

---

## Reverting Changes

Changed your mind? No problem.

**Option A:** Use the built-in revert button inside MaxAtoms to undo all changes.

**Option B:** Use the Windows System Restore point that MaxAtoms created automatically before optimizing.

---

## FAQ

**Is this safe?**
Yes. MaxAtoms only makes changes that are fully reversible through Windows System Restore. It doesn't modify system files, patch executables, or touch anything that can't be undone.

**Will this get me banned in games?**
No. MaxAtoms doesn't interact with any game process, inject code, or modify game files. It only adjusts Windows system settings — the same tweaks you'd find in any Windows optimization guide.

**Does it work on laptops?**
Yes, but some power plan optimizations may increase battery drain. MaxAtoms will warn you before applying laptop-sensitive tweaks.

**Why not just use [other optimizer tool]?**
Most optimizer tools are closed-source, bundled with ads, or try to upsell you on a "Pro" version. MaxAtoms is 100% free, open-source, and transparent. You can read every line of code and see exactly what it does.

---

## Building from Source

```bash
# Clone the repo
git clone https://github.com/adamsmacker/maxatoms.git
cd maxatoms

# Install dependencies
npm install

# Run in development mode
npm run dev

# Build for production
npm run build
```

### Tech Stack

- **Electron + Vite** — Desktop app framework
- **JavaScript** — Core application logic
- **PowerShell** — System optimization scripts

---

## Contributing

Contributions are welcome! If you'd like to add a new optimization, fix a bug, or improve the UI:

1. Fork the repo
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

Please open an issue first for major changes so we can discuss the approach.

---

## Roadmap

- [ ] Game-specific optimization profiles
- [ ] Benchmark mode (before/after FPS comparison)
- [ ] Auto-detect installed games
- [ ] Scheduled optimization runs
- [ ] Community-contributed tweak packs

---

## License

[MIT](LICENSE) — free to use, modify, and distribute.

---

<p align="center">
  <strong>Built by a gamer who was tired of bloated optimizer tools.</strong><br>
  If MaxAtoms helped your FPS, consider giving it a ⭐ on GitHub.
</p>
