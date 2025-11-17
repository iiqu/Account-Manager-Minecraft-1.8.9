# Account Manager - Minecraft 1.8.9

A professional Minecraft Forge mod that allows you to switch between multiple Minecraft accounts seamlessly without restarting the game. Perfect for content creators, server administrators, and players who manage multiple accounts.

## ✨ Features

### 🔄 Account Switching
- **Seamless Switching**: Switch between multiple Minecraft accounts without restarting the game
- **Quick Selection**: Single click to select, second click to activate (or double-click for instant switching)
- **Auto-Detection**: Automatically detects and saves your current account as "Default Account"
- **Visual Feedback**: Color-coded account status indicators (green for active, yellow for selected)

### 🎭 Anonymous Mode
- **Privacy Protection**: Hide usernames and UUIDs for privacy during streams
- **Toggle Control**: Easy toggle button to switch between anonymous and normal modes
- **Stream-Friendly**: Shows generic labels like "Account 1", "Account 2 [Active]" instead of real usernames
- **Perfect for Content Creators**: Protect account information while streaming or recording

### 📝 Account Management
- **Add Accounts**: Add new accounts with display name, username, UUID, and access token
- **Edit Accounts**: Modify account information at any time
- **Delete Accounts**: Remove accounts you no longer need
- **Persistent Storage**: All accounts saved to a JSON configuration file

### 🎨 User Interface
- **Minecraft-Style GUI**: Clean interface that fits seamlessly into the game
- **Intuitive Navigation**: Clear visual feedback and easy-to-use controls
- **Scrollable List**: View all your saved accounts in an organized list
- **Status Indicators**: Always know which account is currently active

## 📦 Installation

### Requirements
- **Minecraft Version**: 1.8.9
- **Forge Version**: 11.15.1.2318 (or compatible)
- **Java**: Java 8

### Quick Install

1. **Download the Mod**
   - Download `AccountManager-1.8.9-1.0.1.jar` from the [Releases](https://github.com/iiqu/Account-Manager---Minecraft-1.8.9/releases) page

2. **Install Forge** (if not already installed)
   - Download and install Minecraft Forge 1.8.9 from [files.minecraftforge.net](https://files.minecraftforge.net/net/minecraftforge/forge/)
   - Run the installer and select the "Client" installation

3. **Install the Mod**
   - Open your Minecraft directory:
     - **Windows**: `%appdata%\.minecraft`
     - **macOS**: `~/Library/Application Support/minecraft`
     - **Linux**: `~/.minecraft`
   - Navigate to the `mods` folder (create it if it doesn't exist)
   - Place `AccountManager-1.8.9-1.0.1.jar` into the `mods` folder

4. **Launch Minecraft**
   - Select the Forge profile in the Minecraft launcher
   - Launch the game

## 🚀 Usage

### Accessing the Account Manager

1. Launch Minecraft with the mod installed
2. Navigate to the **Multiplayer** menu
3. Click the **"Account Manager"** button
4. The Account Manager screen will open

### Adding an Account

1. Click the **"Add"** button
2. Fill in the account details:
   - **Display Name**: A friendly name for the account (e.g., "My Main Account")
   - **Username**: Your Minecraft username
   - **UUID**: Your Minecraft UUID (32 hex characters, with or without dashes)
   - **Access Token**: Your Minecraft access token (required for switching)
3. Click **"Save"**

### Switching Accounts

**Method 1: Two-Step Selection**
1. Click once on an account to select it (it will turn yellow)
2. Click again on the selected account to activate it

**Method 2: Double-Click**
- Double-click any account to instantly select and switch to it

**Method 3: Select Button**
1. Click once on an account to select it
2. Click the **"Select"** button at the bottom

### Anonymous Mode

1. Click the **"Anonymous: OFF"** button in the top-right corner
2. The button will change to **"Anonymous: ON"**
3. All usernames and UUIDs will be hidden, replaced with generic labels like "Account 1", "Account 2 [Active]"
4. Click again to toggle back to normal mode

### Editing an Account

1. Select the account you want to edit
2. Click the **"Edit"** button
3. Modify the account details
4. Click **"Save"**

### Deleting an Account

1. Select the account you want to delete
2. Click the **"Delete"** button
3. Confirm the deletion in the confirmation screen

## ⚙️ Configuration

Account data is stored in:
```
.minecraft/accountmanager/account_switcher.json
```

This file contains all your saved accounts in JSON format. You can manually edit this file if needed, but be careful to maintain valid JSON syntax.

## 🔧 Technical Details

### Mod Information
- **Mod ID**: `accountmanager189`
- **Version**: `1.0.1`
- **Minecraft Version**: `1.8.9`
- **Forge Version**: `11.15.1.2318+`

### Features Implementation
- Uses Minecraft's native Session API for account switching
- Stores account data in JSON format for easy editing
- Implements UUID canonicalization for consistent account matching
- Anonymous mode uses visual-only rendering changes (no data modification)

## 🐛 Troubleshooting

### Account Switching Not Working
- **Check Access Token**: Make sure the account has a valid access token
- **Verify UUID Format**: UUIDs should be 32 hex characters (with or without dashes)
- **Check Logs**: Look for error messages in the Minecraft logs

### Mod Not Loading
- **Verify Forge Version**: Make sure you're using Forge 1.8.9
- **Check Mod File**: Ensure the JAR file is in the correct `mods` folder
- **Check Logs**: Review the Minecraft launcher logs for errors

### Accounts Not Saving
- **Check Permissions**: Ensure Minecraft has write permissions to the `.minecraft` folder
- **Verify File Path**: Check that `accountmanager` folder exists in `.minecraft`
- **Check Disk Space**: Ensure you have enough disk space

## 📋 Version History

### Version 1.0.1 (Current)
- Initial release for Minecraft 1.8.9
- Account switching functionality
- Anonymous mode for streaming
- Account management (add, edit, delete)
- Default account detection
- Clean, intuitive UI

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Credits

- **Developer**: IIQU
- **Minecraft**: Mojang Studios
- **Forge**: Minecraft Forge Team

## ⚠️ Disclaimer

This mod is for educational and personal use. Use responsibly and in accordance with Minecraft's Terms of Service. The developers are not responsible for any misuse of this mod.

---

Made with ❤️ for the Minecraft 1.8.9 community

For support, issues, or feature requests, please visit the [GitHub Issues](https://github.com/iiqu/Account-Manager---Minecraft-1.8.9/issues) page.
