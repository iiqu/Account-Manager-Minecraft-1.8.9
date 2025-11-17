# Account Manager - Minecraft 1.8.9

A Minecraft Forge mod that allows you to switch between multiple Minecraft accounts without restarting the game. Perfect for content creators, server administrators, and players who manage multiple accounts.

## Showcase

### Video Demonstration

**[Watch Full Mod Showcase Video](media/videos/Mod%20Showcase.mp4)** - Complete walkthrough of all features

### Screenshots

**Multiplayer Menu Integration**
![Multiplayer Accounts Button](media/screenshots/Multiplayer%20Accounts%20Button%20Showcase.png)
*The Account Manager button seamlessly integrated into the Multiplayer menu*

**Adding a New Account**
![Add Account Interface](media/screenshots/Add%20Account%20Showcase.png)
*Simple and intuitive interface for adding new accounts with all required information*

**Anonymous Mode**
![Anonymous Mode](media/screenshots/Accounts%20Showcase%20In%20Anonymous.png)
*Privacy protection mode perfect for streaming - hides usernames and UUIDs*

## Features

### Account Switching
Switch between multiple Minecraft accounts seamlessly without restarting. Single click to select, second click to activate, or double-click for instant switching. The mod automatically detects and saves your current account as "Default Account" and provides visual feedback with color-coded account status indicators.

### Anonymous Mode
Hide usernames and UUIDs for privacy during streams. Toggle between anonymous and normal modes with a single button click. In anonymous mode, accounts are displayed as generic labels like "Account 1" or "Account 2 [Active]" instead of real usernames, making it perfect for content creators who want to protect account information.

### Account Management
Add new accounts with display name, username, UUID, and access token. Edit account information at any time or delete accounts you no longer need. All accounts are saved to a JSON configuration file for easy backup and manual editing.

### User Interface
Clean Minecraft-style GUI that fits seamlessly into the game. Intuitive navigation with clear visual feedback, scrollable list showing all saved accounts, and status indicators showing which account is currently active.

## Installation

### Requirements
- Minecraft Version: 1.8.9
- Forge Version: 11.15.1.2318 (or compatible)
- Java: Java 8

### Installation Steps

1. **Download the Mod**
   - Download `account-manager-1.8.9.jar` directly from the repository

2. **Install Forge** (if not already installed)
   - Download and install Minecraft Forge 1.8.9 from [files.minecraftforge.net](https://files.minecraftforge.net/net/minecraftforge/forge/index_1.8.9.html)
   - Run the installer and select the "Client" installation

3. **Install the Mod**
   - Open your Minecraft directory:
     - Windows: `%appdata%\.minecraft`
     - macOS: `~/Library/Application Support/minecraft`
     - Linux: `~/.minecraft`
   - Navigate to the `mods` folder (create it if it doesn't exist)
   - Place `account-manager-1.8.9.jar` into the `mods` folder

4. **Launch Minecraft**
   - Select the Forge profile in the Minecraft launcher
   - Launch the game

## Usage

### Accessing the Account Manager

Launch Minecraft with the mod installed, navigate to the Multiplayer menu, and click the "Account Manager" button. The Account Manager screen will open.

### Adding an Account

Click the "Add" button and fill in the account details:
- Display Name: A friendly name for the account (e.g., "My Main Account")
- Username: Your Minecraft username
- UUID: Your Minecraft UUID (32 hex characters, with or without dashes)
- Access Token: Your Minecraft access token (required for switching)

Click "Save" to add the account.

### Switching Accounts

**Method 1: Two-Step Selection**
1. Click once on an account to select it (it will turn yellow)
2. Click again on the selected account to activate it

**Method 2: Double-Click**
- Double-click any account to instantly select and switch to it

**Method 3: Select Button**
1. Click once on an account to select it
2. Click the "Select" button at the bottom

### Anonymous Mode

Click the "Anonymous: OFF" button in the top-right corner to toggle anonymous mode. When enabled, all usernames and UUIDs will be hidden and replaced with generic labels. Click again to toggle back to normal mode.

### Editing an Account

Select the account you want to edit, click the "Edit" button, modify the account details, and click "Save".

### Deleting an Account

Select the account you want to delete, click the "Delete" button, and confirm the deletion in the confirmation screen.

## Configuration

Account data is stored in:
```
.minecraft/accountmanager/account_switcher.json
```

This file contains all your saved accounts in JSON format. You can manually edit this file if needed, but be careful to maintain valid JSON syntax.

## Technical Details

**Mod Information:**
- Mod ID: `accountmanager189`
- Version: `1.0.1`
- Minecraft Version: `1.8.9`
- Forge Version: `11.15.1.2318+`

**Implementation:**
- Uses Minecraft's native Session API for account switching
- Stores account data in JSON format for easy editing
- Implements UUID canonicalization for consistent account matching
- Anonymous mode uses visual-only rendering changes (no data modification)

## Troubleshooting

### Account Switching Not Working
- Check Access Token: Make sure the account has a valid access token
- Verify UUID Format: UUIDs should be 32 hex characters (with or without dashes)
- Check Logs: Look for error messages in the Minecraft logs

### Mod Not Loading
- Verify Forge Version: Make sure you're using Forge 1.8.9
- Check Mod File: Ensure the JAR file is in the correct `mods` folder
- Check Logs: Review the Minecraft launcher logs for errors

### Accounts Not Saving
- Check Permissions: Ensure Minecraft has write permissions to the `.minecraft` folder
- Verify File Path: Check that `accountmanager` folder exists in `.minecraft`
- Check Disk Space: Ensure you have enough disk space

## Version History

### Version 1.0.1
- Initial release for Minecraft 1.8.9
- Account switching functionality
- Anonymous mode for streaming
- Account management (add, edit, delete)
- Default account detection
- Clean, intuitive UI

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Credits

- Developer: IIQU
- Minecraft: Mojang Studios
- Forge: Minecraft Forge Team

## Disclaimer

This mod is for educational and personal use. Use responsibly and in accordance with Minecraft's Terms of Service. The developers are not responsible for any misuse of this mod.

---

For support, issues, or feature requests, please visit the [GitHub Issues](https://github.com/iiqu/Account-Manager-Minecraft-1.8.9/issues) page.
