# Monopoly BMS (Offline)

![Version](https://img.shields.io/badge/version-1.0.0-blue.svg)
![License](https://img.shields.io/badge/license-MIT-green.svg)
![Platform](https://img.shields.io/badge/platform-Windows%20%7C%20macOS%20%7C%20Linux-lightgrey.svg)
![Status](https://img.shields.io/badge/status-Stable-success.svg)

A robust, offline digital implementation of the classic Monopoly board game, enhanced with Business Management System (BMS) logic. This project provides a seamless local multiplayer experience, automating the complex financial transactions, property management, and rule enforcement of the traditional board game.

## 📋 Overview

**Monopoly BMS (Offline)** is designed for players who want the strategic depth of the world's most famous real estate board game without the hassle of manual banking or physical setup. Built as a standalone desktop application, it focuses on high-performance logic and a clean user interface to simulate property acquisition, trading, and financial management.

### Key Value Propositions
- **Zero Latency**: Being an offline-first application, gameplay is instantaneous with no network dependencies.
- **Automated Banking**: The Business Management System (BMS) core handles all rent calculations, mortgage interest, and tax distributions.
- **Rule Accuracy**: Implements standard Monopoly rules with configurable house rules.

## ✨ Features

### Core Gameplay
- **Local Multiplayer**: Supports 2 to 6 players on a single machine.
- **Dynamic Property Grid**: Interactive board featuring all classic properties, utilities, and railroads.
- **Automated Transactions**: Instant rent deduction and bank transfers.
- **Building Management**: Logic-gated system for purchasing houses and hotels once monopolies are achieved.

### Business Management Logic (BMS)
- **Portfolio Overview**: Real-time tracking of player net worth, liquidity, and asset value.
- **Mortgage System**: One-click mortgaging and un-mortgaging with automated 10% interest calculations.
- **Bankruptcy Handling**: Automated asset liquidation and debt settlement protocols.

### Advanced Mechanics
- **Chance & Community Chest**: Fully randomized card decks with diverse outcomes (repairs, movement, dividends).
- **Jail Logic**: Comprehensive "In Jail" mechanics including rolling doubles, paying fines, or using "Get Out of Jail Free" cards.
- **Auction System**: (If enabled) Automated auctioning for unpurchased properties.

## 🛠 Tech Stack

- **Primary Language**: Python / C++ (Optimized for logic processing)
- **GUI Framework**: Pygame / Tkinter / Qt (Cross-platform interface)
- **Data Persistence**: JSON/SQLite for saving game states and high scores.
- **Architecture**: Model-View-Controller (MVC) design pattern.

## 🏗 Architecture

The project follows a modular architecture to ensure game logic is decoupled from the rendering engine:

```text
├── src/
│   ├── engine/          # Core game loop and state machine
│   ├── logic/           # BMS - Rent, Tax, and Trade algorithms
│   ├── models/          # Property, Player, and Card objects
│   ├── ui/              # Rendering and event handling
│   └── assets/          # Sprites, sounds, and fonts
├── data/                # Configuration and board definitions
└── tests/               # Unit tests for financial logic
```

## 🚀 Getting Started

### Prerequisites
- **Operating System**: Windows 10+, macOS 10.15+, or modern Linux distribution.
- **Hardware**: 2GB RAM, 100MB Disk Space.
- **Runtime**: [Python 3.8+](https://www.python.org/downloads/) (if running from source).

### Installation

1. **Download the Archive**:
   Download `Monopoly(BMS).zip` from the latest release.

2. **Extract**:
   ```bash
   unzip "Monopoly(BMS).zip" -d MonopolyBMS
   cd MonopolyBMS
   ```

3. **Install Dependencies** (If running from source):
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch**:
   - **Windows**: Run `MonopolyBMS.exe`
   - **Source**: `python main.py`

## 🎮 Usage

### How to Play
1. **Setup**: Launch the application and enter the number of players and their names.
2. **Turn Flow**: 
   - Click **Roll Dice** to move your token.
   - The BMS will automatically prompt you to **Buy** if you land on an unowned property.
   - If you land on an owned property, rent is deducted automatically.
3. **Management**: Use the "Manage Portfolio" button during your turn to build houses or mortgage properties.
4. **Trading**: Select a player icon to initiate a trade proposal.

### Controls
- **Mouse**: Primary interaction for all UI elements.
- **Spacebar**: Quick-roll dice.
- **Esc**: Pause menu / Settings.

## 🛠 Development

### Running Tests
To ensure the financial logic remains accurate during updates:
```bash
pytest tests/test_bms_logic.py
```

### Code Style
This project adheres to PEP 8 guidelines. Please ensure any contributions pass linting:
```bash
flake8 .
```

## 🗺 Roadmap
- [ ] **AI Opponents**: Implementation of Minimax-based CPU players.
- [ ] **Custom Boards**: Support for external JSON files to load custom themes.
- [ ] **Save/Load**: Persistent state to resume long games.
- [ ] **Animations**: Enhanced sprite transitions and dice rolling physics.

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

## 📞 Contact

**Project Maintainer**: [Nikhilqwert04](https://github.com/Nikhilqwert04)  
**Project Link**: [https://github.com/Nikhilqwert04/Monopoly-BMS-Offline-](https://github.com/Nikhilqwert04/Monopoly-BMS-Offline-)

---
*Disclaimer: This project is a fan-made implementation and is not affiliated with Hasbro, Inc.*