# Big Blocks

<p align="center">
  <img src="https://github.com/big-comm/bigblocks/blob/main/usr/share/icons/hicolor/scalable/apps/bigblocks.svg" alt="Big Blocks Logo" width="128" height="128">
</p>

<p align="center">
  <strong>Linux Distribution Themed Puzzle Game</strong>
</p>

<p align="center">
  <a href="https://github.com/big-comm/bigblocks/releases"><img src="https://img.shields.io/badge/Version-1.0.0-blue.svg" alt="Version"/></a>
  <a href="https://bigcommunity.com"><img src="https://img.shields.io/badge/BigCommunity-Platform-blue" alt="BigCommunity Platform"/></a>
  <a href="https://github.com/big-comm/bigblocks/blob/main/LICENSE"><img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License"/></a>
  <a href="https://www.qt.io/"><img src="https://img.shields.io/badge/Qt-6.5+-orange.svg" alt="Qt Version"/></a>
  <a href="https://doc.qt.io/qt-6/qtquick-index.html"><img src="https://img.shields.io/badge/QML-QtQuick-purple.svg" alt="QML QtQuick"/></a>
</p>

## Overview

Big Blocks is an innovative puzzle game that combines classic falling-block gameplay with Linux distribution themes. Each game piece represents a different Linux distro, complete with unique colors, symbols, and special abilities. Challenge yourself with combo chains, perfect clears, and the powerful BigLinux Super Mode!

## Features

- **7 Linux distribution themes**: Ubuntu, Debian, Fedora, Arch Linux, Linux Mint, openSUSE, and BigLinux
- **BigLinux Power System**: Charge and unleash devastating clearing power
- **Ghost piece preview** and hold functionality for strategic gameplay
- **Dynamic scoring** with combos, perfect clears, and level progression
- **Top 5 high scores** with persistent storage and comprehensive statistics
- **Smooth animations**, visual effects, and distro-themed styling

## Screenshots

> Screenshots will be available soon. The game features a modern dark theme with colorful Linux distribution-themed blocks and smooth animations.
<p align="center">
  <img width="722" height="760" alt="bigblock_welcome" src="https://github.com/user-attachments/assets/5b697f7a-25c5-40ad-893d-b9c9eab465ad" />
</p>

<p align="center">
  <img width="722" height="760" alt="bigblocks_game" src="https://github.com/user-attachments/assets/1a020d3d-cdac-4424-8794-4cc38ad66c35" />
</p>



## Installation

### BigCommunity Distributions

If you're using a BigCommunity distribution, simply install via pacman:

```bash
sudo pacman -S bigblocks
```

### Other Arch-based Distributions

For other Arch Linux based distributions, you need to add the BigCommunity repository first:

1. Add the repository to your `/etc/pacman.conf`:

```ini
[community-stable]
SigLevel = PackageRequired
Server = https://repo.communitybig.org/stable/$arch
```

2. Import the GPG keys:

```bash
sudo pacman-key --recv-keys 1EA0CEEEB09B44A3
sudo pacman-key --lsign-key 1EA0CEEEB09B44A3
```

3. Update package databases and install:

```bash
sudo pacman -Sy
sudo pacman -S bigblocks
```

## Game Controls

| Key | Action |
|-----|--------|
| **←/→** | Move piece left/right |
| **↓** | Soft drop (faster descent) |
| **↑/Z** | Rotate piece clockwise |
| **Space** | Hard drop / BigLinux Power (when charged) |
| **C** | Hold current piece |
| **P** | Pause/unpause game |
| **T** | View top 5 scores |
| **Enter** | Start game / Play again |
| **ESC** | Exit confirmation / Return to menu |
| **Y/N** | Confirm/cancel actions |

## Gameplay Mechanics

**Scoring:** Lines cleared give 100-800 × level points, with combo bonuses (50% per combo) and perfect clear bonuses (1000 × level).

**Level Progression:** Advance every 10 lines with increasing speed.

**BigLinux Power:** Charge 15% per line cleared. At 100%, press Space to clear bottom 3 rows and gain 500 × level bonus points.

## Technical Requirements

**Dependencies:** Qt 6.5+ with QML support, QtQuick.Controls 6.5+, QtQuick.Shapes 6.5+

**System:** 256MB RAM, 50MB storage, 700×700 display resolution

## Development

### Building from Source

1. Clone the repository:
```bash
git clone https://github.com/big-comm/bigblocks.git
cd bigblocks
```

2. Install dependencies:
```bash
sudo pacman -S qt6-base qt6-declarative
```

3. Run directly:
```bash
qml usr/share/biglinux/bigblocks/BigBlocks.qml
```

## Contributing

We welcome contributions to Big Blocks! Here's how you can help:

### Bug Reports
- Use GitHub Issues to report bugs
- Include system information and steps to reproduce
- Attach screenshots if relevant

### Feature Requests
- Suggest new Linux distributions to include
- Propose gameplay enhancements
- Request localization for new languages

### Code Contributions
- Fork the repository
- Create a feature branch
- Follow QML coding standards
- Test thoroughly before submitting PR

## Game Statistics

Big Blocks tracks comprehensive gameplay statistics:

- **Pieces placed**: Total pieces used
- **Perfect clears**: Complete board clears
- **Maximum combo**: Highest combo achieved
- **Super mode uses**: BigLinux power activations
- **Top 5 scores**: Best historical performances

## Credits

### Development
- **BigCommunity**: Game design and development
- **Qt Framework**: Cross-platform application framework
- **Linux Community**: Inspiration for distro themes

## License

This project is licensed under the MIT. See the [LICENSE](LICENSE) file for details.

## Support

### Community Support
- **BigCommunity**: [https://communitybig.org/](https://communitybig.org/)
- **GitHub Issues**: [https://github.com/big-comm/bigblocks/issues](https://github.com/big-comm/bigblocks/issues)

### Documentation
- **Qt QML Documentation**: [https://doc.qt.io/qt-6/qtquick-index.html](https://doc.qt.io/qt-6/qtquick-index.html)
