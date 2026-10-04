# 🎨 APPYness PackageHub

> **Developing Joy!** — A delightful, powerful package management desktop application by [APPYness](https://appyness.dev).

**PackageHub** is a modern WinUI 3 desktop application that brings joy and simplicity to software package management on Windows. Manage multiple package managers (WinGet, Scoop, Chocolatey, Pip, npm, and more) through one beautiful, intuitive interface—**developed by Vincent Kinney and the APPYness team with ❤️**.

---

## ✨ What is PackageHub?

PackageHub transforms the complexity of managing multiple package managers into a seamless, delightful experience. Instead of remembering CLI syntax or juggling multiple tools, you get:

- **🎯 One Dashboard** – Discover, install, update, and uninstall packages from all your favorite package managers
- **⚡ Lightning Fast** – Modern C# / .NET 10 / Windows App SDK architecture optimized for performance
- **🌍 Multilingual** – Community-supported translations in 20+ languages
- **🔧 Deep Integration** – Native support for WinGet, Scoop, Chocolatey, Pip, npm, .NET Tools, PowerShell Gallery, Cargo, and Vcpkg
- **📦 Smart Bulk Operations** – Install, update, or remove multiple packages at once
- **💾 Backup & Restore** – Export package lists and settings for quick setup on new machines
- **🔐 Secure & Private** – Open source (MIT) with full transparency

---

## 🚀 Getting Started

### Installation

Choose your preferred method:

#### Microsoft Store (Recommended)
```
[Store Link Coming Soon]
```

#### Download Installer
**[Download Latest Release](https://github.com/VpkDevs/unigetuiclone2/releases)** – PackageHub.Installer.exe

#### Via WinGet
```powershell
winget install --exact --id APPYness.PackageHub
```

#### Via Scoop
```powershell
scoop bucket add extras
scoop install extras/packagehub
```

#### Via Chocolatey
```powershell
choco install packagehub
```

### First Launch

1. Open PackageHub
2. Ensure your package managers are installed (WinGet, Scoop, Chocolatey, etc.)
3. Click **Scan** to discover available packages
4. Start managing with joy! 🎉

---

## 🎯 Core Features

### 📊 Package Discovery & Management
- Search across all configured package managers simultaneously
- View detailed package metadata: publisher, version, size, dependencies
- Compare packages across managers
- Sort and filter by any criteria

### ⚙️ Advanced Installation Options
- **Custom Installation Parameters** – Choose installation directory, architecture (32/64-bit), and custom flags
- **Version Selection** – Install specific versions or stay on latest
- **Upgrade Strategy** – Auto-update, manual updates, or skip specific packages
- **Batch Operations** – Install, update, or remove dozens of packages in one click

### 📦 Package Management
- **Automatic Updates** – Keep everything current with one-click bulk updates
- **Version Pinning** – Lock specific packages to prevent unwanted upgrades
- **Dependency Resolution** – Automatic handling of package dependencies
- **Package Sharing** – Generate shareable links for your favorite packages

### 💾 Backup & Migration
- **Export Configurations** – Save your entire package setup as JSON
- **Import Configurations** – Quickly restore on new machines with preserved installation parameters
- **Settings Backup** – Full app configuration backup and restore

### 🌐 System Tray Integration
- **Quick Access** – Minimize to system tray for quick package management
- **Update Notifications** – Get notified when updates are available
- **Background Updates** – Optional automatic update checking

---

## 📋 Supported Package Managers

| Manager | Install | Update | Uninstall | Upgrade All | Search | Details | Version Selection |
|---------|---------|--------|-----------|-------------|--------|---------|-------------------|
| **WinGet** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Scoop** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Chocolatey** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Python (pip)** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **npm / Node** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **.NET Tools** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **PowerShell Gallery** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Cargo (Rust)** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |
| **Vcpkg (C++)** | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ | ✅ |

---

## 🏗️ Architecture

PackageHub follows a **modern, modular architecture** designed for extensibility and maintainability:

```
PackageHub/
├── Interface Layer (WinUI 3 XAML)
├── Core Services (Settings, Logging, Localization, Icons)
├── Package Engine (Interfaces, Base Classes, Manager Implementations)
├── Operations Layer (Install, Update, Uninstall, Search)
└── Helper Services (Details, Operations, Source Management)
```

**Key Technologies:**
- **UI Framework:** WinUI 3 (Windows App SDK)
- **Runtime:** .NET 10
- **Language:** C# with latest features (nullable annotations enabled)
- **Build System:** Modern project SDK with code analysis
- **Testing:** xUnit with comprehensive test coverage
- **Code Style:** Strict enforcement via DeepSource and EditorConfig

---

## 📖 Documentation

- **[Architecture Guide](docs/ARCHITECTURE.md)** – Deep dive into the codebase structure
- **[Adding Package Managers](docs/ADD_MANAGER.md)** – Step-by-step guide for new manager integrations
- **[CLI Reference](docs/CLI.md)** – Command-line interface documentation
- **[IPC Reference](docs/IPC.md)** – Inter-process communication API
- **[Contributing Guide](CONTRIBUTING.md)** – How to contribute to PackageHub
- **[Translations](TRANSLATION.md)** – Help translate PackageHub into your language

---

## 🤝 Contributing

We ❤️ contributions! Whether it's bug reports, feature requests, translations, or code contributions, your involvement helps us develop more joy.

### Getting Started with Development

```bash
# Clone the repository
git clone https://github.com/VpkDevs/unigetuiclone2.git
cd unigetuiclone2

# Restore dependencies
dotnet restore

# Run tests
dotnet test --verbosity quiet --nologo

# Build the project
dotnet build src/UniGetUI/UniGetUI.csproj

# Publish release
dotnet publish src/UniGetUI/UniGetUI.csproj /p:Configuration=Release /p:Platform=x64
```

See [CONTRIBUTING.md](CONTRIBUTING.md) for detailed contribution guidelines.

---

## 🌍 Translations

PackageHub is available in 20+ languages thanks to our amazing community translators. Help us reach more users:

- **[View Translation Status](TRANSLATION.md)**
- **[Contribute a Translation](TRANSLATION.md#contributing-translations)**

---

## 📸 Screenshots

### Main Dashboard
![PackageHub Dashboard](media/packagehub-dashboard.png)

### Package Search & Details
![Package Search](media/packagehub-search.png)

### Installation Options
![Installation Options](media/packagehub-install.png)

### Bulk Operations
![Bulk Updates](media/packagehub-bulk.png)

*[View more screenshots](media/)*

---

## ⚙️ System Requirements

- **OS:** Windows 10 (19041) or Windows 11
- **Runtime:** .NET 10 Runtime (automatically installed)
- **Memory:** 512 MB minimum (1 GB recommended)
- **Disk Space:** ~200 MB for installation

### Optional Dependencies
- **Microsoft Visual C++ Redistributable** (for MSI deployment)
- **Microsoft Edge WebView Runtime** (for MSI deployment)

---

## 🔒 Security

PackageHub is open source and thoroughly reviewed. If you discover a security issue, please report it responsibly at [security@appyness.dev](mailto:security@appyness.dev) rather than opening a public issue.

**Disclaimer:** PackageHub is not affiliated with any of the package managers it integrates with. Packages are provided by third-party sources—always review publishers and sources before installation.

---

## 📄 License

PackageHub is released under the **MIT License**. See [LICENSE](LICENSE) for details.

---

## 👏 Credits

**Original Creator:** Martí Climent  
**Current Steward & Lead Developer:** Vincent Kinney (APPYness)  
**Company:** [APPYness](https://appyness.dev) — *Developing Joy!*

### Thanks To
- The amazing open-source community
- All translators contributing to internationalization
- Package manager maintainers (WinGet, Scoop, Chocolatey, etc.)
- Everyone reporting issues and suggesting improvements

---

## 🌟 Status

![Build Status](https://img.shields.io/github/actions/workflow/status/VpkDevs/unigetuiclone2/dotnet-test.yml?branch=main&style=for-the-badge)
![Latest Release](https://img.shields.io/github/v/release/VpkDevs/unigetuiclone2?style=for-the-badge)
![License](https://img.shields.io/badge/license-MIT-blue?style=for-the-badge)
![Downloads](https://img.shields.io/github/downloads/VpkDevs/unigetuiclone2/total?style=for-the-badge)

---

<p align="center">
  Made with ❤️ by <a href="https://appyness.dev">APPYness</a><br>
  <strong>Developing Joy!</strong>
</p>
