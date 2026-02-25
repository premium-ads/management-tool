# Management Tool

Desktop application for Publishers.

## Download

Go to [Releases] (https://github.com/premium-ads/management-tool/releases) and download the latest version for your platform:

| Platform | File |
|---|---|
| macOS Apple Silicon (M1/M2/M3/M4) | `ManagementTool-macos-apple-silicon.zip` |
| macOS Intel | `ManagementTool-macos-intel.zip` |
| Windows | `ManagementTool-windows-amd64.exe` |

## macOS: Fix "damaged and can't be opened" Error

Since the app is not signed with an Apple Developer certificate, macOS Gatekeeper may block it. To fix this:

### Option 1: Terminal command (Recommended)

After downloading and extracting the `.zip` file, open **Terminal** and run:

```bash
xattr -cr "/path/to/Management Tool.app"
```

For example, if you extracted it to the Downloads folder:

```bash
xattr -cr ~/Downloads/Management\ Tool.app
```

Or if you moved it to Applications:

```bash
xattr -cr /Applications/Management\ Tool.app
```

Then double-click the app to open it normally.

### Option 2: System Settings

1. Double-click the app (it will show the error)
2. Open **System Settings** → **Privacy & Security**
3. Scroll down — you'll see a message about "Management Tool" being blocked
4. Click **"Open Anyway"**
5. Enter your password to confirm
